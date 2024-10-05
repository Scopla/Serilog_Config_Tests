# Reproduce error

- Checkout repo
- place breakpoint
- observe through the debugger which formatter is set
  - should show Serilog.Formatting.Compact.CompactJsonFormatter
- change the submodule branch to dev
- update the submodule with git submodule update --remote
- debug again
- should now set the expected formatter Serilog.Formatting.Json.JsonFormatter
