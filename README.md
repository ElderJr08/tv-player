# tv-player

A one-page YouTube player for a TV home screen app (webOS) that runs from a local file.

YouTube refuses embedded players on pages without a web address (error 153). The TV app shows this page in a frame
instead, so the trailer plays inside the app: `https://elderjr08.github.io/tv-player/?v=VIDEO_ID&mute=1`.

It holds no keys or personal data: only the player. It reports what happens to the app with `postMessage`
(`{tvPlayer: 'ready' | 'playing' | 'paused' | 'ended' | 'error'}`) and takes `play`, `pause`, `mute` and `unmute`.
