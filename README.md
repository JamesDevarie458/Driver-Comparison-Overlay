# F1 Driver Comparison

Compare Formula 1 drivers using official session timing data.

The project uses [FastF1](https://docs.fastf1.dev/) to load race-weekend sessions, then looks at qualifying results and laps so two drivers can be compared on the same weekend. The current notebook loads 2026 Spanish Grand Prix qualifying and pulls results for Andrea Kimi Antonelli and Max Verstappen, with lap selection as the next step toward a side-by-side comparison.

## What's in the repo

`Untitled.ipynb` is the working notebook. It:

1. Loads a session with FastF1 (`2026`, Spanish Grand Prix, qualifying).
2. Prints the session results.
3. Looks up individual drivers by abbreviation (`ANT`, `VER`).
4. Starts selecting laps for a driver so those laps can be compared.

Matplotlib and NumPy are imported for the charts that comparison will use.

## Run the notebook

Use the project virtual environment and open `Untitled.ipynb`. FastF1 downloads session data on first load and stores it in `cache/`. Live timing endpoints may ask for Formula 1 account credentials via `F1_USERNAME` and `F1_PASSWORD`; without them, some telemetry is unavailable and the notebook still loads the timing results it can reach.
