# fogata-libwebrtc

Builds of libwebrtc for [Fogata](https://github.com/holypandadev/Fogata) on Linux and Windows:
WebRTC at a pinned branch-head, with webrtc-sdk's C++ wrapper and Fogata's patches, made by
`tools/webrtc` in the Fogata repository (see its `README.md`). Only VP8 and Opus are built in.

Each release is one version (`fogata-libwebrtc.m<milestone>.<branch-head>.<n>`) and holds an
archive per system:

    libwebrtc-linux-x64-release.zip
    libwebrtc-win-x64-release.zip

Fogata's build downloads them from here and refuses any archive whose SHA-256 is not the one
`app/third_party/flutter_webrtc/third_party/libwebrtc_version.ini` names. The same sources
and patches give the same archive, byte for byte: anyone can build one again and compare
(`tools/webrtc/README.md`, "Checking an archive").

Each archive carries the licence of WebRTC and of every library built into it (`LICENSE`,
`NOTICE.md`).
