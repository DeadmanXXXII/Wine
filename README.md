# Wine
Linux subsystem for windows

# Comprehensive List of Wine Commands

## Wine-Specific Commands

- **Check Wine version:**
  ```bash
  wine --version
  ```

- **Configure Wine settings:**
  ```bash
  winecfg
  ```

- **Install a Windows application with Wine:**
  ```bash
  wine setup.exe
  ```

- **Run a Windows application with Wine:**
  ```bash
  wine application.exe
  ```

- **Uninstall a Windows application with Wine:**
  ```bash
  wine uninstaller
  ```

- **View Wine logs:**
  ```bash
  wine application.exe &> wine.log
  ```

- **Run a Windows application as a different Windows version:**
  ```bash
  WINEPREFIX=~/.wine winecfg
  ```

- **Set environment variables for Wine:**
  ```bash
  WINEPREFIX=~/.wine WINEARCH=win64 wine application.exe
  ```

- **List all installed Windows applications in Wine:**
  ```bash
  wine uninstaller
  ```

- **Update Wine to the latest version (for WineHQ builds):**
  ```bash
  sudo apt update
  sudo apt upgrade --install winehq-stable
  ```

- **Create a new Wine prefix:**
  ```bash
  WINEPREFIX=~/newwineprefix winecfg
  ```

- **Remove a Wine prefix:**
  ```bash
  rm -rf ~/wineprefix
  ```

- **Run a Windows executable with Wine in 32-bit mode:**
  ```bash
  WINEARCH=win32 wine application.exe
  ```

- **Run a Windows executable with Wine in 64-bit mode:**
  ```bash
  WINEARCH=win64 wine application.exe
  ```

- **Verify Wine installation and configuration:**
  ```bash
  wine --check
  ```

- **Run Wine in debug mode:**
  ```bash
  WINEDEBUG=+relay wine application.exe
  ```

- **Install a DLL with Winetricks:**
  ```bash
  winetricks dllname
  ```

- **Create a Wine virtual desktop:**
  ```bash
  winecfg
  ```

## General Wine-Related Tasks

### Wine Configuration and Management

- **Install Winetricks:**
  ```bash
  sudo apt install winetricks
  ```

- **Update Winetricks:**
  ```bash
  winetricks --self-update
  ```

- **List available Winetricks components:**
  ```bash
  winetricks --list-all
  ```

- **Remove a Wine component:**
  ```bash
  winetricks --uninstall component
  ```

### Troubleshooting Wine Applications

- **Check Wine application compatibility:**
  ```bash
  https://appdb.winehq.org/
  ```

- **Check Wine logs for errors:**
  ```bash
  wine application.exe &> wine.log
  ```

- **Reset Wine configuration:**
  ```bash
  rm -rf ~/.wine
  ```

### Wine Application Management

- **List installed applications:**
  ```bash
  wine uninstaller
  ```

- **Modify Wine application settings:**
  ```bash
  winecfg
  ```

- **Run Wine in different desktop environments:**
  ```bash
  WINEPREFIX=~/.wine wine application.exe
  ```

### File Management with Wine

- **Access Wine virtual drive from Linux:**
  ```bash
  cd ~/.wine/drive_c/
  ```

- **Create shortcuts for Windows applications:**
  ```bash
  ln -s ~/.wine/drive_c/Path/To/Application.exe ~/Desktop/Application
  ```

### Wine and Wine Staging

- **Install Wine Staging (development version):**
  ```bash
  sudo apt update
  sudo apt install --install-recommends winehq-staging
  ```

- **Switch between Wine stable and Wine Staging:**
  ```bash
  sudo apt install --install-recommends winehq-stable
  sudo apt install --install-recommends winehq-staging
  ```

### Miscellaneous

- **Generate a Wine crash report:**
  ```bash
  WINEDEBUG=+seh wine application.exe
  ```

- **Run Wine in virtual desktop mode:**
  ```bash
  winecfg
  ```

- **Configure Wine for specific Windows applications:**
  ```bash
  winecfg
  ```

- **Generate a debug log for Wine:**
  ```bash
  WINEDEBUG=+debug wine application.exe &> debug.log
  ```

### Wine System Integration

- **Access Windows system directories from Wine:**
  ```bash
  cd ~/.wine/drive_c/Windows/System32
  ```

- **Access Windows user profiles from Wine:**
  ```bash
  cd ~/.wine/drive_c/Users/YourUsername
  ```

This list provides a broad range of commands and utilities for managing Wine and running Windows applications on Linux through Wine. It includes installation, configuration, troubleshooting, and integration commands.
