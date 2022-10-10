![Dataset Preview](docs/img/sx-data.jpg)

# DigiFace-1M Dataset

The DigiFace-1M dataset is a collection of over one million diverse synthetic face images for face recognition.

It was introduced in our paper [DigiFace-1M: 1 Million Digital Face Images for Face Recognition](https://microsoft.github.io/DigiFace1M) and can be used to train deep learning models for facial recognition.

The dataset contains:

- 720K images with 10K identities (72 images per identity). For each identity, 4 different sets of accessories are sampled and 18 images are rendered for each set.
- 500K images with 100K identities (5 images per identity). For each identity, only one set of accessories is sampled.

The DigiFace-1M dataset can be used for **non-commercial** research, and is licensed under the license found in [LICENSE](LICENSE).

## Downloading the Dataset

For convenience the dataset is split into 8 parts which can be downloaded here: 

72 images per identity 
- [P1](https://facesyntheticspubwedata.blob.core.windows.net/wacv-2023/subjects_0-1999_72_imgs.zip)
- [P2](https://facesyntheticspubwedata.blob.core.windows.net/wacv-2023/subjects_2000-3999_72_imgs.zip)
- [P3](https://facesyntheticspubwedata.blob.core.windows.net/wacv-2023/subjects_4000-5999_72_imgs.zip)
- [P4](https://facesyntheticspubwedata.blob.core.windows.net/wacv-2023/subjects_6000-7999_72_imgs.zip)
- [P5](https://facesyntheticspubwedata.blob.core.windows.net/wacv-2023/subjects_8000-9999_72_imgs.zip)

5 images per identity
- [P1](https://facesyntheticspubwedata.blob.core.windows.net/wacv-2023/subjects_100000-133332_5_imgs.zip)
- [P2](https://facesyntheticspubwedata.blob.core.windows.net/wacv-2023/subjects_133333-166665_5_imgs.zip)
- [P3](https://facesyntheticspubwedata.blob.core.windows.net/wacv-2023/subjects_166666-199998_5_imgs.zip)

## Dataset Layout

The DigiFace-1M dataset contains cropped color images in the following layout.

```
subj_id_n
├── 0.png                 # First rendered image of subject subj_id_n
├── 1.png                 # Second rendered image of subject subj_id_n
...
├── k.png                 # k+1 rendered image of subject subj_id_n
```

## Disclaimer

Some of our rendered faces may be close in appearance to the faces of real people.
Any such similarity is naturally unintentional, as it would be in a dataset of real images, where people may appear similar to others unknown to them.

## Citation

If you use the DigiFace-1M dataset in your work, please cite the following [paper](https://github.com/microsoft/DigiFace1M/raw/main/paper.pdf):

```
@inproceedings{bae2023digiface1m,
  title={DigiFace-1M: 1 Million Digital Face Images for Face Recognition},
  author={Bae, Gwangbin and de La Gorce, Martin and Baltru{\v{s}}aitis, Tadas and Hewitt, Charlie and Chen, Dong and Valentin, Julien and Cipolla, Roberto and Shen, Jingjing},
  booktitle={2023 IEEE Winter Conference on Applications of Computer Vision (WACV)},
  year={2023},
  organization={IEEE}
}
```
