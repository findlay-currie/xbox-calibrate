# Xbox Stick Calibrator

Android app that permanently recalibrates Xbox Series X|S controller thumbsticks over USB. It sends the same calibration commands as Microsoft's Xbox Accessories app, and the controller saves the result in its own memory.

**Download:** https://findlay-currie.github.io/xbox-calibrate/

## Layout

| Path | What it is |
|---|---|
| `index.html` | Download page (the GitHub Pages site) |
| `XboxStickCalibrator.apk` | The app |
| `android/` | App source: `calibrator.html` is the app's screen, `MainActivity.java` gives it USB access, `build.sh` builds the APK |

## Notes

- Needs controller firmware 5.19.3221.0 or later and a USB-C data cable.
- Starting a calibration erases that stick's stored calibration until it finishes.
- Calibration can't fix a worn stick part.
- Protocol from [xboxctl](https://github.com/bb441db/xboxctl) (0BSD). Not affiliated with Microsoft.
