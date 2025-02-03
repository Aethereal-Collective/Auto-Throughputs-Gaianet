# Auto-Throughputs-Gaianet

## Overview
Auto-Throughputs-Gaianet is a script designed to send automated Throughputs the Gaianet API using multiple threads. It continuously processes user messages and interacts with the API to retrieve responses.

## Installation
To get started, clone this repository and navigate to the project directory:

```sh
git clone https://github.com/Aethereal-Collective/Auto-Throughputs-Gaianet
cd Auto-Throughputs-Gaianet
```

## Setup
1. **Edit `api.txt`**
   - Open a terminal and run:
     ```sh
     nano api.txt
     ```
   - Add the following details:
     - **First line:** API Key (Obtain from [Gaianet Settings](https://www.gaianet.ai/setting))
     - **Second line:** API URL (Navigate to [Gaianet Chat](https://www.gaianet.ai/chat?domain) and select your domain)
   - Click on **API Tutorial** at the bottom of the "Go to Chat" screen.
   - Copy `/v1/chat/completions`.
   - Copy the API key and replace it in `api.txt`.

2. **Create a virtual environment & Create screen**
   ```sh
   screen -S auto-gaianet
   python3 -m venv venv
   source venv/bin/activate
   ```
3. **Install dependencies:**
   ```sh
   pip install -r requirements.txt
   ```

## Usage
Run the script with:
```sh
python3 auto-throughputs-gaianet.py
```

You will be prompted to specify the number of threads to use. The script will then begin processing requests automatically.

## License
This project is open-source and available under the MIT License.

