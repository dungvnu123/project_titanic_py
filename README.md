drone_search/
│  README.md
│  requirements.txt
│
├─data/
│  ├─raw/           # dữ liệu gốc (file zip giải nén vào đây)
│  │   ├─scene_001/
│  │   │   ├─video.mp4
│  │   │   └─images/  (3 ảnh ref)
│  │   ├─scene_002/
│  │   └─...
│  ├─yolo/          # dataset sau khi convert sang YOLO format
│  │   ├─images/
│  │   │   ├─train/
│  │   │   └─val/
│  │   └─labels/
│  │       ├─train/
│  │       └─val/
│  └─outputs/       # kết quả inference (video có bbox, file submit)
│
├─src/
│  ├─__init__.py
│  ├─config.py         # đường dẫn chung, tham số chung
│  ├─explore_data.py   # xem thử video + ref
│  ├─extract_frames.py # tách frame từ video để gắn label YOLO
│  ├─train_yolo.py     # script train YOLO
│  └─infer_video.py    # chạy model trên video, xuất bbox
│
└─notebooks/
   └─eda.ipynb         # nếu muốn nghịch thử bằng notebook
