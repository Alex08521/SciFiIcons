# SciFi Icons
Sours is an SVG icon theme for Linux. It is a descendant of [Beautyline](https://store.kde.org/p/1425426) and [Candy](https://github.com/EliverLara/candy-icons) icons, with [Sweet](https://github.com/EliverLara/Sweet-folders) and [Beauty Solar](https://store.kde.org/p/2037657)-inspired folders and substantial original artwork added to complete the theme, based on [Sours](https://store.kde.org/p/2214536)

Features:

- Tasty gradients
- Monochrome system tray (up to 38px panel size or 'small' in tray settings)
- Color-coordinated (files match their app and directory)
- Sci-fi inspired gaps
- Rounded lines
- Uplit

## Installation
- Extract SciFi_Icons.tar.gz to ~/.local/share/icons

or

- In System Settings -> Appearance -> Icons, use the 'Install from File...' dialog to find and select SciFi_Icons.tar.gz

then

- In System Settings -> Appearance -> Icons, select Sours and click Apply (lower right)
- It may be necessary to log out and log back in or restart to fully apply the icon theme (icon caches are stubbornly persistent)

### For Dolphin to use the provided symbolic icons for named folders (like Downloads or Github) it may be necessary to:
- Right-click the folder and open Properties
- Click the icon next to its name
- Choose the corresponding icon in the dialog

### If an app has a white icon in your app launcher (like KeepassXC):
- Right-click the app in your application launcher
- Select "Edit Application"
- On the General tab, click the app's icon and use the icon browser dialog to choose the properly colored icon

### If the icon in the app's titlebar is incorrect (like a Wayland W or a stock icon):
### or
### If an app uses a different icon after it is launched (like Kvantum Preview or Battle.net):
- You can tell KDE which desktop file to use for a particular app by creating a Window Rule:
    - Open the titlebar context menu and navigate to More Actions -> Configure Special Application Settings... -> Add Property -> Desktop file name -> Force -> put the preferred desktop file name
    - .desktop files are located in either ~/.local/share/applications or /usr/share/applications
    - If something goes wrong, delete the Window Rule in System Settings -> Window Management -> Window Rules (default naming scheme: Application settings for "app")
- Explanation: .desktop files are metadata for their corresponding application. Sometimes the metadata that KDE assigns an app when it is installed is different from the metadata that apps send KDE. Using a Window Rule to force KDE to use a particular .desktop file for a particular app means that KDE will use the icon, name, and description specified in that .desktop file to represent the app
- I use this method to correct the OpenRGB icon (desktop file name OpenRGB), to give Kvantum Preview the Kvantum Manager icon (desktop file name kvantummanager), and to make Battle.net behave (desktop file name net.lutris.battlenet-1 if installed through Lutris). 

### Contributing
Icon themes are inevitably a work in progress. Please open an issue if you notice any stock or broken icons, or to make an icon request.

### License

This project is licensed under the GNU GPL v3 - see the [LICENSE.md](LICENSE.md) file for details.

