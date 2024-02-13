# SaveGuard - Palworld Preservation Protocol

SaveGuard is a Python script designed to automatically backup the save data for Palworld game servers running on Windows. It helps prevent loss of game progress in case of server restarts or crashes.

## Features

- Automatic periodic (houlry) backup of Palworld save data.
- Customizable backup file paths.
- Logging to track backup operations.

## Requirements

- Python 3.x
- `python-dotenv` library (install via `pip install python-dotenv`)

### Prerequisites

Before running SaveGuard, ensure you have Python installed on your system. Follow these steps to install Python:

1. **Download Python:** 
    - Go to the [official Python website](https://www.python.org/downloads/).
    - Choose the appropriate installer for your operating system (Windows, macOS, or Linux).
    - Download the installer and follow the installation instructions provided on the website.

2. **Add Python to System Environment Variables:**
   - After installing Python, add the Python installation directory to the system environment variables. This step allows you to run Python commands from any directory in the command prompt or terminal.
   - **Windows:**
     - Search for "Environment Variables" in the Start menu and select "Edit the system environment variables."
     - In the System Properties window, click on the "Environment Variables..." button.
     - Under "System variables," select the "Path" variable and click "Edit..."
     - Click "New" and add the path to the Python installation directory (e.g., `C:\Users\[user]\AppData\Local\Programs\Python\Python[version number]`). 


Where [user] is your windows username and [version number] is the version you installed with no brackets.

See the image [here](https://docs.python.org/3/using/windows.html)

     - Click "OK" to save the changes and close the windows.

   - restart the system.
    
3. **Verify Installation:**
    - Open a terminal or command prompt.
    - Type `python --version` and press Enter.
    - If Python is installed correctly, you should see the installed Python version printed in the terminal.



## Installation

1. Clone this repository to your local machine:

- git clone https://github.com/NemesisGuy/SaveGuard---Palworld-Preservation-Protocol.git

2. Install the required dependencies:

- pip install python-dotenv

3. Configure the `.env` file with your desired save data and backup paths.

4. Run the script:

-  python saveguard.py


## Configuration

SaveGuard uses a `.env` file to manage configuration settings. You can customize the following settings:

- `SAVE_DATA_PATH`: Path to the Palworld save data directory.
- `BACKUP_PATH`: Path to the directory where backups will be stored.

Example of where the save game might be found, this will vary depending on your install location and your setup:
 - 'C:\Users\UserName\SteamCmd\Steamapps\common\palserver\pal\Saved\SaveGame'

## Donation

If you find SaveGuard useful and would like to support its development, consider making a donation. Your contribution helps maintain and improve the project.

### How to Donate

You can donate using the following methods:

1. **PayPal:** [Donate via PayPal](https://www.paypal.com/donate/?hosted_button_id=5NCF4SUNPZQP8)

Your support is greatly appreciated!

## Usage

Once configured, SaveGuard will automatically run in the background and perform backups according to the specified interval. You can monitor the backup process by checking the logs in the `saveguard.log` file.

## Contributing

Contributions are welcome! Feel free to submit bug reports, feature requests, or pull requests to help improve SaveGuard.


## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.



