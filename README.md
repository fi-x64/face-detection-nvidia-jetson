# Face Detection using Multi-task Cascaded Convolutional Networks (MTCNN)

Multi-task Cascaded Convolutional Networks (MTCNN) is a deep learning-based framework for detecting faces and facial landmarks. It uses a three-stage cascaded structure:

1. P-Net (Proposal Network): Generates initial face candidates using a sliding window and removes overlaps with Non-Maximum Suppression (NMS).

2. R-Net (Refinement Network): Refines P-Net’s output by filtering out false positives and adjusting bounding boxes.

3. O-Net (Output Network): Makes the final face detections and accurately localizes five facial landmarks (eyes, nose, mouth corners).

## Key Features

1. Multi-task Learning: Detects faces and landmarks simultaneously.
2. Cascaded Architecture: Increases detection precision through progressive refinement.
3. Applications: Face recognition, security, and AR/VR face tracking.

## Build with 2 environments

We will have 2 environments for comparing speed and accuracy

### With "fd-use-lib.ipynb" we will use "req-lib.txt" requirement file.

This is the build which we will use libraries for handling with a bit of delay and lag

#### Create Env

```
    python -m venv venv
```

#### Setup environment

```
    venv\Scripts\activate
    pip install -r req.txt -q
```

#### run fd-use-lib.ipynb

- Select the Kernal
- Choose "venv" environment
- Run all

### With "fd-from-scraft.ipynb" we will use "req-scraft.txt" requirement file.

#### Create Env

```
    python -m venv venv1
```

#### Setup environment

```
    venv1\Scripts\activate
    pip install -r req1.txt -q
```

#### run fd-use-lib.ipynb

- Select the Kernal
- Choose "venv1" environment
- Run all

## Future Improvement

1. Optimize the model with TensorRT, ONNX, or model pruning for faster real-time applications.
2. Train with multi-scale images to improve face detection across various resolutions.
3. Use better Non-Maximum Suppression (NMS) techniques like Soft-NMS for reducing false positives.

## Reference

1. https://github.com/timesler/facenet-pytorch
2. https://www.kaggle.com/code/timesler/guide-to-mtcnn-in-facenet-pytorch
