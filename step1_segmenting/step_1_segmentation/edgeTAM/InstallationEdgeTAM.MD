The script for step 1 segmenting is at .\edgeTAM\EdgeTAM\notebooks\wimtest.py

# to do
- to discuss

```bash
git clone https://github.com/facebookresearch/EdgeTAM.git && cd EdgeTAM
cd EdgeTam

conda create -n edgetam python=3.10
conda activate edgetam
```

Make sure you have cuda toolkit 12.8 installed (and an nvidia gpu). Then go here https://pytorch.org/get-started/locally/ and get the appropriate installer

For Wim's machine that is
```bash
pip3 install torch torchvision --index-url https://download.pytorch.org/whl/cu128
pip install timm
```

Then install edgetam from repo
```bash
pip install -e ".[notebooks]"
```

Lets also make sure that you have access to the environment
```bash
pip install ipykernel
python -m ipykernel install --user --name edgetam --display-name "edgeTAM"
```

Then to be sure also download all modesl
go to \EdgeTAM\checkpoints\
and click on the .sh for downloading the model checkpoints



