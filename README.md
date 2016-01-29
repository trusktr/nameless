# nameless

A project that isn't named yet.

## high-level TODOs

Let's create a separate branch for each TODO item, then merge into master.

- [ ] Get an arbitrary app running full screen in X directly after boot (no desktop environment) in some linux distro. (We could use Systemd+ArchLinux for this, for example, to make sure the app restarts when it crashes). We can keep the alternate terminals active (ctrl+alt+f1/f2/f3...), for the advanced users to play with.
- [ ] Now let's get a browser view (Chromium, Webktit, Electron, or etc) running full screen in this X setup.
- [ ] Provide access to OS features via the browser JavaScript environment (done if we choose Electron in the previous step, via Node.js).
- [ ] Make a user login system (perhaps it needs to interact with PAM).
- [ ] Make a web-based desktop for the user to interact with after login.
- [ ] Use the browser's native plugin system to run a linux app (an app that relies on Xorg, for now) inside a `<div>` of the webtop.
- [ ] Make desktop features. For example, make the `<div>` that is wrapping the linux app a window-like thing that we can move around on the webtop, like we do in Gnome, Windows, OS X, etc. Add a menu system for browsing apps, workspaces, alt-tab behavior, etc, for desktop, tablet, and mobile. An idea: When a window is maximized maybe that puts all windows in maximized form and the mode becomes mobile (like Android or iOS where we get a pile of cards to move between apps). When we un-maximize, the windows float again.
- [ ] Write an app system inside of this webtop that let's us add other web apps from anywhere on the web based on a URL, or that let's us add apps from a catalogue that we maintain and expose via an app in the webtop.
- [ ] Once this app system accepts web-based apps, add a permissions system.
- [ ] Once we have a permissions system we can add support for apps that run native Linux applications. Idea: Maybe we can provide each app a light-weight systemd-nspawn container for it's filesystem.
