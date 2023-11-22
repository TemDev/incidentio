# Render Schedule

This script, `render-schedule.py`, is designed to process a schedule and override information based on specified command-line arguments.

## Usage

Make sure Python3 is installed on the computer.

To run the script, use the following command:

```bash
./render-schedule --schedule=schedule.json --overrides=overrides.json --from='2023-11-17T17:00:00Z' --until='2023-12-01T17:00:00Z'
```

Command-line Arguments

--schedule: Path to the schedule JSON file.

--overrides: Path to the overrides JSON file.

--from: Start date and time in ISO format ('YYYY-MM-DDTHH:mm:ssZ').

--until: End date and time in ISO format ('YYYY-MM-DDTHH:mm:ssZ').

Script Logic

Parsing Command-line Arguments:
The script uses the argparse module to parse command-line arguments, specifying the schedule file, overrides file, start date, and end date.
Processing Schedule:
Reads the main schedule from the specified JSON file.
Populates the schedule based on a handover interval and user information.
Generates entries in the schedule until the specified start and end dates.
Processing Overrides:
Reads override information from the specified JSON file(s).
Modifies the schedule based on the override periods, handling various conditions and edge cases.
Running the Script:
Execute the script with the provided command, replacing the placeholders with actual file paths and date-time values.