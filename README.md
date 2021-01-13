# self supervised learning試す

データ: kaggleのキャッサバコンペ

https://www.kaggle.com/c/cassava-leaf-disease-classification

<br>

## 試した手法
### SwAV 

Backborn Model: ResNet50

Self Supervised Training

- https://www.kaggle.com/anonamename/swav-tf

Supervised Training

- 実行環境: windows10, poetry ([pyproject.toml](env/tfgpu/pyproject.toml))
- 

### BYOL

Backborn Model: SeResNeXT50_32x4d

Self Supervised Training

- 実行環境: windows10, anaconda ([lightning.yml](env/lightning.yml))

- ①画像サイズ224*224: [byol-pytorch_seresnext50_32x4d.ipynb](BYOL/byol-pytorch_seresnext50_32x4d.ipynb)
- ➁画像サイズ512*512: [byol-pytorch_seresnext50_32x4d_512.ipynb](BYOL/byol-pytorch_seresnext50_32x4d_512.ipynb)

Supervised Training

- 実行環境: windows10, anaconda ([lightning.yml](env/lightning.yml))
- ①のモデル+画像サイズ224*224: [byol-pytorch_seresnext50_32x4d_Supervised_Training_224.ipynb](BYOL/byol-pytorch_seresnext50_32x4d_Supervised_Training_224.ipynb)
- ①のモデル+画像サイズ224*224 + Data Augmentationあり: [byol-pytorch_seresnext50_32x4d_Supervised_Training_224_aug.ipynb](BYOL/byol-pytorch_seresnext50_32x4d_Supervised_Training_224_aug.ipynb)
- ①のモデル+画像サイズ512*512: [byol-pytorch_seresnext50_32x4d_Supervised_Training_512.ipynb](BYOL/byol-pytorch_seresnext50_32x4d_Supervised_Training_512.ipynb)
- ➁のモデル+画像サイズ512*512: [Supervised_Training_512_aug_byol-pytorch_seresnext50_32x4d_512.ipynb](BYOL/Supervised_Training_512_aug_byol-pytorch_seresnext50_32x4d_512.ipynb)



