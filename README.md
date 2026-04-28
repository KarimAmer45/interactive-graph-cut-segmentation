# Interactive Graph Cut Segmentation

Interactive foreground/background segmentation with scribbles, histogram and Gaussian-mixture color models, graph cuts, and dataset-level evaluation.

## Highlights

- Uses user scribbles to build foreground and background color models.
- Supports histogram and GMM unary terms.
- Optimizes binary labels with graph cuts and pairwise smoothness.
- Includes an OpenCV interaction loop with undo, save, and optional IoU scoring.
- Ships sample inputs, scribbles, ground truth masks, and result figures.

## Repository Layout

- `graphcut_core.py` - color models, graph construction, segmentation, and evaluation.
- `interactive_tool.py` - interactive scribble UI.
- `dataset/` - images, scribbles, masks, and generated segmentation outputs.
- `examples/` - selected visual outputs.

## Setup

```bash
pip install -r requirements.txt
```

## Run

```bash
python graphcut_core.py
python interactive_tool.py dataset/images/scissors.jpg
```

