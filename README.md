# 🕶️ VAE Glasses Removal – VGG Perceptual Loss
Remove eyeglasses from face images using a simple Variational Autoencoder (VAE).

> 📚 系列作品｜Project Series:
> - [Part 1: Baseline VAE](https://github.com/VanessaTsai0828/vae-glasses-v1-baseline)
> - [Part 2: Grayscale VAE](https://github.com/VanessaTsai0828/vae-glasses-v2-grayinput)
> - [Part 3: VAE with VGG Loss](https://github.com/VanessaTsai0828/vae-glasses-v3-vggloss)
> - [Part 4: Stylized Output VAE](https://github.com/VanessaTsai0828/vae-glasses-v4-stylized)

---

## 🧠 專案內容 | What’s Inside

- 使用 CNN 架構的變分自編碼器，加入 VGG16 感知損失
- 訓練資料為 160x160 的 RGB 臉部影像（有/無眼鏡）
- 更能保留個人特徵、臉部結構與風格
- 損失函數組合為：重建誤差、KL 散度、特徵感知誤差
- 輸出結果為更擬真的去眼鏡臉部影像

- CNN-based Variational Autoencoder with **VGG16 perceptual loss**
- Trained on 160x160 RGB face images (with/without glasses)
- Better retains facial identity, structure, and style
- Combines reconstruction loss, KL divergence, and feature-wise perceptual loss
- Outputs glasses-free face with **enhanced realism**

---

## 📸 範例結果 | Sample Result
![image](https://github.com/user-attachments/assets/add3bef3-a306-461c-b0ba-c9694d8aff4c)


---

## 📌 備註 | Notes

- 損失函數包含：重建 + KL 散度 + Perceptual Loss
- VGG 感知損失使用中間層（如 block3_conv3）特徵比對
- 可作為進入 GAN 前的高品質中階版本

- Loss function includes: reconstruction, KL divergence, and perceptual loss
- Perceptual loss compares VGG intermediate features (e.g., block3_conv3)
- This version serves as a high-quality intermediate step before applying GANs


### 😅 開發者內心話｜Self-Roast Corner
- 我也不知道他為什麼這麼醜...如果你有辦法怎麼讓他變漂亮請告訴我:)
- No idea why it’s this ugly.  If you can make it prettier, you’re officially my hero.
