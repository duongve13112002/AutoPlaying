# AutoPlay Game with python

## Overview

This repository contains code for an AutoPlay Game project using AlexNet. The project focuses on automating gameplay in the popular game Grand Theft Auto: San Andreas (GTA SAN) by predicting the optimal actions based on the screen information.

## Features

- **AlexNet:** The core of the project is a deep learning model trained to analyze the game screen and make decisions on player actions.

- **Screen Analysis:** The model processes real-time screenshots from the game to understand the current state, identify objects, and determine the next action.

- **Game Interaction:** The implementation includes scripts to interact with the game, sending commands to control the player character based on the predictions of the deep learning model.

- **Customization:** Users can customize the model, training data, and game interactions to adapt the system to their specific gameplay style.

## Video Demo

For a visual representation of the project in action, check out the [Video Demo](https://drive.google.com/file/d/1c0I4HnZ23pf9E7TkXGzzJUXH669avizz/view?usp=sharing).

## Getting Started

### Prerequisites

- Install the required dependencies listed in `requirements.txt`.
- Ensure you have the game (GTA SAN) installed on your system.

### Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/duongve13112002/AutoPlaying.git
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Training the Model

The repository includes tools and scripts for training your own deep learning model based on your gameplay data. Follow these steps to train the model:

1. Open the game from which you want to collect data (ensure the game is in "Windowed mode").

2. Navigate to the directory containing the file named "Collect_data.py".

3. Run the command "python Collect_data.py" and press enter to start collecting data.

4. Control the game (note: Caps Lock must be enabled). (To temporarily pause data collection, press the 'T' key, and to end the data collection process, press the 'E' key.)

5. After collecting the data, go to the "data" directory and run the "balance_data.py" file to balance the data (Perform this process for as many files or training samples as you desire. Recommending a minimum of 100,000 samples after balancing, but the greater the number, the better).

6. Finally, run the "train_model.py" file to train the model.

## Running program

To make Python play a game (note: a model must be available), follow these steps:

1. Open the game (Do not "run as administrator" for the application; the game must be in "Windowed mode," and the Caps Lock key must be enabled)

2. Navigate to the directory containing the file named "test_model.py."

3. Run the command "python test_model.py" to let the model play the game. (To temporarily pause the model, press the 'T' key, and to end the model's execution, press the 'E' key).


## Contributing

Contributions are welcome! If you have ideas for improvements, new features, or bug fixes, please open an issue or submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- Special thanks to [Rockstar Games](https://www.rockstargames.com/) the creators of GTA SAN and the [TFLearn libraries](https://github.com/tflearn/tflearn) used in this project.

Happy Auto-Playing! 🎮🚗


