# OOSL

Open-source Android launcher targeting OnePlus 6T (`fajita`), Jaguar / Android 11,
as an ordinary third-party Home app. Based on Neo Launcher 0.9.3 at
`022833f7df33d01e1a64c17d928a812e88555e63`.

- Application ID: `hu.szecsi.oosl` (including debug builds)
- Application title: **OOSL**
- Development branch: `oosl`
- Current signing: upstream public **debug key only**; no production signing configured
- System Recents stays with the ROM launcher; QuickSwitch is not required

The first milestone is an offline left-page Shelf with persistent Notes.
Shelf implementation has not started. Native Steps, Parking Location and
OxygenOS 10 visual fidelity are later milestones. This is an independent project.

## Build the debug APK

Use JDK 11, Android SDK Platform 33 and Build-Tools 30.0.3. The wrapper provides
Gradle 7.5.1. Set `JAVA_HOME` and `ANDROID_HOME` for your local installations, then:

```sh
bash ./gradlew assembleAospWithQuickstepOmegaDebug
```

The APK is under `build/outputs/apk/aospWithQuickstepOmega/debug/`.
The `withQuickstep` source variant is required by the inherited launcher classes;
building it does not make OOSL the system Recents provider.
Only the debug build is currently supported. Its key is public and is not suitable
for production distribution. Existing Neo packages can remain installed separately.

## Upstream credits and licensing

OOSL retains Neo/Omega, Lawnchair and AOSP source notices and the upstream license.
The original Neo Launcher README follows for attribution and upstream information;
its download links refer to Neo, not OOSL.

---

# Neo Launcher <img title="" src="./fastlane/metadata/android/en-US/images/icon.png" align="left" width="64">

**Free and Open Source Launcher**
<br/>
[![GitHub repo stars](https://img.shields.io/github/stars/NeoApplications/Neo-Launcher?style=flat)](https://github.com/NeoApplications/Neo-Launcher/stargazers)
[![GitHub License](https://img.shields.io/github/license/NeoApplications/Neo-Launcher)](https://github.com/NeoApplications/Neo-Launcher/blob/A-12/LICENSE)
[![GitHub All Releases](https://img.shields.io/github/downloads/NeoApplications/Neo-Launcher/total.svg)](https://github.com/NeoApplications/Neo-Launcher/releases/)
[![GitHub release](https://img.shields.io/github/v/release/NeoApplications/Neo-Launcher?display_name=tag)](https://github.com/NeoApplications/Neo-Launcher/releases/latest)
[![Small translation badge](https://hosted.weblate.org/widgets/omegalauncher/-/omegalauncher/svg-badge.svg)](https://hosted.weblate.org/engage/omegalauncher/?utm_source=widget)

[![Neo Applications Banner](neo_banner.png)](https://github.com/NeoApplications)

## *Installation & Download*

Our builds are available on:

- **Github**: [Releases](https://github.com/NeoApplications/Neo-Launcher/releases).

- **F-Droid**: On **[IzzyOnDroid repo](https://apt.izzysoft.de/fdroid/repo?fingerprint=3BF0D6ABFEAE2F401707B6D966BE743BF0EEE49C2561B9BA39073711F628937A)** or **[our own repo (only for test)](https://raw.githubusercontent.com/nonaybay/newomega/master/fdroid/repo)**.

- **Telegram**: [Neo Applications channel](https://t.me/neo_applications).

## *Community*

You can join either our [Telegram](https://t.me/neo_launcher) or [Matrix](https://matrix.to/#/#neo-launcher:matrix.org) groups to make suggestions, ask questions, receive news, or just chat.

## *App features:*

### **Some of the main features**

- Rich themes support.
- The Dash.
- Custom search engines.
- Gestures support.
- A unique custom-widget.
- Categories or folders in the app drawer.
- Icon shapes and packs support.
- Customize app icons.
- Desktop grid preference.
- Hide apps.
- Vertical Apps Lists.
- Icons' scaling.
- Back up and restore preferences.

There's also a [developer's document](DEVDOC.md), where the maintainer and collaborators communicate
their TODOs and plans.

## *Screenshots*

<table>
    <tr>
        <td><img src="https://raw.githubusercontent.com/otakuhqz/Omega/omega-11/snapshots/omega1.jpg" alt="" width="256"></td>
        <td><img src="https://raw.githubusercontent.com/otakuhqz/Omega/master/snapshots/omega2.jpg" alt="" width="256"></td>
        <td><img src="https://raw.githubusercontent.com/otakuhqz/Omega/omega-11/snapshots/omega3.jpg" alt="" width="256"></td>
        <td><img src="https://raw.githubusercontent.com/otakuhqz/Omega/master/snapshots/omega4.jpg" alt="" width="256"></td>
    </tr>
    <tr>
        <td><img src="https://raw.githubusercontent.com/otakuhqz/Omega/omega-11/snapshots/omega5.jpg" alt="" width="256"></td>
        <td><img src="https://raw.githubusercontent.com/otakuhqz/Omega/master/snapshots/omega6.jpg" alt="" width="256"></td>
        <td><img src="https://raw.githubusercontent.com/otakuhqz/Omega/master/snapshots/omega7.jpg" alt="" width="256"></td>
        <td><img src="https://raw.githubusercontent.com/otakuhqz/Omega/master/snapshots/omega8.jpg" alt="" width="256"></td>
    </tr>
</table>

## *Contributions*

**If you have knowledge in Java or Kotlin you can work on additional features or bugs, and open pull requests. Make sure the code is formatted before make a pull request.**

**You can also contribute to this project by opening issues for bugs or new features.**

## *Support*

<a href="https://www.paypal.com/paypalme/saulhdev"><img src="https://img.shields.io/badge/Paypal-Donate-blue?style=for-the-badge&logo=paypal" alt="Donate via PayPal"/></a>

## *FAQ*
Is QuickSwitch available?
No, it's not, and there is no plans to add it.

## *Credits*

#### Thanks to The LawnchairLauncher team for the great work on Lawnchair.

#### Thanks to <a href="https://github.com/machiav3lli">Antonios Hazim</a> for creating the logo and his great contributions in the project.

#### Thanks to <a href="https://github.com/nonaybay">Rafael Venâncio</a> for creating the F-Droid repo.

#### Thanks to Helena Zhang and Toby Fried for the great [Phosphor icons](https://phosphoricons.com), which we use since 0.9.0.

## *Translation*

Translations are handled via Weblate. If want to help, visit <a href="https://hosted.weblate.org/projects/omegalauncher">Hosted Weblate</a>.

#### **Translation stats:** [<img align="right" src="https://hosted.weblate.org/widgets/omegalauncher/-/287x66-white.png" alt="Übersetzungsstatus" />](https://hosted.weblate.org/engage/omegalauncher/?utm_source=widget)

<img src="https://hosted.weblate.org/widgets/omegalauncher/-/multi-red.svg" />
