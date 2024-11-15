# Scene123: One Prompt to 3D Scene Generation via Video-Assisted and Consistency-Enhanced MAE


 As Artificial Intelligence Generated Content (AIGC) advances, a variety of methods have been developed to generate text, images, videos, and 3D objects from single or multimodal inputs, contributing efforts to emulate human-like cognitive content creation. However, generating realistic large-scale scenes from a single input presents a challenge due to the complexities involved in ensuring consistency across extrapolated views generated by models. Benefiting from recent video generation models and implicit neural representations, we propose Scene123, a 3D scene generation model,  that not only ensures realism and diversity through the video generation framework but also uses implicit neural fields combined with Masked Autoencoders (MAE) to effectively ensures the consistency of unseen areas across views. Specifically, we initially warp the input image (or an image generated from text) to simulate adjacent views, filling the invisible areas with the MAE model. However, these filled images usually fail to maintain view consistency, thus we utilize the produced views to optimize a neural radiance field, enhancing geometric consistency. Moreover, to further enhance the details and texture fidelity of generated views, we employ a GAN-based Loss against images derived from the input image through the video generation model. Extensive experiments demonstrate that our method can generate realistic and consistent scenes from a single prompt. Both qualitative and quantitative results indicate that our approach surpasses existing state-of-the-art methods.



![image](https://github.com/YiyingYang12/Scene123-One-Image-to-3D-scene-generation/blob/main/Figure/pipeline.png)


## 🚩 News

- [2024/08/10] Upload paper.
- [2024/08/26] Upload videos on the [project page](https://yiyingyang12.github.io/Scene123.github.io/).


## ⚡  Quick Start




 ## 📖 Citation

If you find our code or paper helpful, please consider citing:

```bibtex
@misc{yang2024scene123prompt3dscene,
      title={Scene123: One Prompt to 3D Scene Generation via Video-Assisted and Consistency-Enhanced MAE}, 
      author={Yiying Yang and Fukun Yin and Jiayuan Fan and Xin Chen and Wanzhang Li and Gang Yu},
      year={2024},
      eprint={2408.05477},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2408.05477}, 
}
