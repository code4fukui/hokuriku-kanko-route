# hokuriku-kanko-route

This project provides interactive visualizations of tourist movement and congestion in Japan's Hokuriku region. It uses open data from WiFi packet sensing, originally collected by Kanazawa University and published by the Hokuriku Inbound Tourism DX Data Consortium. The raw data is processed and made available in the [code4fukui/mac-address](https://github.com/code4fukui/mac-address) repository.

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

## Demo

-   **[Hokuriku Tourism Movement Trajectory](https://code4fukui.github.io/hokuriku-kanko-route/)**
    
    An interactive map visualizing visitor flow. Locations are marked with circles sized according to visitor numbers. You can select a specific location to see popular routes originating from it (blue lines) or trace an individual anonymous user's journey (green lines).

-   **[Hokuriku Tourism Congestion by Time of Day](https://code4fukui.github.io/hokuriku-kanko-route/traffic.html)**
    
    A line chart for comparing visitor traffic. Select up to four tourist facilities to visualize and compare their congestion levels by time of day.

## Features

-   **Movement Trajectory Map:** Visualizes popular travel routes between tourist spots and displays individual, anonymized visitor paths.
-   **Congestion Chart:** Compares hourly visitor traffic patterns across multiple, user-selected locations.
-   **Interactive Interface:** Allows users to filter data by location or individual user to explore movement patterns.
-   **Client-Side:** Runs entirely in the browser with no server-side setup required.

## Getting Started

### Using the Live Demos

The easiest way to use this tool is to access the live demos linked above.

### Running Locally

1.  Clone the repository:
    ```sh
    git clone https://github.com/code4fukui/hokuriku-kanko-route.git
    ```
2.  Navigate to the project directory:
    ```sh
    cd hokuriku-kanko-route
    ```
3.  Open `index.html` (for the trajectory map) or `traffic.html` (for the congestion chart) directly in your web browser.

## Data Sources

-   **Processed Data:** [code4fukui/mac-address](https://github.com/code4fukui/mac-address) - Processed CSV files derived from the original WiFi packet sensing data.
-   **Original Data:** [hokuriku-inbound-kanko/mac-address](https://github.com/hokuriku-inbound-kanko/mac-address) - Raw WiFi packet sensing data from Kanazawa University.
-   **Data Publisher:** [Hokuriku Inbound Tourism DX Data Consortium](https://kanko-dx.jp/case-study/1784/)
-   **Data Portal:** [TIFDATA Hokuriku Tourism Data Portal](https://tifdata.jp/)

## License

MIT License — see [LICENSE](LICENSE).