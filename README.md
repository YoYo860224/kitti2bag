# [kitti2bag](https://github.com/tomas789/kitti2bag)

Update pip and numpy for docker.

## Start
* Work Directory
```
├── <T>
│   ├── <T>_drive_<R>_sync
│   ├── calib_cam_to_cam.txt
│   ├── calib_imu_to_velo.txt
│   └── calib_velo_to_cam.txt
└── 2011_09_26
    ├── 2011_09_26_drive_0001_sync
    ├── 2011_09_26_drive_0002_sync
    ├── 2011_09_26_drive_0005_sync
    ├── calib_cam_to_cam.txt
    ├── calib_imu_to_velo.txt
    └── calib_velo_to_cam.txt
```

* Docker Command
```
docker run -v `pwd`:/data -it --rm yoyo860224/kitti2bag -t <T> -r <r> raw_synced
docker run -v `pwd`:/data -it --rm yoyo860224/kitti2bag -t 2011_09_26 -r 0001 raw_synced
```
