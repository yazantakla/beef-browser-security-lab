# Lab Notes and Evidence Map

## Purpose

Document the visible outcomes of a local BeEF session and separate direct observations from interpretations.

## Run outline recorded by the evidence

1. Start BeEF using `beef-xss-start` from the Kali Linux terminal.
2. Open the BeEF web interface on the loopback host.
3. Open the local demo page and observe the browser listing in the BeEF console.
4. Inspect the browser Details and Logs tabs.
5. Review configuration screens for Fake Notification Bar (Firefox) and TabNabbing.
6. Enter a harmless test string into the local text field and inspect the available event log evidence.

The screenshots are documentary artifacts rather than a reproducible script. This repository intentionally does not include executable payloads or instructions to target third-party browsers.

## Evidence map

| Screenshot | Directly visible | Interpretation limit |
|---|---|---|
| 01 | BeEF startup output and local authentication page | Does not prove a vulnerability in a target application |
| 02 | BeEF Getting Started page | Interface overview only |
| 03 | Local page titled The Butcher | Does not show the source code or injection point |
| 04 | BeEF control panel | UI state only |
| 05 | Browser Details with Firefox 128.0 / Linux x86_64 values | Values are browser-reported; cookie-like identifier redacted |
| 06 | Log view with browser events | Only events shown in the table are confirmed |
| 07 | Fake Notification Bar (Firefox) configuration | Configuration is not by itself proof of successful execution; private lab host redacted |
| 08 | Notification-style banner at the top of the demo page | Screenshot captures a visible banner, not whether a user was deceived |
| 09 | TabNabbing configuration and module history | Does not establish real-world phishing success |
| 10 | Local page with empty text field | Page display only |
| 11 | Local page with a harmless test string | Does not prove the string was transmitted or exfiltrated |
| 12 | Focus, blur, and textarea mouse-click entries | Does not establish complete keystroke logging |

## Reporting language

Use wording such as “The lab console displayed…”, “The screenshot records…”, and “The observed log contains…”. Avoid stronger wording unless additional evidence exists, for example “XSS vulnerability exploited”, “credentials captured”, or “session hijacked”.
