Example notebooks demonstrating the use of Prophecy for classification and regression models. (MNIST, ACASXU, GTSRB, TaxiNet)

1. Prophecy_Tool_MNIST.ipynb: Demonstrates the use of Prophecy to extract different types of rules for a CNN for MNIST. It also demonstrates the use of the Marabou tool to prove rules and use of attribution to determine input pixels impacting a rule.

2. ACASX_ProphecyTool.ipynb: Demostrates use of Prophecy to extract rules for the ACASXU (Airborne Collision Avoidance System for Unmanned Aircraft) model https://arxiv.org/pdf/2011.05174. Demonstrates use of Marabou to prove the rules.
Presents sketch of the code to perform compositional verification.

3. GTSRB_ProphecyTool.ipynb: Demostrates use of Prophecy to extract rules for a model for GTSRB (German Traffic Sign Recognition Benchmark) https://paperswithcode.com/dataset/gtsrb.

4. KJ_TaxiNet_ProphecyTool.ipynb: Taxinet is a regression model for center-line tracking on airport runways. It takes in images of the runway and produces two outputs; cross-track error (cte) and head error (he). KJ_Taxinet is a smaller model which takes in down-sampled images of the runway.
This notebook demonstrates the application of Prophecy to extract rules satisfying the safety property (|cte| > safety threshold) , (|he| > safety threshold). It also demonstrates the usage of Marabou to prove these rules.
This is a replication of the work published in 	Ismet Burak Kadron, Divya Gopinath, Corina S. Pasareanu, Huafeng Yu:
Case Study: Analysis of Autonomous Center Line Tracking Neural Networks. VSTTE 2021: 104-121.

5. Airfoil_Self_Noise_ProphecyTool.ipynb: Regression model to prediction of acoustic noise generation from airfoil: 
5D input:
Frequency [Hz]
Airfoil angle of attack [deg]
Chord length [m]
Free-stream velocity [m/s]
Suction side displacement thickness [m]
1D output:
Scaled sound pressure level at given frequency [dB]

Extracts rules and uses Marabou to generate proofs.

6. ProphecyTool_with_CLIP.ipynb: Demonstrates application of Prophecy to extract rules using the fingerprints and zero-shot classification labels of a CLIP model trained on the RIVAL-10 dataset.
