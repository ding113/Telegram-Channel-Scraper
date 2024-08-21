# Telegram Channel Scraper

A powerful and flexible Python tool for scraping public Telegram channels.

## Features

- Multi-channel concurrent scraping
- Multiple output formats: JSON, TXT, CSV, Markdown, PDF, HTML, XLSX, DOCX
- Asynchronous processing for improved efficiency
- Customizable configuration options
- Resumable scraping capability
- Detailed logging
- User-friendly command-line interface

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/ding113/Telegram-Channel-Scraper.git
   cd Telegram-Channel-Scraper
   ```

2. Install the required dependencies:
   ```
   pip install -r requirements.txt
   ```

## Usage

1. (Optional) Create a default configuration file:
   ```
   python telegram.py --create-config
   ```
   This will create a `config.yaml` file with default settings.

2. Edit the configuration file to add your desired channels and adjust settings.

3. Run the scraper:
   ```
   python telegram.py
   ```

### Command-line Options

- `-c`, `--config`: Specify the path to the configuration file (default: `config.yaml`)
- `-f`, `--format`: Specify the output format
- `-d`, `--delimiter`: Set a custom delimiter for TXT and CSV outputs
- `--channels`: Directly specify channels to scrape via command line
- `--create-config`: Create a default configuration file

Example:
```
python telegram.py --channels channel1 channel2 -f json
```

## Configuration

The configuration file (`config.yaml` by default) supports the following options:

- `channels`: List of channels to scrape
- `output_format`: Output format
- `start_ids`: Starting message ID for each channel
- `delimiter`: Delimiter for TXT and CSV outputs
- `max_retries`: Maximum number of retries for failed requests
- `retry_delay`: Delay between retries (in seconds)
- `timeout`: Request timeout (in seconds)
- `max_empty_pages`: Maximum number of consecutive empty pages before stopping

## Caution

- This tool is intended for scraping public Telegram channels only.
- Adhere to Telegram's terms of service and relevant laws and regulations.
- Excessive requests may result in temporary IP bans. Use responsibly.

## Contributing

Contributions are welcome! Please feel free to submit issues and pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
