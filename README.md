# Godot Beginner Tutorial Brackeys

https://www.youtube.com/watch?v=LOhfqjmasi0

## Development Environment

```bash
winget install WingetPathUpdater                  # https://github.com/microsoft/winget-cli/issues/222#issuecomment-1675434402
winget install --id=GodotEngine.GodotEngine  -e   # Godot 4.2.2
winget install Microsoft.DotNet.SDK.8             # NET 8.0 SDK (v8.0.302):
winget install -e --id Microsoft.VisualStudioCode # VSCode
winget install --id Git.Git -e --source winget    # git
```

# To debug

godot --headless --generate-mono-glue modules/mono/glue --rendering-driver opengl3
