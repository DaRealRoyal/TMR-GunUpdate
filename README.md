# Tactical Math Returns

Tactical Math Returns (TMR) is an eco-friendly multiplayer game, where you can virtually plant trees.  
Due to licensing issues we can't publish the source.

Website: [tacticalmath.games/](https://tacticalmath.games/)  
If you can't reach tacticalmath.games, there may be an issue with you DNS servers.  
You can change them to [Cloudflare 1.1.1.1](https://developers.cloudflare.com/1.1.1.1/setup/), [Google Public DNS](https://developers.google.com/speed/public-dns/docs/using), [Quad9](https://www.quad9.net/service/service-addresses-and-features) or any other good DNS servers.

You can download the game through the [TacticalLauncher for Windows](https://tacticalmath.games/windows) or as a [Flatpak for Linux](https://tacticalmath.games/linux).  
The Android version is available on the [Google Play Store](https://play.google.com/store/apps/details?id=com.DaRealRoyal.TacticalMathReturns).

## Server

You can get the server as a Docker image from the [GitHub Container Registry](https://github.com/DaRealRoyal/TacticalDocker/pkgs/container/tmr_server).  
Here is a simple docker-compose.yml for it:

```yaml
version: "3.9"

services:
  tmr_server:
    image: ghcr.io/darealroyal/tmr_server:latest
    restart: unless-stopped
    ports:
      - 7777:7777/udp
```

---

All game files are also available without any update functonality from the [Releases Tab on this Repository](https://github.com/DaRealRoyal/TacticalMathReturns/releases).  
The .zip file is for Windows and the .tar.xz file is for Linux. The .apk and the .obb is for Android (you need to install both). TMR_Server.tar.xz is the server for Linux.
