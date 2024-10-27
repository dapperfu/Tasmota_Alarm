# Tasmota_Alarm
Alarm clock that slowly brightens a dimmable light bulb. Run in cron.

All scripts were written by AI. ChatGPT 4o and [Ollama codegemma](https://ollama.com/library/codegemma).

Per ChatGPT: 

Here's a concise "How to Use" section for a GitHub README that covers both the first and the most recent script versions.

---

## How to Use

### Requirements
Make sure you have the following dependencies installed:
```bash
pip install requests click
```

### 1. First Script - Gradual Wakeup Light (Cool to Warm Transition)
This script gradually increases the brightness of a Tasmota-controlled light bulb over a specified period, starting from cool white and transitioning to warm white when brightness reaches 75%.

#### Running the Script
1. Clone the repository and navigate to the directory containing the script.
2. Run the script using the following command:
   ```bash
   python wakeup_light.py --ip-address <YOUR_TASMOTA_IP> --duration <DURATION_IN_MINUTES>
   ```
   - Replace `<YOUR_TASMOTA_IP>` with the IP address of your Tasmota device.
   - Replace `<DURATION_IN_MINUTES>` with the desired wakeup duration (default is 30 minutes).

#### Example
```bash
python wakeup_light.py --ip-address 192.168.1.100 --duration 20
```
This command will gradually increase the brightness over 20 minutes, starting with a cool white color and smoothly transitioning to warm white as the brightness approaches 100%.

### 2. Latest Script - Gradual Wakeup Light (Warm to Cool Transition)
This version of the script has been updated to start with warm white and transitions to cool white when brightness reaches 75%.

#### Running the Script
1. Clone the repository and navigate to the directory containing the latest script.
2. Run the script using the following command:
   ```bash
   python wakeup_light.py --ip-address <YOUR_TASMOTA_IP> --duration <DURATION_IN_MINUTES>
   ```
   - Replace `<YOUR_TASMOTA_IP>` with the IP address of your Tasmota device.
   - Replace `<DURATION_IN_MINUTES>` with the desired wakeup duration (default is 30 minutes).

#### Example
```bash
python wakeup_light.py --ip-address 192.168.1.100 --duration 20
```
This command will gradually increase the brightness over 20 minutes, starting with a warm white color and smoothly transitioning to cool white as the brightness approaches 100%.

### Notes
- Ensure your Tasmota device is accessible via the network and the correct IP address is provided.
- The scripts use a gradual step-based increase in brightness to ensure a smooth wake-up experience.

--- 

These sections provide clear instructions on how to install dependencies, run each version of the script, and examples of usage, making it easy for anyone to get started.
