# Jet Nano Object Detect  
This project uses a **Jetson Orin Nano** development board running a local Ultralytics YOLO vision model to monitor RTSP camera feeds (driveway and garage). Detection events can trigger **Home Assistant** automations via webhook calls for notifications or script activation.  

## Features  
- RTSP camera detection via YOLOv8  
- Local processing on Jetson Orin Nano  
- Configurable camera sources via JSON file  
- Webhook triggers for Home Assistant notifications and automations  

## Requirements  
- Jetson Orin Nano development board  
- Suitable RTSP-capable IP cameras  
- Python 3.x  
- Required Python packages (see `requirements.txt`)  

## Configuration
```bash
cp `config.example.json` `config.json`  
```  
Edit 'config.json' and replace the placeholder values for the driveway and garage cameras.  

## Usage
python detect.py  

# TODO:  
- Add startup script
- Add systemd service or cron job for automatic startup  
- Add installation instructions and dependency setup
