# -Precision-Recovery-HEP-Inspired-Data-
Working of the Project 
	1.	Problem Identification
Scientific and experimental pipelines often apply compression and face noise during storage or transmission, which leads to loss of numerical precision in floating-point data.

	2.	Synthetic Data Generation
Generated synthetic floating-point values to simulate continuous scientific measurements while keeping full control over ground-truth data.

	3.	Compression Simulation
Applied compression and decompression to the data to intentionally introduce precision degradation, mimicking real-world data handling pipelines.

	4.	Noise Injection
Added controlled Gaussian noise to the decompressed data to replicate sensor errors, transmission noise, and rounding inaccuracies.

	5.	Input–Target Preparation
Used the noisy and degraded data as input, and the original clean data as the target output for training.

	6.	Autoencoder Design
Built a lightweight autoencoder neural network consisting of an encoder for learning compact representations and a decoder for reconstructing the original signal.

	7.	Model Training
Trained the autoencoder using Mean Squared Error (MSE) loss so that the model learns to minimize reconstruction error between recovered and original data.

	8.	Reconstruction (Inference)
Passed noisy inputs through the trained model to obtain recovered numerical values.

	9.	Quantitative Evaluation
Measured reconstruction quality using Mean Squared Error (MSE) to numerically verify precision recovery.

	10.	Visual Validation
Compared Original vs Noisy and Original vs Recovered plots to visually confirm the effectiveness of the model.

	11.	Result Interpretation
Observed significantly reduced error and improved alignment between original and recovered data, confirming that the autoencoder successfully learned noise-robust representations.
