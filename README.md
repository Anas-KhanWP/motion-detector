# Motion Detection System (Under Development)

Welcome to the Motion Detection System project on GitHub! This project is currently under development, and we are excited to share its progress with the open-source community.

## Overview

The Motion Detection System is a Python-based project that utilizes computer vision techniques to detect motion within a video stream. It captures video input from a webcam or video file and identifies motion within a predefined square area. When motion is detected, it sends a notification to a Telegram bot.

## Features

- Real-time motion detection within a specified area of interest.
- Adjustable parameters for threshold, square size, and area threshold.
- Integration with Telegram for immediate notifications.

## Project Structure

- **main.py**: The main Python script that handles video capture and motion detection.
- **requirements.txt**: A file listing the necessary Python packages for running the project.
- **LICENSE**: The project's open-source license.

## How It Works

The Motion Detection System captures video from a webcam or video file using the OpenCV library. It defines a square area within the frame and continually checks for motion within this area. If motion is detected, it draws a green rectangle around the moving object and sends a notification to a Telegram bot.

The system employs the following steps:
1. Initialize a video capture object, and define the square area for motion detection.
2. Apply background subtraction to the square area to isolate moving objects.
3. Threshold the resulting mask to identify motion.
4. Find contours in the thresholded image to locate moving objects.
5. If a contour exceeds a specified area threshold, the system reports motion detection.

## Dependencies

This project relies on the following Python libraries:
- OpenCV: For video capture, image processing, and computer vision.
- Requests: For sending notifications to a Telegram bot.

To install these dependencies, refer to the `requirements.txt` file.

## Usage

You can run this project by executing the `main.py` script. Make sure to specify your Telegram bot token and chat ID in the `TELEGRAM_BOT_TOKEN` and `TELEGRAM_CHAT_ID` variables. You can adjust various parameters, such as the square size and area threshold, to fine-tune the motion detection system according to your needs.

## Contribute

We welcome contributions to this project. If you have ideas for improvements, bug fixes, or new features, please feel free to submit pull requests or open issues. We value your input and collaboration.

## License

This project is open-source and available under the [MIT License](LICENSE).

Thank you for your interest in the Motion Detection System project. We look forward to seeing how this system evolves with your help. Happy coding!
