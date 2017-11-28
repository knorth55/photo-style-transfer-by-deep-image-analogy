# Photo Style Transfer by Deep Image Analogy

I run photo style transfer by [Deep Image Analogy](https://github.com/msracver/Deep-Image-Analogy).

## Requirement

- Caffe

## Results

| A (input) | AB (output) | BA (output) | B (input) |
|:---------:|:-----------:|:-----------:|:---------:|
|![0_A](./images/0/A.png) | ![0_AB](./images/0/resultAB.png) | ![0_BA](./images/0/resultBA.png) | ![0_B](./images/0/B.png) |
|![1_A](./images/1/A.png) | ![1_AB](./images/1/resultAB.png) | ![1_BA](./images/1/resultBA.png) | ![1_B](./images/1/B.png) |
|![2_A](./images/2/A.png) | ![2_AB](./images/2/resultAB.png) | ![2_BA](./images/2/resultBA.png) | ![2_B](./images/2/B.png) |
|![3_A](./images/3/A.png) | ![3_AB](./images/3/resultAB.png) | ![3_BA](./images/3/resultBA.png) | ![3_B](./images/3/B.png) |

## Try it by yourself

### How to Install

```bash
git clone https://github.com/msracver/Deep-Image-Analogy.git
cd Deep-Image-Analogy/
git checkout linux
sh scripts/config_deep_image_analogy.sh

# modify Makefile.config.example
ln -sf Makefile.config.example Makefile.config
make all
sh scripts/make_deep_image_analogy.sh
```

### How to Run

```bash
export LD_LIBRARY_PATH="./build/lib" 
./demo deep_image_analogy/models/ /path/to/img/A.png /path/to/img/B.png /path/to/output/dir/ 0 0.5 2 0
```