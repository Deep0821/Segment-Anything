# Track-Anything

***Track-Anything*** is a flexible and interactive tool for video object tracking and segmentation. It is developed upon [Segment Anything](https://github.com/facebookresearch/segment-anything) and [XMem](https://github.com/hkchengrex/XMem), can specify anything to track and segment via user clicks only. During tracking, users can flexibly change the objects they wanna track or correct the region of interest if there are any ambiguities. These characteristics enable ***Track-Anything*** to be suitable for: 
- Video object tracking and segmentation with shot changes. 
- Data annnotation for video object tracking and segmentation.
- Object-centric downstream video tasks, such as video inpainting and editing. 

## Demo

https://user-images.githubusercontent.com/28050374/232842703-8395af24-b13e-4b8e-aafb-e94b61e6c449.MP4

### Video Object Tracking and Segmentation with Shot Changes

https://user-images.githubusercontent.com/30309970/232848349-f5e29e71-2ea4-4529-ac9a-94b9ca1e7055.mp4

### Video Inpainting (with [E2FGVI](https://github.com/MCG-NKU/E2FGVI))

https://user-images.githubusercontent.com/28050374/232959816-07f2826f-d267-4dda-8ae5-a5132173b8f4.mp4

## Get Started
#### Linux
```bash
# Clone the repository:
git clone https://github.com/gaomingqi/Track-Anything.git
cd Track-Anything

# Install dependencies: 
pip install -r requirements.txt

# Install dependencies for inpainting: 
pip install -U openmim
mim install mmcv

# Install dependencies for editing
pip install madgrad 

# Run the Track-Anything gradio demo.
python app.py --device cuda:0 --sam_model_type vit_h --port 12212
```

## Acknowledgement

The project is based on [Segment Anything](https://github.com/facebookresearch/segment-anything) and [XMem](https://github.com/hkchengrex/XMem). Thanks for the authors for their efforts.
