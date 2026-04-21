# Project Guidelines

## Mandatory Development Checklist
- [ ] `uv sync`
- [ ] `uv run ruff check .`
- [ ] `uv run pytest`
- [ ] Build/run verification: `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000`

## Build and Test
- Runtime: Python 3.13+ with `uv`.
- Key commands:
  - `uv sync`
  - `uv run ruff check .`
  - `uv run pytest`
  - `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000`

## Architecture and Conventions
- Stack: FastAPI + Jinja2 + HTMX.
- Main boundaries:
  - `app/main.py`: routes and app wiring.
  - `app/game_service.py`: `GameSession` and in-memory session state.
  - `app/game_logic.py`: pure board and bingo logic.
- Keep business logic in Python modules, not templates.
- HTMX endpoints should return fragments that replace `#game-container`.
- Preserve template roles:
  - `app/templates/home.html` picks start vs game screen.
  - `app/templates/components/start_screen.html` and `app/templates/components/game_screen.html` are swap roots.
  - `app/templates/components/bingo_board.html` renders the grid.

## References
- Styling rules: `.github/instructions/css-utilities.instructions.md`
- Setup workflow: `.github/prompts/setup.prompt.md`
- Workshop guide: `workshop/GUIDE.md`
- Contribution process: `CONTRIBUTING.md`
- Never use VS Code Simple Browser for app preview.
