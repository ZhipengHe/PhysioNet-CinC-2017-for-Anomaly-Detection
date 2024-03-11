# PhysioNet/CinC 2017 Dataset for Anomaly Detection

This dataset is a modified version of [PhysioNet/CinC Challenge 2017 dataset](https://physionet.org/content/challenge-2017/1.0.0/), specifically curated for anomaly detection tasks. 

## Original Dataset Information

The original PhysioNet Challenge 2017 dataset is a collection of 8,528 single-lead ECG recordings, lasting from 9 seconds to just over 60 seconds and sampled at 300 Hz. The data profile for the original dataset is as follows:

- Normal (N): 5,076 recordings
- AF (A): 758 recordings
- Other (O): 2,415 recordings
- Noisy (~): 279 recordings

## Dataset Split

The dataset is split into a training set and a testing set. The split is as follows:

- Training Set: Randomly selected 80% of the data from the "normal" category.
- Testing Set: Randomly selected 20% of the data from the "normal" category, as well as 100% of the data from the "af", "noisy", and "other" categories.

The training set is intended to be used for training anomaly detection models, while the testing set is intended to be used for evaluating the performance of the trained models. Only "normal" recordings are treated as normal data, while all other types of recordings are treated as anomalous data.

## File Structure

The dataset is organized in the following file structure:

- `training.csv`: This file contains the index of the .mat and .hea files, as well as the corresponding labels for the training set.
- `testing.csv`: This file contains the index of the .mat and .hea files, as well as the corresponding labels for the testing set.

## Usage

To use this dataset for anomaly detection tasks, you can follow these steps:

1. Download the dataset from [link-to-dataset].
2. Extract the dataset files to a local directory.
3. Load the training and testing data using the provided `training.csv` and `testing.csv` files.
4. Preprocess the data as needed for your anomaly detection algorithm.
5. Train your anomaly detection model using the training data.
6. Evaluate the performance of your model using the testing data.
7. Iterate and refine your model as necessary.

## Citation

If you use this dataset in your research or project, please cite the original PhysioNet Challenge 2017 dataset:

> Clifford GD, Liu C, Moody B, Li-wei HL, Silva I, Li Q, Johnson AE, Mark RG. AF classification from a short single lead ECG recording: The PhysioNet/computing in cardiology challenge 2017. In 2017 Computing in Cardiology (CinC) 2017 Sep 24 (pp. 1-4). IEEE. https://doi.org/10.22489/CinC.2017.065-469

## License

[Open Data Commons Attribution License v1.0](https://physionet.org/content/challenge-2017/view-license/1.0.0/)
Please refer to the license information provided with the original PhysioNet Challenge 2017 dataset.







