# MTMC Dataset
- [The MTA Dataset](https://github.com/schuar-iosb/mta-dataset)
  - The MTA (Multi Camera Track Auto) is a large multi target multi camera tracking dataset.
  - Over 2800 person identities, 6 cameras and a video length of over 100 minutes per camera.
  - Day and night period.
  - [Reference](https://openaccess.thecvf.com/content_CVPRW_2020/papers/w70/Kohl_The_MTA_Dataset_for_Multi-Target_Multi-Camera_Pedestrian_Tracking_by_Weighted_CVPRW_2020_paper.pdf)
- [Omni-MOT Dataset](https://github.com/shijieS/OmniMOTDataset)
  - A dataset generated from [CARLA Simulator](http://carla.org/)
  - Objects: Cars
  - [Reference](https://arxiv.org/pdf/2008.08826.pdf)
- [MOT Challenge](https://motchallenge.net)

# MOT Benchmark
- [UA-DETRAC Benchmark Suite](http://detrac-db.rit.albany.edu)
- [KITTI Vision Benchmark Suite](http://www.cvlibs.net/datasets/kitti/eval_tracking.php)


# Metrics for MOT
- **Multiple Object Tracking Accuracy (MOTA):** MOTA is a commonly used evaluation metric for multiple object tracking. It penalizes the sum of missed boxes, false positive boxes, and identity switches divided by the number of ground truth boxes. We report percentage MOTA for evaluation.

<p align="center">
  <img src="https://latex.codecogs.com/svg.latex?MOTA=1-\frac{Misses+FP+Switches}{GT}">
</p>

- **Multiple Object Tracking Precision (MOTP):** the sum of the overlaps of matched boxes divided by the total number of matches. It is an indicator for localization precision. We report percentage MOTP for evaluation.

<p align="center">
  <img src="https://latex.codecogs.com/svg.latex?MOTP=\frac{\sum_i{Overlap_i}}{Matches}">
</p>

- **Number of missed boxes (Misses):** The total number of missed ground-truth boxes.

- **Number of false positives (FP):** The total number of predicted boxes that are not matched with any ground-truth box.

- **Identity switch (Switch):** An identity switch is counted when a ground-truth object is matched with a track that is different from the last known assigned track.

- **Number of mostly tracked objects (Mostly Tracked):** The number of tracks that has at least 80% of its lifespan tracked.

- **Number of mostly lost objects (Mostly Lost):** The number of tracks that has less than 20% of its lifespan tracked.

- **Number of partially tracked objects (Partially Tracked):** The number of tracks that has at least 20% and less than 80% of its lifespan tracked.
