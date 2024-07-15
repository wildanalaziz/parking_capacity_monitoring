
# Video Analytics : Parking Capcity Monitoring Using CCTV / Camera Surveillance



Realtime monitoring parking capacity using CCTV / Camera Surveillance

'''
## Deployment

To deploy this project run

```bash
  python "yolo_app_park.py" --source "CCTV 2.mp4" --view-img --save-img --device 0 --weights "yolov8m.pt" --classes 2 --parking-capacity 15
```

parameters
```
--weights, type=str, default=yolov8s.pt, help=initial weights path
--device, default=, help=cuda device, i.e. 0 or 0,1,2,3 or cpu
--source, type=str, required=True, help=video file path
--view-img, action=store_true, help=show results
--save-img, action=store_true, help=save results
--exist-ok, action=store_true, help=existing project/name ok, do not increment
--classes, nargs=+, type=int, help=filter by class: --classes 0, or --classes 0 2 3
--line-thickness, type=int, default=2, help=bounding box thickness
--region-thickness, type=int, default=4, help=Region thickness
-parking-capacity, type=int, default=10, help=Maximum parking capacity
```