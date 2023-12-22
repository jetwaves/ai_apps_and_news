## 图片应用

1. 图片标注行业已经完蛋了，使用以下技术可以对任意图片进行准确标注。
   - GroundingDINO - detects high-level object classes; in our case, 'car'
   - Segment Anything (SAM) - converts bounding boxes into pixel-perfect masks
   - GPT-4V - adds a precise label; in our case, 'Mercedes'
   - 地址：github.com/roboflow/awesome-openai-vision-api-experiments
