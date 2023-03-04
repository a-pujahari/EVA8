# EVA8 Session 10 Assignment

## The Dawn of Transformers Part 2

### Goals:
1. Rewrite ViT code using convolutions rather than Linear layers
2. Add class token and use class token position to predict classes for CIFAR 10 Dataset
3. Train rewritten model and provide results

### Observations:
1. ViT using convolutions is a hybrid of the ConvMixer architecture (Patches are all you need) and the Vision Transformer architecture
2. Changes have to made within the network to process 4 dimensional tensors (b, c, h, w) as opposed to 3 dimensional tensors (b, n, d) in the original ViT architecture
3. The transformer stack in the ViT implementation provided seems to be incorrect - it does not stack multiple layers in the depth provided

