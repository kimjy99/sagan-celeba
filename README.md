SAGAN (Self Attention GAN) with CelebA dataset
=============

## Model
### Generator:  
> 1x1x(nz) → 4x4x1024 → 8x8x512 → 16x16x256 → 16x16x256 (Self Attention) → 32x32x128 → 32x32x128 (Self Attention) → 64x64x3
  
### Discriminator:  
> 64x64x3 → 32x32x64 → 16x16x128 → 8x8x256 → 8x8x256 (Self Attention) → 4x4x512 → 4x4x512(Self Attention) → 1x1x1

### Gan Loss:  
> Wasserstein hinge loss

### Additional Techniques:
> Spectral Nomalization for both generator and discriminator
  
------------------
## Output Images  
![output_img](./images/output.png)  

------------------
## Loss  
![loss_img](./images/losses.png)  

------------------
## How generator improved
![train_gif](./images/train.gif)  

------------------
## Find latent vectors for real images  
![latent_img](./images/latent.png)  
  
## Linearly mapping images  
![mapping_img](./images/mapping.png)    
![test_gif](./images/test-several.gif)   
