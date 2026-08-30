# Pomodoros

Shared pomodoro timer for [Delta Chat](https://delta.chat), built as a [webxdc](https://webxdc.org) app.

Two-phase focus + break timer with pie chart visualization. Choose 25 or 50 minute sessions. Tap the pie to reveal remaining time. Chat members are notified when time is up.

Multilingual symbol-based UI — no text labels to translate.

## Screenshots

<p align="center">
<img src="screenshots/01.png" width="280" alt="Chat preview showing timer status">
<img src="screenshots/02.png" width="280" alt="Timer idle, ready to start">
<img src="screenshots/03.png" width="280" alt="Timer running with time overlay">
</p>

## Install

Download `pomodoros.xdc` from the [latest release](https://github.com/maphouse/pomodoros/releases/latest) and send it as a file in any Delta Chat conversation.

## Development

Requires [webxdc-dev](https://github.com/niclas/webxdc-dev) for local testing.

```bash
npx webxdc-dev app/
```

Package for Delta Chat:

```bash
(cd app/ && zip -9 --recurse-paths - *) > pomodoros.xdc
```
