# COCO-Image-Captioning

### Training
1. Learning Rate (starting): 0.001
- Step-wise warm-up scheduler with gamma=1.2 for the first 10 epochs to gradually raise the learning rate per 3 epochs.
- Afterwards, employed step-wise learning rate decay scheduler with gamma=1.8 and step size of 3
2. Embedding size: 512
3. Dropout rate: 0.65
4. Batch size: 64
5. Optimizer: AdamW
  
<img width="757" alt="Screenshot 2025-04-03 at 9 56 47 PM" src="https://github.com/user-attachments/assets/f08becc9-72d9-4263-ac5a-34be66a0e2ee" />

### Architecture
- Resnet50 was used as a frozen image encoder

<img src="https://github.com/user-attachments/assets/d9f3654a-f2d4-4989-abd2-27b815c66269" width="600" height="200">
<img width="480" alt="Screenshot 2025-04-03 at 10 00 19 PM" src="https://github.com/user-attachments/assets/f49d3e8f-26c4-48be-8246-930c397341a8" width="450" height="275"/>

### Results
Loss: 2.68
Perplexity: 14.75

**Inference**

The example denotes example outputs using beam search on the test dataset.

<img width="563" alt="Screenshot 2025-04-03 at 9 51 46 PM" src="https://github.com/user-attachments/assets/a9f27c7c-35d9-4ae1-b8b1-3a4ab930f8c6" width="800" height="680"/>
