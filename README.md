# Cable Damage Datasets

A curated collection of open-source datasets, codebases, and resources for training and evaluating AI models in faulty wire detection, cable damage classification, and industrial anomaly detection.

This repository serves as a centralized inventory for researchers, engineers, and computer vision practitioners working on electrical component defect detection.

---

## Curated Resources

| # | Resource Name | Source | Type | Description |
|---|---------------|--------|------|-------------|
| 1 | Stripped Wire Dataset | [Zenodo](https://zenodo.org/records/16686806) | Image Dataset | Academic dataset containing images of electrical wires with 4 diameters. Includes train/test splits with classes: Good, Pulled strands, and Cut strands. Ideal for PatchCore and VLM anomaly detection. |
| 2 | Faulty-Wire-Detection-AI | [GitHub](https://github.com/cjdevx-ai/Faulty-Wire-Detection-AI) | Codebase / Model | A dedicated AI implementation repository for detecting faulty wires. Useful for referencing model architectures, training pipelines, or inference scripts. |
| 3 | Cable Damage Dataset | [Hugging Face](https://huggingface.co/datasets/Francesco/cable-damage) | ML Dataset | A community-uploaded dataset on Hugging Face formatted for easy integration with modern machine learning libraries (e.g., datasets, transformers). |
| 4 | Cable Damage (Roboflow 100) | [Roboflow](https://universe.roboflow.com/roboflow100vl-full/cable-damage-z5nlo-epij) | Annotated Dataset | Pre-annotated computer vision dataset hosted on Roboflow. Includes bounding boxes/masks and supports easy export to YOLO, COCO, or TensorFlow formats. |

---

## Target Defect Taxonomy

Based on the curated resources, this collection supports the detection of the following defect types:

- **Cut / Severed Strands**: Visible physical breaks in the wire conductor.
- **Pulled / Frayed Strands**: Partially detached or displaced conductor strands.
- **General Cable Damage**: Insulation tears, crushing, or deformation.

---

## How to Use This Repository

1. **For Data Collection**: Start with the Roboflow or Hugging Face datasets for quick prototyping, as they are pre-formatted for popular machine learning frameworks.
2. **For Academic and Research Rigor**: Use the Zenodo Stripped Wire Dataset, which provides controlled, well-documented train/test splits specifically designed for anomaly detection benchmarks.
3. **For Implementation**: Reference the Faulty-Wire-Detection-AI repository for ready-made training scripts and model architectures.

---

## Quick Start Example

Load the Hugging Face cable damage dataset in just three lines of Python:

```python
from datasets import load_dataset

dataset = load_dataset("Francesco/cable-damage")
print(dataset["train"][0])
```

---

## Citation

If you find this curated list useful in your research, project, or publication, please consider citing this repository:

```bibtex
@misc{jha2026cabledamage,
  author = {Murli Jha},
  title = {Cable Damage Datasets: A Curated Collection},
  year = {2026},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/murlijha2025/cable-damage-datasets}},
  url = {https://github.com/murlijha2025/cable-damage-datasets}
}
```

---

## Contributing

Have another dataset, paper, or codebase related to wire or cable defect detection? 

Please open an Issue or submit a Pull Request to add it to this list. When submitting, please include:
- The name of the resource
- The source link
- A brief description of its contents, format, and license (if known)

Last Updated: July 2026
