# KartSplitter

KartSplitter is an auto-splitter made for Mario Kart 64. It uses a combination of template matching and predictions via a convolutional neural-network to analyze gameplay frame-by-frame and generate splits for LiveSplit.

## Features

**Automatic Starts and Resets:** KartSplitter can determine when a run begins, and also whether a reset has occurred (and then reset the LiveSplit timer).

**Automatic Splits:** Each frame of gameplay is analyzed by being passed through a neural network to determine whether it is after a track has finished. Once the program has detected such a frame with a reasonably high probability (>.90), the program will then automatically handle splitting on LiveSplit.

## Usage

**Python Version:** `3.10.7`

Clone this repository into a folder of your choice:
```
git clone https://github.com/chris-ehmann/KartSplitter
cd KartSplitter
```

Then install the required Python packages:
```
pip install -r requirements.txt
```

You can then simply run the file `mk64as.py` located inside the `kartsplitter` directory:

```
python mk64as.py
```








