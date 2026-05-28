<p align="center">
  <img src="https://raw.githubusercontent.com/Orange-3DV-Team/SmartDirector/website/assets/logo.png" width="72" style="border-radius: 16px;" />
  &nbsp;&nbsp;
  <img src="https://readme-typing-svg.demolab.com?font=Bebas+Neue&weight=700&size=52&pause=100000&color=F5C542&center=true&vCenter=true&width=500&height=60&lines=SMARTDIRECTOR" alt="SmartDirector" />
</p>

<h3 align="center">Keyframe-Conditioned Cinematic Video Generation with Narrative Pacing Control</h3>

<p align="center">
  <a href="#">Zhida Zhang</a><sup>1</sup>,
  <a href="#">Jie Ma</a><sup>2</sup>,
  <a href="#">Zhan Peng</a><sup>3</sup>,
  <a href="#">Haoxue Wu</a><sup>2</sup>,
  <a href="#">Yang Han</a><sup>2</sup>,
  <a href="#">Jun Liang</a><sup>2</sup>,
  <a href="#">Jie Cao</a><sup>1</sup>,
  <a href="#">Jing Li</a><sup>2</sup>
</p>

<p align="center">
  <sup>1</sup> New Laboratory of Pattern Recognition, Institute of Automation, Chinese Academy of Sciences &nbsp;&nbsp;
  <sup>2</sup> Youku Moku-Lab &nbsp;&nbsp;
  <sup>3</sup> Huazhong University of Science and Technology
</p>

<p align="center">
<a href="https://orange-3dv-team.github.io/SmartDirector/"><img src="https://img.shields.io/static/v1?label=Project%20Page&message=Web&color=green"></a> &ensp;
<a href="https://github.com/Orange-3DV-Team/SmartDirector"><img src="https://img.shields.io/static/v1?label=Code&message=Github&color=blue"></a> &ensp;
<a href="https://arxiv.org/abs/2605.27891"><img src="https://img.shields.io/static/v1?label=Paper&message=arXiv&color=red"></a> &ensp;
</p>

## 🎬 Demo

VIDEO_PLACEHOLDER

## 📝 Abstract

The narrative quality of a video fundamentally determines its perceptual value. Although existing video generation methods can produce visually appealing content, they predominantly rely on sparse conditioning signals such as text prompts or first/last frames, which limits precise control over narrative structure and temporal pacing.

In this paper, we propose **SmartDirector**, a framework that enhances the narrative capacity of video generation models through multiple keyframes. SmartDirector supports flexible generation scenarios including single-shot generation, multi-shot narrative synthesis, and video extension. The framework operates in two stages: **Director-Gen** generates a low-resolution video conditioned on the provided keyframes, and **Director-SR** refines the output by exploiting high-resolution keyframes as semantic anchors to recover fine-grained details. To enable robust multi-keyframe training, we construct a data pipeline that curates single-shot and multi-shot sequences from movies. Extensive experiments demonstrate that SmartDirector substantially outperforms existing state-of-the-art approaches.

## 🔥 Updates

- __[2026.05.28]__: Release the [project page](https://orange-3dv-team.github.io/SmartDirector/).
- __[2026.05.28]__: Paper released on [arXiv](https://arxiv.org/abs/2605.27891).

## 🌟 Citation

If you find our work helpful, please leave us a star ⭐ and cite our paper:

```bibtex
@article{zhang2026smartdirector,
  title     = {SmartDirector: Keyframe-Conditioned Cinematic Video
               Generation with Narrative Pacing Control},
  author    = {Zhang, Zhida and Ma, Jie and Peng, Zhan and Wu, Haoxue
               and Han, Yang and Liang, Jun and Cao, Jie and Li, Jing},
  journal   = {arXiv preprint arXiv:2605.27891},
  year      = {2026}
}
```
