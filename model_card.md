# YOLOv7 Configuration
yolov7:
  model_path: 'yolov7x.pt'  # Path to the YOLOv7 model weights
  img_size: 640  # Input image size for YOLOv7
  conf_thres: 0.5  # Object confidence threshold
  iou_thres: 0.45  # Non-maximum suppression IOU threshold

# DeepSORT Configuration
deepsort:
  max_age: 30  # Maximum number of missed frames before deactivating a track
  n_init: 3  # Number of consecutive detections to start a new track
  nn_budget: 100  # Maximum size of the appearance descriptors gallery
  max_cosine_distance: 0.3  # Cosine distance threshold for association

# General Configuration
video_path: 'path/to/input/video.mp4'  # Path to the input video file
output_path: 'path/to/output/folder'  # Path to save the output video
show_video: True  # Whether to display the video during processing
save_video: True  # Whether to save the output video
draw_tracks: True  # Whether to draw the object tracks on the video

# Visualization
line_thickness: 2  # Thickness of the bounding box lines
box_color: [0, 255, 0]  # Color of the bounding boxes (RGB)
font_size: 0.5  # Font size for the object IDs
font_thickness: 1  # Thickness of the font for object IDs
