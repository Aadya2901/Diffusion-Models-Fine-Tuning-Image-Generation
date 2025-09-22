
### Parameter Explored
- **Guidance Scale Values Tested:** `[1.5, 5.0, 7.5, 12.5]`  
- **Other Parameters:**  
  - `num_inference_steps = 30` (fixed for consistency)  
  - `seed = 42` (reproducibility)  

---

## 🖼️ Observations on Generated Images

- **Guidance Scale = 1.5**
  - Highly creative, abstract outputs  
  - Astronaut/horse often blended into background  
  - Lacked structure, but artistic  

- **Guidance Scale = 5.0**
  - Balanced creativity & clarity  
  - Distinct astronaut, horse, and Martian landscape  
  - Outputs felt more coherent  

- **Guidance Scale = 7.5**
  - **Sweet spot** ✅  
  - Sharp, photorealistic, well-aligned with prompt  
  - Best trade-off between realism & creativity  

- **Guidance Scale = 12.5**
  - Very literal → astronaut + horse + Mars clearly visible  
  - Slightly over-saturated, less natural aesthetics  
  - Accuracy > artistry  

---

## 📂 Repository Contents
- `SDXL_GuidanceScale_Experiment.ipynb` → Full notebook:
  - Load SDXL pipeline  
  - Generate images with varying guidance scales  
  - Visualize results (side-by-side comparison)  
- 📊 Saved plots of generated images (`results.png`)  
- 📑 Analysis and conclusions  

---

## 🔮 Future Work
- 🌱 **More Prompts:** Test on abstract/artistic prompts (e.g., anime, fantasy)  
- 🎨 **Image-to-Image:** Explore conditioning on input sketches  
- 🧠 **ControlNet/LoRA:** Add fine-grained control for pose or style  
- 📉 **Efficiency:** Try `fp16` + GPU optimizations for faster inference  

---

## ⚡ References
- [Stable Diffusion XL](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)  
- [Hugging Face Diffusers Library](https://huggingface.co/docs/diffusers/index)  
- [Original Stable Diffusion Paper](https://arxiv.org/abs/2112.10752)  

---

## ✨ Author
👩‍💻 **Aadya Patel**  
Exploring AI Creativity | #21Days21Projects 🚀  
