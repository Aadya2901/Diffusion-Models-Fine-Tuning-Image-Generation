# AI Storytelling: Diffusion Models Fine-Tuning for Image Generation

📌 **Project Overview**  
This project explores **fine-tuning diffusion models** for customized image generation. We experiment with prompt engineering, guidance scales, and training parameters to analyze how model fine-tuning affects output quality, creativity, and prompt adherence.

📊 **Key Insights from Analysis**  
- **Model Used:** Stable Diffusion XL (SDXL) base model  
- **Dataset:** Custom or curated image prompts for fine-tuning  
- **Preprocessing:** Image resizing, normalization, and optional augmentations  
- **Parameter Effects:** Guidance scale has a strong influence on creativity vs. realism  
- **Observations:**  
  - Low guidance → creative but abstract  
  - Medium guidance → balanced realism and artistry  
  - High guidance → accurate but sometimes over-saturated  

---

### Parameter Explored
- **Guidance Scale Values Tested:** `[1.5, 5.0, 7.5, 12.5]`  
- **Other Parameters:**  
  - `num_inference_steps = 30` (fixed for consistency)  
  - `seed = 42` (reproducibility)  

---

## 🖼️ Observations on Generated Images

- **Guidance Scale = 1.5**
  - Highly creative, abstract outputs  
  - Objects often blend into background  
  - Artistic, but lacks clarity  

- **Guidance Scale = 5.0**
  - Balanced creativity & structure  
  - Objects clearly recognizable  
  - Visually coherent  

- **Guidance Scale = 7.5**
  - **Sweet spot** ✅  
  - Sharp, photorealistic, aligned with prompt  
  - Best trade-off between realism & creativity  

- **Guidance Scale = 12.5**
  - Very literal representation  
  - Slight over-saturation  
  - Accuracy prioritized over artistry  

---

## 📂 Repository Contents
- `Diffusion_FineTuning_Experiment.ipynb` → Full notebook:  
  - Load SDXL pipeline  
  - Fine-tune model / generate images  
  - Visualize results side-by-side for different guidance scales  
- 📊 Saved plots of generated images (`results.png`)  
- 📑 Analysis and conclusions  

---

## 🔮 Future Work
- 🌱 **More Prompts:** Test abstract, anime, or fantasy themes  
- 🎨 **Image-to-Image:** Conditioning on sketches or reference images  
- 🧠 **ControlNet/LoRA:** Fine-grained control for pose, style, or objects  
- 📉 **Efficiency:** FP16 + GPU optimization for faster inference  

---

## ⚡ References
- [Stable Diffusion XL](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)  
- [Hugging Face Diffusers Library](https://huggingface.co/docs/diffusers/index)  
- [Original Stable Diffusion Paper](https://arxiv.org/abs/2112.10752)  

---

## ✨ Author
👩‍💻 **Aadya Patel**  
Exploring AI Creativity | #21Days21Projects 🚀
