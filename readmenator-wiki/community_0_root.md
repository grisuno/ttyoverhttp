# root

*Community 0 | 1 files | cohesion 1.00*

## Definition

This community groups 1 file(s) rooted at `root` with dominant language py (cohesion 1.00). Central symbols: `AllTheReads`, `ReadCmd`, `RunCmd`, `SetupShell`, `WriteCmd`, `__init__`, `run`, `sig_handler`. Core file: `tty_over_http.py` (8 symbols).

## Files

| File | Language | Layer | Symbols | Doc |
|------|----------|-------|---------|-----|
| `tty_over_http.py` | py | presentation | 8 | no |

## Key Symbols

- `AllTheReads` (class, `tty_over_http.py:7`) `class AllTheReads(object)`
- `__init__` (method, `tty_over_http.py:8`) `def __init__(self, interval)`
- `run` (method, `tty_over_http.py:14`) `def run(self)`
- `RunCmd` (method, `tty_over_http.py:24`) `def RunCmd(cmd)`
- `WriteCmd` (method, `tty_over_http.py:33`) `def WriteCmd(cmd)`
- `ReadCmd` (method, `tty_over_http.py:42`) `def ReadCmd()`
- `SetupShell` (method, `tty_over_http.py:47`) `def SetupShell()`
- `sig_handler` (method, `tty_over_http.py:66`) `def sig_handler(sig, frame)`

## Internal vs External Edges

- Internal resolved imports (EXTRACTED): 0
- Cross-boundary resolved imports (EXTRACTED): 0

## Connections

- No cross-community bridges recorded. This community is self-contained.

## Risks

- [taint medium] `tty_over_http.py` -> `tty_over_http.py` via `requests` (0 hops)

## Open Questions

- Why do 1 file(s) lack file-level docs (e.g. `tty_over_http.py`)? What purpose do they serve?
- Is the dangerous import `requests` in `tty_over_http.py` still required, or can it be isolated?
- What would break if the most connected file in root changed?
- Should root be split, given cohesion 1.00?

## Sources

- `tty_over_http.py`
