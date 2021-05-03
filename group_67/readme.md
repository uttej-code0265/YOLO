Data Pre-Processing:

    Nothing to specify here. The VOCDataset function of pre-processing cell, does the pre-processing of data.

Training:

    Specify the respective paths for IMG_DIR, LABEL_DIR and set CONTINUE_TRAINING flag to true if the training is started from a particular checkpoint, false if otherwise.

    In the train_dataset, test_dataset, validation_dataset pass the respective path of .csv files as the first input of the function VOCDataset.

    Specify the path for saving the weights file for best_val, and for each checkpoint and path for graph_metrics.txt which saves the data of number of epochs completed, best map, maps and loss vs epocs .

Generating Plots: ( Loss vs Epocs & MAP's vs Epocs )

    Run the load metrics cell, after training using graph_metrics.txt. This generates two graphs:
    a. Loss vs Epocs
    b. MAP's vs Epocs

Downloading the dataset:

    The datasets (PASCAL VOC 2007 & PASCAL VOC 2012) can be downlaoaded from the download_dataset.ipynb .

Making Predictions:

    In the Validation Cell (final cell), specify the path to the weights file obtained after the training in the variable LOAD_MODEL_FILE. Running the cell generates the outputs on the images in the path specified in IMG_DIR. 
