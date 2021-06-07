# Insights from Images
This proof of concept focuses on helping the global brand Uniqlo understand consumer behavior. We would be going about this by being able to detect uniqlo products and people in images using zero shot/few shot learning based object detection. After which we would be going on to captioning these images hoping to capture how the user is using the product or anything else that could serve as an actionable insight.

## Data collected

##### **Last updated 06/05/2021

The data collected from the instagram account @uniqlousa can be found [here](https://drive.google.com/drive/folders/1pOhZzIuDAAYGgHg9m_q_EYC4aqcRBHEt?sp=sharing) . Some of the metadata in terms of json files are missing for which the scraping needs to be repeated.  This will be updated again, very soon.

To uncompress the json files and view the metadata in a readable format you could use jq (for ubuntu) and the following command:

	xzcat 2021-05-31_19-09-24_UTC.json.xz | jq .node
	
##### ** TODO: add a short table explaining the various datapoints for quick reference

##### ** TODO: add a snapshot of the consolidated csv file

## Public datasets

## References 
#### Object Detection
1. Synthesizing the Unseen for Zero-shot Object Detection (2020) [[paper]](https://arxiv.org/pdf/2010.09425v1.pdf)  [[code]](https://github.com/nasir6/zero_shot_detection).
2. Zero-Shot Object Detection: Learning to Simultaneously Recognize and Localize Novel Concepts (2018) [[paper]](https://arxiv.org/abs/1803.06049) [[code]](https://github.com/salman-h-khan/ZSD_Release) 
3. Latent Embedding Feedback and Discriminative Features for Zero-Shot Classification (ECCV 2020) [[paper]](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123670477.pdf)  [[code]](https://github.com/akshitac8/tfvaegan) 

#### Image Captioning
1. Fast Parameter Adaptation for Few-shot Image Captioning
and Visual Question Answering [[paper]](https://xuanyidong.com/resources/papers/ACM-MM-18-FPAIT.pdf) 


For a more extensive list of resources and future references the following 'awesome'-github repositories may be useful. 

- [Papers and implementations of image augmentation, image duplication and object detection](https://github.com/daicoolb/Awesome-Object-Detections) : Last updated 1 June 2020
- [Papers on zero shot object detection](https://github.com/amusi/awesome-object-detection) : an older collection that has a few papers on zero shot object-detection and no implementations.
- [A collection of papers/code on few shot learning](https://github.com/Duan-JM/awesome-papers-fewshot) : 
- [Papers and implementations of image captioning](https://github.com/forence/Awesome-Visual-Captioning) :
- [Datasets and popular implementations of image captioning](https://ghttps://github.com/zhjohnchan/awesome-image-captioning) : implementations based on tools like pytorch and tensorflow


## Useful tools
- Scraper used to download pictures and other metadata from instagram: [Instaloader](https://instaloader.github.io/) 
- Data annotation tool for manually labelling products: [Diffgram](https://diffgram.com/) 

## Feedback and contribution

