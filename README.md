# knifeguard-bot_telegram
KnifeGuard Bot: AI-powered weapon detection system for customs control. Uses computer vision to identify 4 combat knife types in X-ray scans with 85% accuracy and progressive metric stabilization.
This Telegram bot uses a state-of-the-art YOLOv8 model to identify four types of combat knives in X-ray images from inspection systems. It's designed for customs control to detect dangerous objects without physical inspection.
![image](https://github.com/user-attachments/assets/42f2077c-f4f8-4e32-8a00-c264fcc509cc)
Key Features
Real-time detection of four combat knife types:
Army knives
Hunting knives
Sabers
Folding knives
High accuracy with precision up to 85%
User-friendly interface with interactive menu
Fast processing - results in seconds
Customizable confidence threshold

Performance Metrics 📊
Metric	Value	Description
Precision	0.8	Accuracy of positive identifications
Recall	0.7	Ability to find all relevant instances
mAP@0.5	0.776	Mean Average Precision at 0.5 IoU
mAP50-95	0.65	Mean AP across IoU thresholds 0.5-0.95

Installation and Setup ⚙️
Prerequisites
Python 3.8+
Telegram bot token (get from @BotFather)

# Clone repository
git clone https://github.com/yourusername/combat-knife-detection-bot.git
cd combat-knife-detection-bot

# Install dependencies
pip install -r requirements.txt

# Install additional dependencies
pip install python-telegram-bot --upgrade
pip install ultralytics


Configuration
Place your trained YOLOv8 model at /content/best.pt
Set your Telegram bot token:

BOT_TOKEN = "YOUR_TELEGRAM_BOT_TOKEN"

python knife_detection_bot.py

Usage Guide 📱
Start the bot with /start command
Send an X-ray image from inspection systems
Receive detection results within seconds

Bot Commands:
/start - Initialize the bot
/help - Get usage instructions
/about - Learn about the bot's capabilities
/settings - View current configuration

