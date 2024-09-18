# SoundCloud Stream Analysis

This project analyzes SoundCloud streaming logs to identify unusual changes in stream counts, which may indicate potential fake streams. It processes JSON data containing log information for various tracks, evaluates the gradients of stream counts over time, and visualizes the results through plots.
Features

    Data Loading: Reads streaming log data from a JSON file.
    Log Grouping: Groups logs by track name and organizes counts over time.
    Data Cleaning: Removes invalid records where the stream count decreases from one log to the next.
    Gradient Analysis: Calculates gradients of stream counts to detect unusual spikes.
    Unusual Change Reporting: Identifies tracks with significant changes in stream patterns.
    Fake Stream Probability Calculation: Estimates the likelihood of fake streams based on unusual points.
    Data Visualization: Generates plots to visualize stream counts and highlight unusual changes.

# Requirements

    Python 3.x
    NumPy
    Matplotlib
    JSON

# Usage

    Ensure that you have the required libraries installed.
    Place your SoundCloud logs in a JSON file named soundcloudLogs.json.
    Run the script to analyze the logs:

    bash

    python your_script_name.py

    Review the console output for warnings and reports of unusual changes.
    Check the generated JPG files for visual representations of the stream counts.

# Example Output

The analysis will output warnings for tracks with insufficient data or constant log times and display unusual changes for other tracks. It will also produce visual plots that highlight the detected anomalies.
Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to enhance functionality or fix bugs.
License

This project is licensed under the MIT License. See the LICENSE file for more details.
