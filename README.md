# Awesome Video Domain Adaptation
[![MIT License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT) 

__This repo is a comprehensive collection of awesome research (papers, codes, etc.) and other items about video domain adaptation.__ 

__Our comprehensive survey on Video Unsupervised Domain Adaptation with Deep Learning is now available. Please check our paper on [arXiv](https://arxiv.org/abs/2211.10412).__

Domain adaptation has been a focus of research in transfer learning, enabling models to improve robustness which is crucial to apply models to real-world applications. Despite a long history of domain adaptation research, there has been limited discussions on __video domain adaptation__. This repo aims to present a collection of research on video domain adaptation including papers, code, etc. 

_Feel free to star, fork or raise an issue to include your research or to add in more categories! Discussion is most welcomed!_


# Contents
- [Contents](#contents)
- [Explanatory Notes](#explanatory-notes)
- [Papers](#papers)
	- [Closed-set VDA](#closed-set-vda)
	- [Partial-set VDA](#partial-set-vda)
	- [Open-set VDA](#open-set-vda)
	- [Multi-Source VDA](#multi-source-vda)
	- [Source-Free or Test-time VDA](#source-free-or-test-time-vda)
	- [Zero-shot VDA (Video Domain Generalization)](#zero-shot-vda-video-domain-generalization)
	- [Other Topics in Video Transfer Learning](#other-topics-in-video-transfer-learning)
- [Datasets](#datasets)
- [Useful Tools and Other Resources](#useful-tools-and-other-resources)


<!-- - [Survey](#survey) -->
<!-- - [Multi-Target VDA](#multi-target-vda) -->
<!-- - [Universal VDA](#universal-vda) -->
<!-- - [Zero-shot or Few-shot VDA](#zero-shot-or-few-shot-vda) -->
<!-- - [Black-box VDA](#black-box-vda) -->
<!-- - [Active VDA](#active-vda) -->

# Explanatory Notes
This repository categorizes video domain adaptation papers according to the domain adaptation scenarios (i.e., closed-set, partial-set, source-free, etc.), sorted by date of publish/public appearance. These include both semi-supervised, weakly-supervised, and unsupervised DA. By default, VDA research focuses on action recognition. For other tasks, the corresponding task would be annotated independently.

Note: *This repository is inspired by the [ADA](https://github.com/zhaoxin94/awesome-domain-adaptation) repository, a repository with awesome domain adaptation papers. For more research on domain adaptation (with images/point cloud etc.), you may check out that repository.*


# Papers

## Closed-set VDA

**Conference**
- [Synthetic-to-Real Domain Adaptation for Action Recognition: A Dataset and Baseline Performances](https://ieeexplore.ieee.org/document/10160416) IEEE International Conference on Robotics and Automation (ICRA) (2023) [[Code]](https://github.com/reddyav1/RoCoG-v2) [[ArXiv]](https://arxiv.org/abs/2303.10280)
- [Recur, Attend or Convolve? On Whether Temporal Modeling Matters for Cross-Domain Robustness in Action Recognition](https://openaccess.thecvf.com/content/WACV2023/papers/Broome_Recur_Attend_or_Convolve_On_Whether_Temporal_Modeling_Matters_for_WACV_2023_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2023)
- [Exploiting Instance-based Mixed Sampling via Auxiliary Source Domain Supervision for Domain-adaptive Action Detection](https://openaccess.thecvf.com/content/WACV2023/papers/Lu_Exploiting_Instance-Based_Mixed_Sampling_via_Auxiliary_Source_Domain_Supervision_for_WACV_2023_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2023) (*Video Action Detection*)
- [Domain Adaptive Video Semantic Segmentation via Cross-Domain Moving Object Mixing](https://openaccess.thecvf.com/content/WACV2023/papers/Cho_Domain_Adaptive_Video_Semantic_Segmentation_via_Cross-Domain_Moving_Object_Mixing_WACV_2023_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2023) (*Video Semantic Segmentation*)
- [Domain Adaptive Video Segmentation via Temporal Pseudo Supervision](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136900612.pdf) European Conference on Computer Vision (ECCV) (2022) [[Code-PyTorch]](https://github.com/xing0047/TPS) (*Video Segmentation*)
- [Audio-Adaptive Activity Recognition Across Video Domains](https://openaccess.thecvf.com/content/CVPR2022/papers/Zhang_Audio-Adaptive_Activity_Recognition_Across_Video_Domains_CVPR_2022_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2022) [[Code-PyTorch]](https://github.com/xiaobai1217/DomainAdaptation) [[Project Page]](https://xiaobai1217.github.io/DomainAdaptation/)
- [Interact before Align: Leveraging Cross-Modal Knowledge for Domain Adaptive Action Recognition](https://openaccess.thecvf.com/content/CVPR2022/papers/Yang_Interact_Before_Align_Leveraging_Cross-Modal_Knowledge_for_Domain_Adaptive_Action_CVPR_2022_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2022) [[Project Page]](https://www.ut-vision.org/publication/2022-yang-interact/)
- [Multi-Level Attentive Adversarial Learning With Temporal Dilation for Unsupervised Video Domain Adaptation](https://openaccess.thecvf.com/content/WACV2022/papers/Chen_Multi-Level_Attentive_Adversarial_Learning_With_Temporal_Dilation_for_Unsupervised_Video_WACV_2022_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2022) [[Code-PyTorch]](https://github.com/justchenpp/MA2L-TD)
- [Dual-Head Contrastive Domain Adaptation for Video Action Recognition](https://openaccess.thecvf.com/content/WACV2022/papers/da_Costa_Dual-Head_Contrastive_Domain_Adaptation_for_Video_Action_Recognition_WACV_2022_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2022) [[Code-PyTorch]](https://github.com/vturrisi/CO2A)
- [Contrast and mix: Temporal contrastive video domain adaptation with background mixing](https://proceedings.neurips.cc/paper/2021/file/c47e93742387750baba2e238558fa12d-Paper.pdf) Conference on Neural Information Processing Systems (NeruIPS) (2021) [[Code-PyTorch]](https://github.com/CVIR/CoMix) [[Project Page]](https://cvir.github.io/projects/comix)
- [Learning Cross-Modal Contrastive Features for Video Domain Adaptation](https://openaccess.thecvf.com/content/ICCV2021/papers/Kim_Learning_Cross-Modal_Contrastive_Features_for_Video_Domain_Adaptation_ICCV_2021_paper.pdf) IEEE/CVF International Conference on Computer Vision (ICCV) (2021)
- [Domain Adaptive Video Segmentation via Temporal Consistency Regularization](https://openaccess.thecvf.com/content/ICCV2021/papers/Guan_Domain_Adaptive_Video_Segmentation_via_Temporal_Consistency_Regularization_ICCV_2021_paper.pdf) IEEE/CVF International Conference on Computer Vision (ICCV) (2021) [[Code-PyTorch]](https://github.com/Dayan-Guan/DA-VSN) (*Video Segmentation*)
- [Unsupervised Curriculum Domain Adaptation for No-Reference Video Quality Assessment](https://openaccess.thecvf.com/content/ICCV2021/papers/Chen_Unsupervised_Curriculum_Domain_Adaptation_for_No-Reference_Video_Quality_Assessment_ICCV_2021_paper.pdf) IEEE/CVF International Conference on Computer Vision (ICCV) (2021) [[Code-PyTorch]](https://github.com/cpf0079/UCDA) (*Video Quality Assessment (VQA)*)
- [Spatio-temporal Contrastive Domain Adaptation for Action Recognition](https://openaccess.thecvf.com/content/CVPR2021/html/Song_Spatio-temporal_Contrastive_Domain_Adaptation_for_Action_Recognition_CVPR_2021_paper.html) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2021)
- [Unsupervised Domain Adaptation for Spatio-Temporal Action Localization](http://faculty.ucmerced.edu/mhyang/papers/bmvc2020_action.pdf) British Machine Vision Conference (BMVC) (2020) (*Video Action Localization*)
- [Adversarial Bipartite Graph Learning for Video Domain Adaptation](https://dl.acm.org/doi/abs/10.1145/3394171.3413897) ACM Multimedia (ACM MM) (2020) [[Code-PyTorch]](https://github.com/Luoyadan/MM2020_ABG)
- [Shuffle and Attend: Video Domain Adaptation](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123570664.pdf) European Conference on Computer Vision (ECCV) (2020)
- [Multi-Modal Domain Adaptation for Fine-Grained Action Recognition](http://openaccess.thecvf.com/content_CVPR_2020/papers/Munro_Multi-Modal_Domain_Adaptation_for_Fine-Grained_Action_Recognition_CVPR_2020_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2020) Oral [[Code-TensorFlow]](https://github.com/jonmun/MM-SADA-code) [[Project Page]](https://jonmun.github.io/mmsada/)
- [Action Segmentation with Joint Self-Supervised Temporal Domain Adaptation](https://openaccess.thecvf.com/content_CVPR_2020/papers/Chen_Action_Segmentation_With_Joint_Self-Supervised_Temporal_Domain_Adaptation_CVPR_2020_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2020) [[Code-PyTorch]](https://github.com/cmhungsteve/SSTDA) [[Project Page]](https://minhungchen.netlify.app/project/cdas/) (*Action Segmentation*)
- [Transferring Cross-domain Knowledge for Video Sign Language Recognition](https://openaccess.thecvf.com/content_CVPR_2020/papers/Li_Transferring_Cross-Domain_Knowledge_for_Video_Sign_Language_Recognition_CVPR_2020_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2020) Oral (*Video Sign Language Recognition*)
- [Adversarial Cross-Domain Action Recognition with Co-Attention](https://arxiv.org/pdf/1912.10405.pdf) AAAI Conference on Artificial Intelligence (AAAI) (2020)
- [Generative Adversarial Networks for Video-to-Video Domain Adaptation](https://ojs.aaai.org/index.php/AAAI/article/view/5750) AAAI Conference on Artificial Intelligence (AAAI) (2020) (*Video Translation (Generation)*)
- [Action Segmentation with Mixed Temporal Domain Adaptation](https://openaccess.thecvf.com/content_WACV_2020/papers/Chen_Action_Segmentation_with_Mixed_Temporal_Domain_Adaptation_WACV_2020_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2020) (*Action Segmentation*)
- [Unsupervised and Semi-Supervised Domain Adaptation for Action Recognition from Drones](https://openaccess.thecvf.com/content_WACV_2020/papers/Choi_Unsupervised_and_Semi-Supervised_Domain_Adaptation_for_Action_Recognition_from_Drones_WACV_2020_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2020)
- [Temporal Attentive Alignment for Large-Scale Video Domain Adaptation](http://openaccess.thecvf.com/content_ICCV_2019/papers/Chen_Temporal_Attentive_Alignment_for_Large-Scale_Video_Domain_Adaptation_ICCV_2019_paper.pdf) IEEE/CVF International Conference on Computer Vision (ICCV) (2019) Oral [[Code-Pytorch]](https://github.com/cmhungsteve/TA3N)  [[Project Page]](https://minhungchen.netlify.app/project/cdar/)
- [Actor and Observer: Joint Modeling of First and Third-Person Videos](https://ieeexplore.ieee.org/document/8578870) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2018) [[Code-PyTorch]](https://github.com/gsig/actor-observer)
- [Deep Domain Adaptation in Action Space](http://bmvc2018.org/contents/papers/0960.pdf) British Machine Vision Conference (BMVC) (2018)

**Journal**
- [Aligning Correlation Information for Domain Adaptation in Action Recognition](https://arxiv.org/abs/2107.04932) IEEE Transactions on Neural Networks and Learning Systems, Early Access (2022) [[Project Page]](https://xuyu0010.github.io/vuda.html)
- [Rescaling Egocentric Vision: Collection, Pipeline and Challenges for EPIC-KITCHENS-100](https://link.springer.com/article/10.1007/s11263-021-01531-2) International Journal of Computer Vision, Volume 130, Pages 33–55 (2022) (Open Access)
- [Dynamic video mix-up for cross-domain action recognition](https://www.sciencedirect.com/science/article/pii/S0925231221017318) Neurocomputing, Volume 471, Pages 358-368 (2022)
- [A Novel Multiple-View Adversarial Learning Network for Unsupervised Domain Adaptation Action Recognition](https://ieeexplore.ieee.org/document/9543528) IEEE Transactions on Cybernetics, Early Access (2021)
- [A Pairwise Attentive Adversarial Spatiotemporal Network for Cross-Domain Few-Shot Action Recognition-R2](https://ieeexplore.ieee.org/document/9268986) IEEE Transactions on Image Processing, Volume 30, Pages 767-782 (2020)
- [Pairwise Two-Stream ConvNets for Cross-Domain Action Recognition With Small Data](https://ieeexplore.ieee.org/document/9288873) IEEE Transactions on Neural Networks and Learning Systems, Volume 33, Pages 1147-1161 (2020) 
- [Evaluation of local spatial–temporal features for cross-view action recognition](https://www.sciencedirect.com/science/article/pii/S092523121501125X) Neurocomputing, Volume 173, Pages 110-117 (2016)

**ArXiv and Workshops**
- [Unsupervised Video Domain Adaptation: A Disentanglement Perspective](https://arxiv.org/abs/2208.07365) ArXiv 2208.07365 [[Code-PyTorch]](https://github.com/ldkong1205/TranSVAE) [[Project Page]](https://ldkong.com/TranSVAE)
- [Memory Efficient Temporal & Visual Graph Model for Unsupervised Video Domain Adaptation](https://arxiv.org/abs/2208.06554) ArXiv 2208.06554
- [Channel-Temporal Attention for First-Person Video Domain Adaptation](https://arxiv.org/pdf/2108.07846v2.pdf) ArXiv 2108.07846v2
- [Unsupervised Domain Adaptation for Video Semantic Segmentation](https://arxiv.org/abs/2107.11052) ArXiv 2107.11052
- [Temporal Attentive Alignment for Video Domain Adaptation](https://arxiv.org/abs/1905.10861v5) IEEE/CVF Computer Vision and Pattern Recognition Conference Workshop (CVPRW) (2019) [[Code-Pytorch]](https://github.com/cmhungsteve/TA3N) (Highly related to [TA3N]((http://openaccess.thecvf.com/content_ICCV_2019/papers/Chen_Temporal_Attentive_Alignment_for_Large-Scale_Video_Domain_Adaptation_ICCV_2019_paper.pdf)))

## Partial-set VDA

**Conference**
- [Partial Video Domain Adaptation With Partial Adversarial Temporal Attentive Network](https://openaccess.thecvf.com/content/ICCV2021/papers/Xu_Partial_Video_Domain_Adaptation_With_Partial_Adversarial_Temporal_Attentive_Network_ICCV_2021_paper.pdf) IEEE/CVF International Conference on Computer Vision (ICCV) (2021) Oral [[Code-PyTorch]](https://github.com/xuyu0010/PATAN) [[Project Page]](https://xuyu0010.github.io/pvda.html)
- [Calibrating Class Weights with Multi-Modal Information for Partial Video Domain Adaptation](https://dl.acm.org/doi/abs/10.1145/3503161.3548095) ACM Multimedia (ACM MM) (2022)

<!-- **ArXiv and Workshops** -->


## Open-set VDA

**Conference**
- [Conditional Extreme Value Theory for Open Set Video Domain Adaptation](https://dl.acm.org/doi/10.1145/3469877.3490600) ACM Multimedia Asia (MMAsia) (2021) [[Code-PyTorch]](https://github.com/zhuoxiao-chen/Open-Set-Video-Domain-Adaptation)
- [Dual Metric Discriminator for Open Set Video Domain Adaptation](https://ieeexplore.ieee.org/document/9413361) IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP) (2021)

**Journal**
- [Open Set Domain Adaptation for Image and Action Recognition](https://ieeexplore.ieee.org/abstract/document/8531764) IEEE Transactions on Pattern Analysis and Machine Intelligence, Volume 42, Issue 2 (2018)

<!-- ## Universal VDA -->

<!-- **Conference** -->
<!-- - [Unsupervised and Semi-Supervised Domain Adaptation for Action Recognition from Drones](https://openaccess.thecvf.com/content_WACV_2020/papers/Choi_Unsupervised_and_Semi-Supervised_Domain_Adaptation_for_Action_Recognition_from_Drones_WACV_2020_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2020) -->


## Multi-Source VDA

**ArXiv and Workshops**
- [Multi-Source Video Domain Adaptation with Temporal Attentive Moment Alignment](https://arxiv.org/abs/2109.09964) ArXiv 2109.09964 [[Project Page]](https://xuyu0010.github.io/msvda.html)


## Source-Free or Test-time VDA

**Conference**
- [Video Test-Time Adaptation for Action Recognition](https://openaccess.thecvf.com/content/CVPR2023/papers/Lin_Video_Test-Time_Adaptation_for_Action_Recognition_CVPR_2023_paper.pdf)  IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2023) [[Code]](https://github.com/wlin-at/ViTTA) [[Supplementary]](https://openaccess.thecvf.com/content/CVPR2023/supplemental/Lin_Video_Test-Time_Adaptation_CVPR_2023_supplemental.pdf)
- [Source-Free Video Domain Adaptation with Spatial-Temporal-Historical Consistency Learning](https://openaccess.thecvf.com/content/CVPR2023/papers/Li_Source-Free_Video_Domain_Adaptation_With_Spatial-Temporal-Historical_Consistency_Learning_CVPR_2023_paper.pdf) IEEE/CVF Computer Vision and Pattern Recognition Conference (CVPR) (2023)
- [Overcoming Label Noise for Source-free Unsupervised Video Domain Adaptation](https://hal.science/hal-03929619/document) Indian Conference on Computer Vision, Graphics and Image Processing (ICVGIP) (2022)
- [Source-free Video Domain Adaptation by Learning Temporal Consistency for Action Recognition](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136940144.pdf) European Conference on Computer Vision (ECCV) (2022) [[Code-PyTorch]](https://github.com/xuyu0010/ATCoN) [[Project Page]](https://xuyu0010.github.io/sfvda.html)
- [Self-supervised Test-time Adaptation on Video Data](https://openaccess.thecvf.com/content/WACV2022/papers/Azimi_Self-Supervised_Test-Time_Adaptation_on_Video_Data_WACV_2022_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2022)

<!-- **ArXiv and Workshops** -->


## Target-Free VDA

**Conference**
- [Cross-Domain Video Anomaly Detection without Target Domain Adaptation](https://openaccess.thecvf.com/content/WACV2023/papers/Aich_Cross-Domain_Video_Anomaly_Detection_Without_Target_Domain_Adaptation_WACV_2023_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2023) (*Video Anomaly Detection*)


## Zero-shot VDA (Video Domain Generalization)

**Conference**
- [Domain Generalization through Audio-Visual Relative Norm Alignment in First Person Action Recognition](https://openaccess.thecvf.com/content/WACV2022/papers/Planamente_Domain_Generalization_Through_Audio-Visual_Relative_Norm_Alignment_in_First_Person_WACV_2022_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2022)

**Journal**
- [VideoDG: generalizing temporal relations in videos to novel domains](https://ieeexplore.ieee.org/abstract/document/9556560) IEEE Transactions on Pattern Analysis and Machine Intelligence (2021)


## Other Topics in Video Transfer Learning

**Conference**
- [CycDA: Unsupervised Cycle Domain Adaptation to Learn from Image to Video](https://www.ecva.net/papers/eccv_2022/papers_ECCV/papers/136630684.pdf) European Conference on Computer Vision (ECCV) (2022)
- [Benchmarking the robustness of Spatial-Temporal Models](https://openreview.net/forum?id=MQlMIrm3Hv5) The Conference on Neural Information Processing Systems (NeurIPS) Datasets and Benchmarks Track (2021) [[Code-TensorFlow]](https://github.com/Newbeeyoung/Video-Corruption-Robustness) (*Video Robustness*)
- [Spatial-temporal causal inference for partial image-to-video adaptation](https://ojs.aaai.org/index.php/AAAI/article/view/16187) AAAI Conference on Artificial Intelligence (AAAI) (2021) [[Code-PyTorch]](https://github.com/ChenJinBIT/HPDA) (*Partial-Set Image-to-Video*)
- [Image to Video Domain Adaptation Using Web Supervision](https://openaccess.thecvf.com/content_WACV_2020/papers/Kae_Image_to_Video_Domain_Adaptation_Using_Web_Supervision_WACV_2020_paper.pdf) IEEE/CVF Winter Conference on Applications of Computer Vision (WACV) (2020) (*Image-to-Video*)
- [DistInit: Learning Video Representations Without a Single Labeled Video](https://openaccess.thecvf.com/content_ICCV_2019/papers/Girdhar_DistInit_Learning_Video_Representations_Without_a_Single_Labeled_Video_ICCV_2019_paper.pdf) IEEE/CVF International Conference on Computer Vision (ICCV) (2019) (*Image-to-Video*)

**Journal**
- [Multi-Domain and Multi-Task Learning for Human Action Recognition](https://ieeexplore.ieee.org/iel7/83/8478029/08476540.pdf) IEEE Transactions on Image Processing, Volume 28, Pages 853-867 (2019)
- [Deep Image-to-Video Adaptation and Fusion Networks for Action Recognition](https://ieeexplore.ieee.org/document/8931264) IEEE Transactions on Image Processing, Volume 29, Pages 3168-3182 (2019) [[Project Page]](https://yangliu9208.github.io/DIVAFN/) (*Image-to-Video*)

**ArXiv**
- [Recur, Attend or Convolve? On Whether Temporal Modeling Matters for Cross-Domain Robustness in Action Recognition](https://arxiv.org/abs/2112.12175) ArXiv 2112.12175


# Datasets
We collect relevant datasets designed for video domain adaptation. Datasets are designed for __closed-set__ video domain adaptation addressing __action recognition__ by default. Note that downloading some datasets may require permission. You are advised to download common action recognition datasets e.g., [HMDB51](https://serre-lab.clps.brown.edu/resource/hmdb-a-large-human-motion-database/), [UCF101](https://www.crcv.ucf.edu/data/UCF101.php), [Kinetics](https://www.deepmind.com/open-source/kinetics), which are commonly used in these cross-domain video datasets.

**2021-2022**
- [Sports-DA](https://xuyu0010.github.io/msvda.html#data-download)
- [Daily-DA](https://xuyu0010.github.io/msvda.html#data-download)
- [HMDB-ARID](https://xuyu0010.github.io/vuda.html#papers-and-download) [(The Full ARID (v1.0))](https://xuyu0010.github.io/arid.html#papers-and-download)
- [ActorShift](https://xiaobai1217.github.io/DomainAdaptation/)
- [Mixamo&rarr;Kinetics](https://github.com/vturrisi/CO2A)
- [UCF-HMDB _<sub>partial</sub>_](https://xuyu0010.github.io/pvda.html#papers-notes-and-download) (*Partial-set*)
- [HMDB-ARID _<sub>partial</sub>_](https://xuyu0010.github.io/pvda.html#papers-notes-and-download) (*Partial-set*)
- [MiniKinetics-UCF](https://xuyu0010.github.io/pvda.html#papers-notes-and-download) (*Partial-set*)
- [VIPER&rarr;Cityscapes-Seq](https://github.com/Dayan-Guan/DA-VSN) (*Video Segmentation*)
- [SYNTHIA-Seq&rarr;Cityscapes-Seq](https://github.com/Dayan-Guan/DA-VSN) (*Video Segmentation*)

**2018-2020**
- [Epic-Kitchens](https://github.com/jonmun/MM-SADA-code) [(Epic-Kitchens Splits)](https://github.com/jonmun/MM-SADA_Domain_Adaptation_Splits) [(The Full Epic-Kitchens)](https://epic-kitchens.github.io/2022)
- [UCF-HMDB _<sub>full</sub>_](https://github.com/cmhungsteve/TA3N)
- [Kinetics-Gameplay](https://github.com/cmhungsteve/TA3N) (*Permission Needed*)
- [Charades-Ego](https://prior.allenai.org/projects/charades-ego)
- [Kinetics&rarr;NEC-Drone](https://www.nec-labs.com/~mas/NEC-Drone/)

**Before 2015**
- [UCF-HMDB _<sub>small</sub>_](https://github.com/cmhungsteve/TA3N)
- [UCF-Olympic](https://github.com/cmhungsteve/TA3N)

# Useful Tools and Other Resources

## Challenges for Video Domain Adaptation
*Note: these are the latest editions of the respective challenges, please check their previous versions through their respective websites*
- [5<sup>th</sup> UG2<sup>+</sup> Prize Challenge: Bridging the Gap Between Computational Photography and Visual Recognition (Track 2)](http://cvpr2022.ug2challenge.org/track2.html) IEEE/CVF Computer Vision and Pattern Recognition Conference Workshop (CVPRW) (2022) [2022 UG2+ Workshop](http://cvpr2022.ug2challenge.org/program22.html)
- [Epic-Kitchens-100 2022 Challenge: Domain Adaptation for Action Recognition](https://epic-kitchens.github.io/2022#challenge-domain-adaptation) IEEE/CVF Computer Vision and Pattern Recognition Conference Workshop (CVPRW) (2022) [EPIC@CVPR2022 Workshop](https://eyewear-computing.org/EPIC_CVPR22/)
