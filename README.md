# inpainting-editing

Pytorch implementation for image inpainting and editing.

**Path to code:**

```/home/notebook/data/group/gaojianhao/Inpainting_editing```

**Pretrained model:**

```/home/notebook/data/group/gaojianhao/Inpainting_editing/checkpoints/exp_places_new_para_resnet_noRN/latest_net_G.pth```

**Training:**

1. Make the files which contain the paths of images and masks and name them as img.flist and mask.flist.

2. run the command

```python train.py --name inpainting_editing --img_flist img.flist --mask_flist mask.flist```

**Testing:**

*Path:*

```/home/notebook/data/group/gaojianhao/Inpainting_editing/application```

1. Move the pretrained model to the path

2. Set the path of image and mask to be inpainted or edited in Line 31-32 of ```/home/notebook/data/group/gaojianhao/Inpainting_editing/application/apply.py```.

3. Set the path of pretrained model in Line 621 of ```/home/notebook/data/group/gaojianhao/Inpainting_editing/application/networks.py```

4. run ```apply.py```

**Notification:**

The editing interaction function has not been completed yet in Line 66 of ```apply.py```. In the work before, the predict mask is edited manually and then fed back to the network. 

