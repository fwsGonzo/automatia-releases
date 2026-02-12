# automatia-releases

Public release packages for the Automatia game.

## Automated Release Publishing

This repository is configured to automatically publish draft releases. When a draft release is created (typically from the private automatia repository), a GitHub Actions workflow will automatically:

1. Publish the draft release (make it public)
2. Mark it as the latest release

The packages included in each release:
- `automatia-linux.zip`
- `automatia-macos.zip`
- `automatia-windows.zip`

No manual intervention is required - just create the draft release and the automation will handle the rest.