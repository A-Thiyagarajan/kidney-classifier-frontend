# Kidney Disease Classifier - Frontend

🫘 **AI-Powered Kidney CT Scan Classification Web Application**

[![GitHub Pages](https://img.shields.io/badge/Deployed-GitHub%20Pages-blue?logo=github)](https://yourusername.github.io/kidney-classifier-frontend/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Status: Active](https://img.shields.io/badge/Status-Active-green)]()

## 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/your-username/kidney-classifier-frontend.git
cd kidney-classifier-frontend

# Option 1: Deploy to GitHub Pages
# Just push to main branch - automatic deployment via GitHub Actions

# Option 2: Local development
# Python HTTP server
python -m http.server 8000

# Option 3: Using Node.js
npx http-server
```

Then open `http://localhost:8000/Kidney-Classifier/`

## 📁 Project Structure

```
kidney-classifier-frontend/
│
├── Kidney-Classifier/              # Main application
│   ├── index.html                  # 🎯 Main web app (GitHub Pages)
│   ├── label.json                  # Class labels mapping
│   ├── app.py                      # Flask backend (optional)
│   └── Kidney.h5                   # Model file (large - in .gitignore)
│
├── .github/
│   └── workflows/
│       └── pages.yml               # GitHub Pages deployment
│
├── .gitignore                      # Git ignore rules
├── README.md                       # This file
├── DEPLOYMENT.md                   # Detailed deployment guide
└── LICENSE                         # MIT License
```

## ✨ Features

- ✅ **Responsive Design** - Mobile, tablet, and desktop optimized
- ✅ **Drag & Drop Upload** - Intuitive file upload interface
- ✅ **Batch Processing** - Analyze multiple images at once
- ✅ **Real-time Predictions** - Instant disease classification
- ✅ **High Accuracy** - 99.96% test accuracy
- ✅ **4 Disease Classes** - Cyst, Normal, Stone, Tumor
- ✅ **Privacy First** - No data logging or storage

## 🎯 Classes

The model classifies kidney CT scans into:

| Class | Description |
|-------|-------------|
| **Cyst** | Fluid-filled sac in kidney |
| **Normal** | Healthy kidney tissue |
| **Stone** | Kidney stone/calculus |
| **Tumor** | Abnormal tissue growth |

## 🌐 Deployment

### GitHub Pages (Recommended)

1. **Enable GitHub Pages:**
   - Go to Settings → Pages
   - Source: Deploy from branch
   - Select `main` branch, `/root` folder

2. **Automatic Deployment:**
   - Push changes: `git push origin main`
   - GitHub Actions handles deployment automatically
   - Live in ~30 seconds

3. **Access Your Site:**
   ```
   https://your-username.github.io/kidney-classifier-frontend/Kidney-Classifier/
   ```

### Backend API

The frontend connects to a backend API for predictions:

**Default:** `https://thiyagu2004-kidney-classifier.hf.space/predict`

To use your own backend:
1. Deploy backend on Hugging Face Spaces, Railway, or Render
2. Edit `Kidney-Classifier/index.html` line ~2134
3. Change API endpoint URL

## 📊 Performance

| Metric | Value |
|--------|-------|
| Page Load | < 2s |
| Image Analysis | < 3s |
| Model Accuracy | 99.96% |
| Lighthouse Score | 95+ |
| Mobile Ready | ✅ Yes |

## 🛠️ Tech Stack

**Frontend:**
- HTML5, CSS3, JavaScript (Vanilla)
- Responsive Grid & Flexbox
- Image Preview with URL.createObjectURL

**Backend:**
- Python 3.8+
- Flask / FastAPI
- TensorFlow / Keras
- NumPy, Pillow

**Deployment:**
- GitHub Pages (Frontend)
- Hugging Face Spaces (Backend)
- GitHub Actions (CI/CD)

## 📱 Browser Support

| Browser | Support |
|---------|---------|
| Chrome  | ✅ 90+ |
| Firefox | ✅ 88+ |
| Safari  | ✅ 14+ |
| Edge    | ✅ 90+ |
| Mobile  | ✅ iOS 14+, Android 10+ |

## 🔧 Configuration

### Change API Endpoint

Edit `Kidney-Classifier/index.html` (line ~2134):

```javascript
// Current
const HF_API = 'https://thiyagu2004-kidney-classifier.hf.space/predict';

// Change to your endpoint
const HF_API = 'https://your-api-endpoint.com/predict';
```

### Update Labels

Edit `Kidney-Classifier/label.json`:

```json
{
  "0": "Cyst",
  "1": "Normal",
  "2": "Stone",
  "3": "Tumor"
}
```

## 🚨 Troubleshooting

| Issue | Solution |
|-------|----------|
| Images not uploading | Check file size (< 5MB), format (PNG/JPG) |
| API errors | Verify endpoint URL, check CORS headers |
| Mobile issues | Clear cache, use latest browser |
| Pages not deploying | Check GitHub Actions logs, verify branch |

## 📖 Documentation

- **[DEPLOYMENT.md](DEPLOYMENT.md)** - Detailed deployment instructions
- **[Kidney-Classifier/README.md](Kidney-Classifier/README.md)** - App documentation

## 🤝 Contributing

Contributions welcome! Please:

1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing`)
3. Commit changes (`git commit -m 'Add feature'`)
4. Push to branch (`git push origin feature/amazing`)
5. Open Pull Request

## 📄 License

This project is licensed under the MIT License - see [LICENSE](LICENSE) file for details.

## 🙋 Support

- **Report Issues:** [GitHub Issues](https://github.com/your-username/kidney-classifier-frontend/issues)
- **Discussions:** [GitHub Discussions](https://github.com/your-username/kidney-classifier-frontend/discussions)
- **Email:** your-email@example.com

## 🎓 Citation

```bibtex
@software{kidney_classifier_2024,
  title={Kidney Disease Classifier - Web Application},
  author={Your Name},
  year={2024},
  url={https://github.com/your-username/kidney-classifier-frontend}
}
```

## 🔗 Links

- 🌐 **Live Demo:** [GitHub Pages](https://yourusername.github.io/kidney-classifier-frontend/Kidney-Classifier/)
- 📚 **Backend Repo:** [HF Spaces](https://huggingface.co/spaces/thiyagu2004/kidney-classifier)
- 👤 **Author:** [Thiyagarajan](https://github.com/A-Thiyagarajan)

---

**Last Updated:** April 2024 | **Status:** ✅ Active & Maintained