```
python tools/train.py projects/configs/maptr/maptr_nano_r18_110e.py



bash tools/train.sh ./projects/configs/maptr/maptr_tiny_r50_24e.py

bash tools/test.sh work_dirs/maptr_tiny_r50_24e/maptr_tiny_r50_24e.py work_dirs/maptr_tiny_r50_24e/epoch_12.pth

python tools/maptr/vis_pred.py work_dirs/maptr_tiny_r50_24e/maptr_tiny_r50_24e.py work_dirs/maptr_tiny_r50_24e/epoch_12.pth
```