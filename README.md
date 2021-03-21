# Mask Detection Monitor

![GitHub repo size](https://img.shields.io/github/repo-size/zeyad-mansour/mask-detection-monitor)
![GitHub contributors](https://img.shields.io/github/contributors/zeyad-mansour/mask-detection-monitor)

Provided video or image input, this tool uses a [YOLOv5](https://github.com/ultralytics/yolov5) model trained to detect the status of medical mask wearers, and based on that, it calculates a score. This score can be used to determine when to send alerts given a threshold. The hack also provides a graph of the mask wearers over time.

## Demo

This project has been integrated into a web application found [here](https://www.zeyadmansour.com/sdm/). This is hosted using Apache on an Ubuntu system.
![demo_image](demo_test.png)

## Prerequisites

* You have installed a 64-bit release of [Python](https://www.python.org/downloads/) 3.7 or above

## Installing SDM

1. Clone this repository.

2. Navigate to the root of the project folder via the CLI. Use the package manager [pip](https://pip.pypa.io/en/stable/) to install the necessary dependencies.
```
pip3 install -r requirements.txt
```  

## Using SDM

Navigate to the root of the project folder via the CLI. Make sure to specify the SOURCE.
* Image or video: SOURCE is the path to that file (relative to the root folder)
	* This is the purpose of the [input_data](input_data) folder.
* Webcam: Provide no additional arguments
* HTTP/RTSP stream: SOURCE is the link

```
python SDM.py "SOURCE"
```
(Ensure that the default interpreter for the "python" command is version 3.7 or above)
## Contributors

This project was created in contribution with:

* [@0xmmalik](https://github.com/0xmmalik) 📖

## Notes

This project was created as part of [OSU's 2021 HS hackathon](https://hack.osu.edu/hs/2021/).

## License

This project uses the following license: [MIT](https://github.com/zeyad-mansour/social-distancing-monitor/blob/main/LICENSE)
