# Awesome Video Domain Adaptation
[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT) 

__This repo is a comprehensive collection of awesome research (papers, codes, etc.) and other items about video domain adaptation.__ 

Domain adaptation has been a focus of research in transfer learning, enabling models to improve robustness which is crucial to apply models to real-world applications. Despite a long history of domain adaptation research, there has been limited discussions on __video domain adaptation__. This repo aims to present a collection of research on video domain adaptation including papers, code, etc. 

_Feel free to star, fork or raise an issue to include your research or to add in more categories! Discussion is most welcomed!_

# Contents
- [Contents](#contents)
- [Explanatory Notes](#explanatory-notes)
- [Papers](#papers)
	<!-- - [Survey](#survey) -->
	- [Closed-set VDA](#closed-set-vda)
	- [Partial-set VDA](#partial-set-vda)
	- [Open-set VDA](#open-set-vda)
	- [Universal VDA](#universal-vda)
	- [Multi-Source VDA](#multi-source-vda)
	<!-- - [Multi-Target VDA](#multi-target-vda) -->
	- [Source-Free or Test-time VDA](#source-free-or-test-time-vda)
	- [Black-box VDA](#black-box-vda)
	<!-- - [Zero-shot or Few-shot VDA](#zero-shot-or-few-shot-vda) -->
	<!-- - [Active VDA](#active-vda) -->
	<!-- - [Other Topics in Video Transfer Learning](other-topics-in-video-transfer-learning) -->
- [Datasets](#datasets)
- [Useful Tools and Other Resources](#useful-tools-and-other-resources)

# Explanatory Notes
This repository categorizes video domain adaptation papers according to the domain adaptation scenarios (i.e., closed-set, partial-set, source-free etc.), sorted by date of publish/public appearance. These include both semi-supervised, weakly-supervised and unsupervised DA. By default, VDA research focus on action recognition. For other tasks, related papers will be categorized into the relevant sub-categories.

<sup><sub>This repository is inspired by the [ADA](https://github.com/zhaoxin94/awesome-domain-adaptation) repository, a repository with awesome domain adaptation papers. For more research on domain adaptation (with images/point cloud etc.) you may check out that repository.</sub></sup>

# Papers

<!-- ## Survey -->

## Closed-set VDA

**Conference**
- [Audio-Adaptive Activity Recognition Across Video Domains](https://openaccess.thecvf.com/content/CVPR2022/papers/Zhang_Audio-Adaptive_Activity_Recognition_Across_Video_Domains_CVPR_2022_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2022) [[Code-PyTorch]](https://github.com/xiaobai1217/DomainAdaptation) [[Project Page]](https://xiaobai1217.github.io/DomainAdaptation/)
- [Interact before Align: Leveraging Cross-Modal Knowledge for Domain Adaptive Action Recognition](https://openaccess.thecvf.com/content/CVPR2022/papers/Yang_Interact_Before_Align_Leveraging_Cross-Modal_Knowledge_for_Domain_Adaptive_Action_CVPR_2022_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2022) [[Project Page]](https://www.ut-vision.org/publication/2022-yang-interact/)
- [Multi-Modal Domain Adaptation for Fine-Grained Action Recognition](http://openaccess.thecvf.com/content_CVPR_2020/papers/Munro_Multi-Modal_Domain_Adaptation_for_Fine-Grained_Action_Recognition_CVPR_2020_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2020) Oral [[Code-TensorFlow]](https://github.com/jonmun/MM-SADA-code) [[Project Page]](https://jonmun.github.io/mmsada/)
- [Temporal Attentive Alignment for Large-Scale Video Domain Adaptation](http://openaccess.thecvf.com/content_ICCV_2019/papers/Chen_Temporal_Attentive_Alignment_for_Large-Scale_Video_Domain_Adaptation_ICCV_2019_paper.pdf) IEEE/CVF International Conference on Computer Vision (ICCV) (2019) Oral [[Code-Pytorch]](https://github.com/cmhungsteve/TA3N)  [[Project Page]](https://minhungchen.netlify.app/project/cdar/)
- [Actor and Observer: Joint Modeling of First and Third-Person Videos](https://ieeexplore.ieee.org/document/8578870) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2018) [[Code-PyTorch]](https://github.com/gsig/actor-observer)

**Journal**

**ArXiv and Workshops**
- [Aligning Correlation Information for Domain Adaptation in Action Recognition](https://arxiv.org/abs/2107.04932) ArXiv 2107.04932 [[Project Page]](https://xuyu0010.github.io/vuda.html)
- [Temporal Attentive Alignment for Video Domain Adaptation](https://arxiv.org/abs/1905.10861v5) IEEE/CVF Computer Vision and Pattern Recognition Conference Workshop (CVPRW) (2019) [[Code-Pytorch]](https://github.com/cmhungsteve/TA3N)

## Partial-set VDA

**Conference**
- [Partial Video Domain Adaptation With Partial Adversarial Temporal Attentive Network](https://openaccess.thecvf.com/content/ICCV2021/papers/Xu_Partial_Video_Domain_Adaptation_With_Partial_Adversarial_Temporal_Attentive_Network_ICCV_2021_paper.pdf) IEEE/CVF International Conference on Computer Vision (ICCV) (2021) Oral [[Code-PyTorch]](https://github.com/xuyu0010/PATAN) [[Project Page]](https://xuyu0010.github.io/pvda.html)


# Datasets
We collect relevant datasets designed for video domain adaptation. Datasets are designed for __closed-set__ video domain adaptation addressing __action recognition__ by default. Note that downloading some datasets may require permissions. You are advised to download common action recognition datasets e.g., [HMDB51](https://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/), [UCF101](https://www.crcv.ucf.edu/data/UCF101.php), [Kinetics](https://www.deepmind.com/open-source/kinetics), which are commonly used in these cross-domain video datasets.

**2021-2022**
- [Sports-DA](https://xuyu0010.github.io/msvda.html#data-download)
- [Daily-DA](https://xuyu0010.github.io/msvda.html#data-download)
- [HMDB-ARID](https://xuyu0010.github.io/vuda.html#papers-and-download) [(The Full ARID (v1.0))](https://xuyu0010.github.io/arid.html#papers-and-download)
- [ActorShift](https://xiaobai1217.github.io/DomainAdaptation/)
- [UCF-HMDB _<sub>partial</sub>_](https://xuyu0010.github.io/pvda.html#papers-notes-and-download) (Partial-set)
- [HMDB-ARID _<sub>partial</sub>_](https://xuyu0010.github.io/pvda.html#papers-notes-and-download) (Partial-set)
- [MiniKinetics-UCF](https://xuyu0010.github.io/pvda.html#papers-notes-and-download) (Partial-set)

**2018-2020**
- [Epic-Kitchens Download](https://github.com/jonmun/MM-SADA-code) [(Epic-Kitchens Splits)](https://github.com/jonmun/MM-SADA_Domain_Adaptation_Splits) [(The Full Epic-Kitchens)](https://epic-kitchens.github.io/2022)
- [UCF-HMDB _<sub>full</sub>_](https://github.com/cmhungsteve/TA3N)
- [Charades-Ego](https://prior.allenai.org/projects/charades-ego)

**Before 2015**
- [UCF-HMDB _<sub>small</sub>_](https://github.com/cmhungsteve/TA3N)
(The original [link](http://cs.stanford.edu/people/karpathy/deepvideo) seems unreachable.)
- [UCF-Olympic](https://github.com/cmhungsteve/TA3N)

# Useful Tools and Other Resources

## Challenges for Video Domain Adaptation
*Note: these are the latest editions of the respective challenges, please check their previous versions through their respective websites*
- [5<sup>th</sup> UG2<sup>+</sup> Prize Challenge: Bridging the Gap Between Computational Photography and Visual Recognition (Track 2)](http://cvpr2022.ug2challenge.org/track2.html) IEEE/CVF Computer Vision and Pattern Recognition Conference Workshop (CVPRW) (2022) [2022 UG2+ Workshop](http://cvpr2022.ug2challenge.org/program22.html)
- [Epic-Kitchens-100 2022 Challenge: Domain Adaptation for Action Recognition](https://epic-kitchens.github.io/2022#challenge-domain-adaptation) IEEE/CVF Computer Vision and Pattern Recognition Conference Workshop (CVPRW) (2022) [EPIC@CVPR2022 Workshop](https://eyewear-computing.org/EPIC_CVPR22/)
