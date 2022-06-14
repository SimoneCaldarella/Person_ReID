# Person Attribute Recognition (PAR) and Person Re-Identification (Person Re-ID)

This is the final project for the Deep Learning course @UniTN

Press [here](https://github.com/SimoneCaldarella/Person_ReID/blob/main/Report.pdf) to download the report.

Our code is supposed to run on Google Colaboratory.

In order to execute, it needs a folder containing the .zip dataset (or a pickle version of our Dataset object); this
can be modified in the first cell of the notebook using the global variable ORIGIN_DATASET_FOLDER.

In case you want to execute it with our directory structure, please add on your GoogleDrive folder a shortcut to this shared folder:
	https://drive.google.com/drive/folders/1qwLVxlQnF0q-tH_nqCkE-Ha1qvumHQ3p?usp=sharing
and modify the ORIGIN_DATASET_FOLDER accordingly; the dataset is supposed to be in a .zip file called 'dataset.zip'.

To access an experiment's results, firstly define its save path inside the 'Main/Task 1' section of the notebook, 
modifying the variable save_path_parent; by default it is the current time string of the experiment, inside the 'results' folder
of the project directory. Then run the experiment and those will be found at the end of the execution in the specified folder.

Structure:\
drive/MyDrive/\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|\_DeepLearningProject\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|\_results\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|\_<experiment date 2>\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|\_<experiment date 1>\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|\_...\
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;|\_dataset.zip

In the result/FINAL folder can be found our proposal model, with the same output files included in the email.

In order to run experiments with different losses, change the name inside the cell 'Main/Task 1'. Other hyperparameters that can be changed in the 
same way are learning rate, batch size, use of a scheduler, and the gamma parameter for the focal loss.
