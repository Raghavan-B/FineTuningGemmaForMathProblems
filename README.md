# Mathematical Problem Solving with Language Models

This project explores the use of fine-tuning a pre-trained language model to solve complex mathematical word problems. The model is trained on mathematical tasks to improve its reasoning abilities and accuracy in answering problems involving arithmetic, algebra, geometry, and more.

## Project Overview

The main goal of this project is to leverage pre-trained language models and fine-tune them for better performance in solving mathematical word problems. We experiment with training the model for 100 epochs and use the Google Colab environment with CPU and TPU hardware acceleration. The project tracks and visualizes various metrics, such as losses and model performance, using **Weights & Biases (wandb)**.

The training utilizes the **Transformers** and **TRL (Transformers Reinforcement Learning)** libraries for efficient training of the model.

### Key Features:
- **Fine-Tuning of Pre-Trained Language Models**: The model is fine-tuned on a math-specific dataset to improve its ability to solve word problems.
- **Tracking with wandb**: All training metrics, including loss and evaluation scores, are captured and visualized using Weights & Biases (wandb).
- **Hardware Optimization**: The training process is conducted in Google Colab using both CPU and TPU for hardware acceleration, which significantly improves training time.
- **Mathematical Reasoning**: The model is specifically fine-tuned for numerical reasoning tasks, such as solving algebraic and arithmetic problems.

## Model Training Details

- **Epochs**: 100 epochs for fine-tuning
- **Hardware**: Google Colab free-tier, utilizing CPU and TPU
- **Libraries**:
  - `transformers`: For pre-trained models and fine-tuning
  - `trl`: For reinforcement learning and training strategies
  - `wandb`: For tracking model metrics (loss, performance, etc.)
  
The model was trained for a limited number of epochs due to hardware constraints, and while it shows improvement in mathematical problem-solving abilities, there is room for further optimization and exploration.

## Results and Discussion

After fine-tuning, the model demonstrated slightly improved performance in reasoning tasks related to mathematical problems. However, it still has limitations, primarily because it was trained for only 100 epochs due to hardware constraints. There is room for further improvements, such as:

- **Longer Training**: Training for more epochs would likely improve the model’s performance.
- **Exploration of Advanced Fine-Tuning Techniques**: Methods like **Reinforcement Learning from Human Feedback (RLHF)** could be explored to enhance reasoning capabilities further.
- **Training from Scratch**: It is hypothesized that training a model from scratch on a dataset specifically designed for solving mathematical problems would yield even better results compared to fine-tuning a pre-trained model.

## Future Work

1. **Extended Training**: Training the model for a larger number of epochs or using a more powerful hardware setup could improve its performance.
2. **Exploration of RLHF**: Reinforcement Learning with Human Feedback could be used to further fine-tune the model for more complex reasoning tasks.
3. **Math-Specific Pretraining**: Creating a custom pre-trained model, specifically designed for solving math problems, could lead to better overall performance.

---

**Note:** The code for training, evaluation, and other processes can be found in the corresponding Google Colab notebook.
