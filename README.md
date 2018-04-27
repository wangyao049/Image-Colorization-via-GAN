  # Image-Colorization-via-GAN
## This is the implement of IPIU paper "Gray-scale Image Colorization using Generative Adversarial Networks"
The paper can be download [here](https://www.eiric.or.kr/community/post2_cseric.php?m=view&gubun=201802&num=13852&pg=24&seGubun=6&seGubun1=&SnxGubun=%C6%F7%BD%BA%C5%CD&searchBy=&searchWord=)

## Prerequisites
1. python 3.5
2. tensorflow 1.0.0

## Getting Start

### Training
'''
python colorization.py \
  --mode train \
  --input_dir manga/train \
  --output_dir manga_train \
  --max_epochs 200 \
  --lab_colorization
'''

### Test
'''
python colorization.py \
  --mode test \
  --input_dir manga/test \
  --output_dir manga_test \
  --checkpoint manga_train
'''

## Note
This code is heavily rely on [pix2pix](https://arxiv.org/pdf/1611.07004v1.pdf)
The tensorflow implement can be found [here](https://phillipi.github.io/pix2pix/)
