# AI-Sudoku-Solver
## Installation

1. Download and install Python3 from [here](https://www.python.org/downloads/)
2. I recommend using [virtualenv](https://virtualenv.pypa.io/en/latest/). Download virtualenv by opening a terminal and typing:
    ```bash
    pip install virtualenv
    ```
3. Create a virtual environment with the name sudokuenv.

   * Windows
   ```bash
   virtualenv sudokuenv
   cd sudokuenv/Scripts
   activate
   ```
   * Linux:
   ```bash
   source sudokuenv/bin/activate
    ```
4. Clone this repository, extract it if you downloaded a .zip or .tar file and cd into the cloned repository.

    * For Example:
    ```bash
    cd A:\AI_Sudoku-master
    ```
5. Install the required packages by typing:
   ```bash
   pip install -r requirements.txt
   ```
## Usage
* Before running the application, know that you can set the **modeltype** variable in **Run.py** to either "CNN" or "KNN" to choose the Convolutional Neural Network or the K Nearest Neighbours Algorithm for Recognition. By default it is set to "KNN" and I got a way higher accuracy using KNN itself, so I would recommend that you don't change it.
    ```Python
    '''Run this file to run the application'''
    from MainUI import MainUI
    from CNN import CNN
    from KNN import KNN
    import os
    # Change the model type variable value to "CNN" to use the Convolutional Neural Network
    # Change the model type variable value to "KNN" to use the K Nearest Neighbours Classifier
    modeltype = "KNN"
    ```
* Type the below command to run the Application. You *need* to be connected to the Internet and it might take 5-10 minutes to create the **knn.sav** file so please wait patiently. This delay is only during the first run as once created, the application will use the local file
    ```bash
    python Run.py
    ```
