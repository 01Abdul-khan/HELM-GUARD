# HELM-GUARD
Detect riders on two-wheelers and whether they wear helmets. Processes .mp4 files, outputs an annotated video and a CSV log of violations (no-helmet). Built with YOLO (Ultralytics) + DeepSORT tracking and organized for easy model swapping.
Features
Detect person and motorcycle/bicycle and identify riders.
Detect helmets and match them to rider head regions.
Track riders over frames with persistent track_id (DeepSORT).
Log violations in CSV with: video_filename, frame_id, frame_timestamp_ms, wall_clock_iso, track_id, class, confidence, xmin, ymin, xmax, ymax.
Produce an annotated MP4 (outputs/annotated_videos/*.mp4).
Modular src/ package for easy maintenance and packaging.

