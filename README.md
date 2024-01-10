## Example Script

### Full Dataset

**Training:** 
```
CUDA_VISIBLE_DEVICES=0,1 python main.py --config configs/ego-video-foundation-big.yml --data_path /home/mr6744/SAYCAM_200K_deblur_crop --data_val_path /home/mr6744/SAYCAM_val --exp ego-video-foundation-bigger-model
```

**Sampling:**
```
CUDA_VISIBLE_DEVICES=2 python main.py --config configs/ego-video-foundation-big-sample.yml --data_path /home/mr6744/SAYCAM_200K_deblur_crop --data_val_path /home/mr6744/SAYCAM_val --exp ego-video-foundation-bigger-model-sample --resume_training
```


### Small Dataset (9 frames)

**Training:** 
```
CUDA_VISIBLE_DEVICES=2 python main.py --config configs/ego-video-foundation-big-overfit.yml --data_path /home/mr6744/SAYCAM_9_deblur_crop --data_val_path /home/mr6744/SAYCAM_9_deblur_crop --exp ego-video-foundation-bigger-model-9-samples
```

**Sampling:** 
```
CUDA_VISIBLE_DEVICES=2 python main.py --config configs/ego-video-foundation-big-overfit-sample.yml --data_path /home/mr6744/SAYCAM_9_deblur_crop --data_val_path /home/mr6744/SAYCAM_9_deblur_crop --exp ego-video-foundation-bigger-model-9-samples-sample
```