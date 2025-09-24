# AnimeGAN

AnimeGAN is a deep learning project that transforms real-world images into anime-style artworks using Generative Adversarial Networks (GANs). This repository provides an implementation of the AnimeGAN architecture, which is designed for high-quality, real-time photo-to-anime translation.

## Features

- Converts real photos to anime-style images
- Pre-trained models for quick inference
- Supports training on custom datasets
- Efficient and lightweight architecture for fast inference

## Demo

| Real Image | AnimeGAN Output |
|------------|----------------|
| ![real](examples/real.jpg) | ![anime](examples/anime.jpg) |

*Replace with your own sample images in the `examples/` directory.*

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yashgupta0410/AnimeGAN.git
   cd AnimeGAN
   ```

2. **Install dependencies:**
   ```bash
   pip install -r requirements.txt
   ```
   > Note: This project requires Python 3.6 or higher.

## Usage

### 1. Inference

To convert an image to anime style:

```bash
python infer.py --input path/to/your/image.jpg --output path/to/save/anime.jpg --checkpoint path/to/model_checkpoint
```

- `--input`: Path to the input image
- `--output`: Path to save the output anime image
- `--checkpoint`: Path to the pre-trained model checkpoint

### 2. Training

To train on your own dataset:

```bash
python train.py --dataset path/to/dataset --epochs 100 --batch_size 8
```

- `--dataset`: Path to your training dataset
- `--epochs`: Number of training epochs
- `--batch_size`: Batch size for training

> See `train.py` for more training options.

## Model Weights

Pre-trained model weights can be downloaded from the [Releases](https://github.com/yashgupta0410/AnimeGAN/releases) page (if available), or you can train your own model.

## Project Structure

```
AnimeGAN/
├── checkpoints/         # Model weights
├── datasets/            # Training datasets
├── examples/            # Example images
├── models/              # Model architecture files
├── infer.py             # Inference script
├── train.py             # Training script
├── requirements.txt     # Python dependencies
└── README.md
```

## Acknowledgements

- [AnimeGAN](https://github.com/TachibanaYoshino/AnimeGAN) by TachibanaYoshino
- TensorFlow & PyTorch communities

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.

---

*Feel free to contribute! Pull requests, issues, and suggestions are welcome.*
