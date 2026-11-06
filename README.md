# Icons-Only Task Manager 2

## 1.4.5

- Added an Appearance option to enable or disable the click bounce animation.
- Added an option to restrict parabolic rise to only the icon under the pointer.
- Both new options default to off, preserving the original dock behaviour for new installs.
- Retained the configurable parabolic rise animation duration (50-500 ms; default 175 ms).

macOS-like icon dock for Plasma 6: zoom on hover, configurable parabolic rise, optional single-icon rise and click bounce, and pinned launchers.

https://store.kde.org/p/2352806/

## 1.4.4

- Click bounce is driven by the persistent task list, so it also appears on the
  first click of a pinned launcher while the launcher transitions into a startup
  entry or running task.

## 1.4.3

- Parabolic rise now animates smoothly on hover and when moving between icons.
- The rise animation duration is adjustable in Appearance settings (50-500 ms).

## 1.4.2

- A left-click makes the activated icon perform one bounce.
- Parabolic rise affects only the icon directly under the pointer.

## 1.4.1

- Magic Lamp follows the painted icon, including on a scaled screen.
- Clicking a dock icon still launches or minimizes if icon geometry cannot be published.

## 1.4

- Magic Lamp and the normal minimize animation target the dock icon.
  The dock publishes each icon's screen rectangle to KWin.
- Meta+1 through Meta+9 activates the matching dock entry (launch, focus,
  or minimize), same as the standard task manager. If the default
  Icons-Only Task Manager is still on the panel, Plasma gives the
  shortcut to that one.

## 1.3

- Works on Plasma 6.7 / CachyOS / Arch **without** the Fedora `arch-patch` binary.
  The widget no longer imports `org.kde.plasma.private.taskmanager`.
- Drop a `.desktop` onto the dock to pin that app.
- Drop a regular file onto the empty strip after the last icon to pin the
  default application for that file type.
- Drop a file onto an existing icon to open it with that app.
- Drop highlight no longer clips against the panel.

Context menu no longer has Jump Lists / Recent Files / Places (those needed
the private C++ plugin). Mute, MPRIS, pin/unpin, desktops still work.
