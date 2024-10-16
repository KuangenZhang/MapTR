```
python tools/create_data.py nuscenes --root-path ./data/nuscenes --out-dir ./data/nuscenes --extra-tag nuscenes --version v1.0-mini --canbus ./data

python tools/train.py --config projects/configs/maptr/maptr_nano_r18_110e_unit_test.py --deterministic

python tools/maptr/vis_pred.py work_dirs/maptr_nano_r18_110e_unit_test/maptr_nano_r18_110e_unit_test.py work_dirs/maptr_nano_r18_110e_unit_test/epoch_110.pth --score-thresh 0.1


bash tools/train.sh ./projects/configs/maptr/maptr_tiny_r50_24e.py

bash tools/test.sh work_dirs/maptr_tiny_r50_24e/maptr_tiny_r50_24e.py work_dirs/maptr_tiny_r50_24e/epoch_12.pth

python tools/maptr/vis_pred.py work_dirs/maptr_tiny_r50_24e/maptr_tiny_r50_24e.py work_dirs/maptr_tiny_r50_24e/epoch_12.pth
```