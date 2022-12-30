# Insights from Images
This proof of concept focuses on helping the japanese casual wear designer, manufacturer and retailer Uniqlo understand consumer behavior. We would be going about this by being able to detect uniqlo products and people in images using object detection. After which we would be going on to captioning these images hoping to capture how the user is using the product or anything else that could serve as an actionable insight.

## Final results can be found in the following links : 
- [First iteration results of object detection] (https://docs.google.com/document/d/1leReyR9DA2lXgw79E1_p3VAj1fZOeOz2OR4sFo_Vej8/edit?usp=sharing)
- [Higher precision object detection] (https://docs.google.com/document/d/1HjyabaysBtBvYmTqeOc6Z8J-7GgFNML8MwzONHhhObE/edit?usp=sharing)
- [Image Captioning first iteration results] (https://docs.google.com/document/d/132Y-U--M0RVxsyUefTkoba17jXZkz5VRlghiu_AlRlg/edit?usp=sharing)
- [Presentation on poc of insights from images] (https://docs.google.com/presentation/d/1xgAUwv6C65SMrzRIYnuiyTgX3am_Q37Ett1TVt9ERlo/edit?usp=sharing)

## Data collected

##### **Last updated 06/05/2021

The data collected from the instagram account @uniqlousa can be found [here](https://drive.google.com/drive/folders/1pOhZzIuDAAYGgHg9m_q_EYC4aqcRBHEt?sp=sharing) . Some of the metadata in terms of json files are missing for which the scraping needs to be repeated.  This will be updated again.

To uncompress the json files and view the metadata in a readable format you could use jq (for ubuntu) and the following command:

	xzcat 2021-05-31_19-09-24_UTC.json.xz | jq .node
	
##### ** TODO: add a short table explaining the various datapoints for quick reference

##### ** TODO: add a snapshot of the consolidated csv file



## Usage



## Demo






## Public Datasets
- Zalando's dataset [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist) which covers products from their catalogue.
- A [customized dataset](https://github.com/berkandemirel/fashion-zero-shot-detection-dataset)  for zero shot object detection based on Fashion-MNIST. ([paper](https://arxiv.org/pdf/1805.06157.pdf))
- [DeepFashion](http://mmlab.ie.cuhk.edu.hk/projects/DeepFashion.html) is a large scale clothes database. Take a look at the benchmarks as well for possible ideas. 



## References 



#### Instance Segmentation
1. Zero-Shot Instance Segmentation (CVPR 2021) [[paper]](https://arxiv.org/pdf/2104.06601.pdf) [[code]](https://github.com/zhengye1995/Zero-shot-Instance-Segmentation) 

#### Object Detection 

1. GTNet: Generative Transfer Network for Zero-Shot Object Detection (AAAI 2020) [[paper]](https://arxiv.org/pdf/2001.06812v2.pdf) 
4. Latent Embedding Feedback and Discriminative Features for Zero-Shot Classification (ECCV 2020) [[paper]](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123670477.pdf)  [[code]](https://github.com/akshitac8/tfvaegan) 
5. Synthesizing the Unseen for Zero-shot Object Detection (2020) [[paper]](https://arxiv.org/pdf/2010.09425v1.pdf)  [[code]](https://github.com/nasir6/zero_shot_detection).
3. Zero-Shot Object Detection: Learning to Simultaneously Recognize and Localize Novel Concepts (2018) [[paper]](https://arxiv.org/abs/1803.06049) [[code]](https://github.com/salman-h-khan/ZSD_Release) 





#### Image Captioning
1. Fast Parameter Adaptation for Few-shot Image Captioning
and Visual Question Answering (ACM 2018) [[paper]](https://xuanyidong.com/resources/papers/ACM-MM-18-FPAIT.pdf) 


For a more extensive list of resources and future references the following 'awesome'-github repositories may be useful.
 
- [Zero-shot object detection ](https://github.com/KennithLi/Awesome-Zero-Shot-Object-Detection) 
- [Papers and implementations of image augmentation, image duplication and object detection](https://github.com/daicoolb/Awesome-Object-Detections) 
- [Papers on zero shot object detection](https://github.com/amusi/awesome-object-detection) : older collection of zsd, no code.
- [A collection of papers/code on few shot learning](https://github.com/Duan-JM/awesome-papers-fewshot)
- [Papers and implementations of image captioning](https://github.com/forence/Awesome-Visual-Captioning) 
- [Datasets and popular implementations of image captioning](https://ghttps://github.com/zhjohnchan/awesome-image-captioning) 





## Useful tools
- Scraper used to download pictures and other metadata from instagram: [Instaloader](https://instaloader.github.io/) 
- Data annotation tool for manually labelling products: [Diffgram](https://diffgram.com/) 
- Object detection and instance segmentation components and modules: [mmdetection](https://github.com/open-mmlab/mmdetection) 
- An open source visual analysis toolbox which does fashion attribute prediction, in-shop clothes retrieval, fashion parsing and segmentation, fashion landmark (upper body , lower body clothes) detection, fashion compatibility and recommendation and virtual try ons. ***(This is an incredibly useful resource!)*** : [mmfashion](https://github.com/open-mmlab/mmfashion) 


## Use cases 
- [How facebook uses computer vision to aid shopping?](https://ai.facebook.com/blog/advancing-ai-to-make-shopping-easier-for-everyone/ ) 

## Feedback and contribution

