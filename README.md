# Vision_Transformer
Source: 

[AN IMAGE IS WORTH 16X16 WORDS: TRANSFORMERS FOR IMAGE RECOGNITION AT SCALE](https://arxiv.org/pdf/2010.11929.pdf)

[Attention Is All You Need](https://arxiv.org/pdf/1706.03762.pdf)

[Visual-Transformers-a-new-computer-vision-paradigm](https://medium.com/swlh/visual-transformers-a-new-computer-vision-paradigm-aa78c2a2ccf2)

####  Step 1: Split the image into fixed-size patches. 
#### Step 2:Flatten the 2D image patches to 1D patch embedding and linearly embed them using a fully connected layer. Positional embeddings are added to the patch embeddings to retain positional information.
#### Step 3: A special classification token(CLS) is added to positional encoding, and the positional encoding is summed. The positional patch encoded vectors will be passed as an input to the Transformer Encoder.
#### Step 4: Transformer Encoder has alternating layers of multiheaded self-attention and MLP blocks. Layernorm (LN) is applied before the self-attention block, and the MLP block and the residual connections are applied after every block.
#### Step 5: A classification head is implemented using MLP with one hidden layer at pre-training time and a single linear layer for fine-tuning for image classification.
![alt text](https://github.com/arshren/Vision_Transformer/blob/main/ViT.JPG)
