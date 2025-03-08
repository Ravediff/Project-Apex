# Apex Launcher (Alpha Build)

Apex Launcher is an alpha build of a game launcher/installer, similar to Steam, designed to manage your game installations and downloads. This application scrapes a game database for titles and allows users to download games and their corresponding magnet links. It automatically scrapes data on app startup and provides a simple search functionality.

## Features

- Automatically scrapes games from a database.
- Search games by name.
- Display game titles with clickable links.
- Retrieve magnet links for game downloads.
- Light and fast user interface (currently in alpha).

## Installation

1. **Download the installer:**
   - Visit the [Release Page](https://github.com/Ravediff/Project-Apex/releases) to download the latest `.exe` file for Windows.

2. **Install the application:**
   - Run the `.exe` file to begin the installation.
   - Follow the on-screen instructions to complete the installation.

3. **Launch Apex Launcher:**
   - After installation, you can launch Apex Launcher from the Start menu or Desktop shortcut.

## Usage

1. **Launching the app:**
   - When you first launch Apex Launcher, it will automatically start scraping for games from the database.
   
2. **Searching for games:**
   - Use the search bar at the top to filter the list of games.
   - The results will show game titles that match your query.

3. **Viewing game details:**
   - Double-click on any game title in the list to open its magnet link in your default browser for downloading.

4. **Managing games:**
   - Games will be listed and scraped automatically when the app starts.

## Requirements

- **Windows 7 or higher**
- **.NET Framework 4.5 or later** (Usually pre-installed on most modern Windows systems)
- **Internet connection** for scraping game data and retrieving magnet links.

## How It Works (Under the Hood)

1. **Web Scraping:**
   - The app scrapes game titles and magnet links from a specified game database URL.
   - It automatically detects the total number of pages and iterates over them to gather all game data.

2. **Game List and Magnet Links:**
   - The app uses an internal list to display games and links. When a game is clicked, it fetches the magnet link from the game detail page.

3. **Auto-Scraping:**
   - As soon as the app is opened, it scrapes the game list and updates the display with the available games.

## Development

This project is built using **C#** and **WPF** for the user interface. The scraping functionality is powered by the **HtmlAgilityPack** library.

### To build from source:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/Apex-Launcher.git
    ```

2. Open the solution in **Visual Studio**:
    - Open `Apex-Launcher.sln` in Visual Studio.

3. Restore NuGet packages (if needed):
    - Right-click the solution and select **Restore NuGet Packages**.

4. Build the solution:
    - Click **Build > Build Solution** or press **Ctrl + Shift + B**.

5. Run the application:
    - After building, run the app directly from Visual Studio or navigate to the output folder to execute the `.exe` file.

## Known Issues

- The app is still in the **alpha** phase, and there may be occasional bugs or incomplete features.
- UI is basic and will be improved in future updates.
- The application might take a few seconds to load and scrape game data, depending on the internet speed and server response.

## Contributing

Contributions are welcome! If you have ideas for new features or encounter bugs, feel free to create an issue or submit a pull request.

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Commit your changes and push to your forked repository.
4. Create a pull request to merge your changes into the main repository.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
