# Self-Supervised-Pre-training-for-Skin-Lesion-Classification-under-Limited-Label-Budgets
Investigated Domain-Adapted self-supervised learning (DINO) to address severe label scarcity and extreme class imbalance in clinical skin screening. Using the dataset from Kaggle https://www.kaggle.com/datasets/roscoekerby/isic-2024-permissive-training-input

# **Model Architectures and Pre-Training Frameworks**

* **Domain-Adapted DINO:** A specialized self-supervised learning (SSL) Vision Transformer adapted to learn fine-grained features from unlabelled skin lesion images.
* **Standard DINOv2:** Off-the-shelf self-supervised Vision Transformer trained on large-scale natural internet images.
* **Supervised ViT-S/16:** Standard Vision Transformer baseline pre-trained on ImageNet.
* **ImageNet ResNet-50:** Traditional Convolutional Neural Network (CNN) baseline pre-trained on ImageNet.

# **Evaluation &amp; Methodology Tools**

* **Linear Probing:** Evaluates the quality of frozen visual feature representations by training a linear classifier head.
* **Simulated Label Budgets:** Evaluated performance across 5%, 10%, 25%, and 100% labeled patient partitions.
* **Paired Bootstrap Testing:** Used for statistical validation of performance differences across model variants.

# **Explainability &amp; Diagnostic Tools**

* **Grad-CAM Overlays:** Used to generate visual attention heatmaps to evaluate whether model focus aligns with physical lesion micro-textures.

### **Dataset**

**SLICE-3D Permissive ISIC 2024 Dataset:** Official ISIC 2024 challenge dataset hosted on Kaggle, consisting of 3D total body photography lesion crops.
