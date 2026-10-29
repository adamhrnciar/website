# HYPERION CanSat website

Website of team HYPERION (Piaristické gymnázium Jozefa Braneckého, Trenčín), finalist of the
Slovak [CanSat](https://www.esa.int/Education/CanSat) 2026 competition.

Live: https://hyperion.potter.software

## The CanSat

- **Primary mission:** temperature and pressure logged at 5 Hz to SD card, with live telemetry
  to the ground station.
- **Secondary mission:** autonomous precision landing. Quadcopter arms deploy after release and a
  Raspberry Pi Zero 2W runs ArUco marker detection to guide a MambaF405 MK2 flight controller
  (ArduPilot) onto a 3×3 m target.
- **Engineering note:** the full Critical Design Review is in
  [`public/TN_HYPERION_CDR.pdf`](public/TN_HYPERION_CDR.pdf).

## Development

```sh
npm install
npm run dev      # local dev server
npm run build    # production build into dist/
```

Pushes to `main` deploy to GitHub Pages via `.github/workflows/deploy.yml`.
