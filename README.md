# building_a_visual_agent

## Introduction

Agentic Object Detection was touched upon by Andrew Ng [recently](https://www.linkedin.com/posts/andrewyng_introducing-agentic-object-detection-given-activity-7293302466249441280-GxAl?utm_source=share&utm_medium=member_desktop&rcm=ACoAABug4sMBXeiiqK6sYTENlHV1ZZl1T1l5neM), as part of [LandingAI](https://va.landing.ai/demo/agentic-od). The implementation is open-source and available on LandingAI's [GitHub repository](https://github.com/landing-ai/vision-agent).

This repository explores the mechanics of an agentic object detection pipeline. Traditionally, object detection has been a closed-vocabulary, closed-domain problem, where models could only detect objects they were explicitly trained on. These models lacked the flexibility to recognize objects beyond their training data. However, the emergence of multimodal models like CLIP has enabled open-vocabulary object detection models such as OWL-ViT, Florence, and DINO, which can detect objects in images based on text prompts.

While open-vocabulary models offer greater flexibility than their predecessors, they may still struggle to detect objects tied to nuanced concepts or interpret user queries accurately. Agentic Object Detection aims to bridge this gap by enabling a system to reason about a user’s request and detect the relevant concepts in the image accordingly. LandingAI [demonstrated](https://landing.ai/agentic-object-detection) that their technique leads to improved performance on object detection benchmarks compared to other existing techniques

## Pipeline

This repository attempts to build an Agentic Object Detection pipeline using Vision-Language Models (VLMs) alongside Open-Vocabulary Object Detection models. Our approach involves a 5-step pipeline, where VLMs act as reasoning agents and reviewers, working in tandem with object detection models to refine and improve the detection process.

![image](https://github.com/user-attachments/assets/8bb2f6f2-9798-4f9e-a301-19a66c49dc66)

## Demo Video

https://github.com/user-attachments/assets/0cdb7e2d-9e15-4e53-8967-8556f9e09b0a

(Video was recorded using https://cursorful.com/ and edited using Flexclip for speeding up the video. The inference process is sped up by a higher factor for representation. The actual inference will take quite a bit of time. In  this repo, the demo video is only allowed for personal and non-commercial use to respect the terms of the Cursorful tool for free usage.

The image used in this video is a photo by <a href="https://unsplash.com/@frank_leuderalbert?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Frank Leuderalbert</a> on <a href="https://unsplash.com/photos/blue-ceramic-cup-with-saucer-on-table-RTVYnQsLgZ0?utm_content=creditCopyText&utm_medium=referral&utm_source=unsplash">Unsplash</a>
      )

## Contributors
Built by [Anand Subramanian](https://www.linkedin.com/in/anand-subu/) and [Bharath Sripathy](https://www.linkedin.com/in/bharath-sripathy-866666156/)

## Running the Demo
1. Run `pip install -r requirements.txt`
2. Run `python main.py` to spin up the Gradio Demo App.



