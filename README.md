# awesome-video-domain-adaptation
[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT) 

__This repo is a comprehensive collection of awesome research (papers, codes, etc.) and other items about video domain adaptation.__ 

Domain adaptation has been a focus of research in transfer learning, enabling models to improve robustness which is crucial to apply models to real-world applications. Despite a long history of domain adaptation research, there has been limited discussions on __video domain adaptation__. This repo aims to present a collection of research on video domain adaptation including papers, code, etc. 

_Feel free to star, fork or raise an issue to include your research or to add in more categories! Discussion is most welcomed!_

# Contents
- [awesome-video-domain-adaptation](#awesome-video-domain-adaptation)
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

## Survey

## Closed-set VDA
**Conference**
- Multi-Modal Domain Adaptation for Fine-Grained Action Recognition [[CVPR2020 Oral]](http://openaccess.thecvf.com/content_CVPR_2020/papers/Munro_Multi-Modal_Domain_Adaptation_for_Fine-Grained_Action_Recognition_CVPR_2020_paper.pdf) [[Code-TensorFlow]](https://github.com/jonmun/MM-SADA-code)
- Temporal Attentive Alignment for Large-Scale Video Domain Adaptation [[ICCV2019 Oral]](http://openaccess.thecvf.com/content_ICCV_2019/papers/Chen_Temporal_Attentive_Alignment_for_Large-Scale_Video_Domain_Adaptation_ICCV_2019_paper.pdf) [[Code-Pytorch]](https://github.com/olivesgatech/TA3N)
- Temporal Attentive Alignment for Video Domain Adaptation [[CVPRW 2019]](https://arxiv.org/abs/1905.10861v5) [[Code-Pytorch]](https://github.com/olivesgatech/TA3N)

**Journal**

**ArXiv**


# Datasets
We collect relevant datasets designed for video domain adaptation. Datasets are designed for __closed-set__ video domain adaptation addressing __action recognition by default__. Note that downloading some datasets may require permissions. You are advised to download common action recognition datasets e.g., [HMDB51](https://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/), [UCF101](https://www.crcv.ucf.edu/data/UCF101.php), [Kinetics](https://www.deepmind.com/open-source/kinetics), which are commonly used in these cross-domain video datasets.

- [Sports-DA](https://xuyu0010.github.io/msvda.html#data-download)
- [Daily-DA](https://xuyu0010.github.io/msvda.html#data-download)
- [HMDB-ARID](https://xuyu0010.github.io/vuda.html#papers-and-download) [The Full ARID (v1.0)](https://xuyu0010.github.io/arid.html#papers-and-download)
- [Epic-Kitchens Download](https://github.com/jonmun/MM-SADA-code) [Epic-Kitchens Splits](https://github.com/jonmun/MM-SADA_Domain_Adaptation_Splits) [The Full Epic-Kitchens](https://epic-kitchens.github.io/2022)
- [UCF-HMDB _<sub>full</sub>_](https://github.com/olivesgatech/TA3N)
- [UCF-HMDB _<sub>small</sub>_](https://github.com/olivesgatech/TA3N)

<sup><sub>The original [link](http://cs.stanford.edu/people/karpathy/deepvideo) seems unreachable.</sub></sup>

- [UCF-Olympic](https://github.com/olivesgatech/TA3N)
