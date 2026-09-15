# Drive to University

A small Android app with one job: get you turn-by-turn navigation to campus in one tap.

Launch it, and after a short splash screen you land on a single button. Tapping it fires an explicit intent to the Google Maps app, pointed at campus coordinates, and hands off to Maps for the actual navigation.

## Requirements

- Google Maps installed on the device (the app launches it directly via `com.google.android.apps.maps`)

## Where things live

- `SplashActivity` — shows the splash screen, then moves to `MainActivity` after a few seconds
- `MainActivity` — the single navigate button, wired to a `google.navigation:` intent
