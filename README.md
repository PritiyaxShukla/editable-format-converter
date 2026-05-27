# 📄 Editable Format Converter

Transform your text-based images into fully editable documents while keeping the layout intact. No more manual retyping, no more formatting headaches—just clean, editable content.

<div align="center">

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-Open%20Source-green)
![Status](https://img.shields.io/badge/Status-Active-brightgreen)

**[🎬 Watch Demo](https://www.youtube.com/watch?v=P_D-PXji0fc&t=261s) • [📧 Contact](https://sites.google.com/d/11_olnBtz_enKQklok0kt-EpS5Uq09Mhh/p/10EM4k2v2MfIy1Vfr9j7B1qN_ReRC44QY/edit)**

</div>

---

## What This Project Does

Have you ever received a scanned document, a poster, or any image with text and thought, "I wish I could just edit this easily"? That's exactly what this tool solves. It uses advanced AI-powered OCR technology to:

- **Extract text** from images with high accuracy
- **Detect text positions** using intelligent bounding box recognition
- **Remove text** from the original image while preserving the background
- **Generate multiple formats** for different use cases (PDF, Word documents, clean images)

Instead of spending hours manually recreating documents or using clunky workarounds, this tool does it all automatically.

---

## Why You'll Love It

**For Productivity:** Stop wasting time retyping content from images. Get editable text in seconds.

**For Design Work:** Keep your original design aesthetic while making content editable. Update posters, certificates, and marketing materials without starting from scratch.

**For Document Management:** Convert physical documents into proper digital formats that are searchable and editable.

**For Flexibility:** Get multiple output formats—choose the one that works best for your workflow.

---

## Visual Workflow

```
┏━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┓
┃                      YOUR INPUT IMAGE                       ┃
┃                  (Any image with text)                      ┃
┗━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━┯━━━━━━━━━━━━━━━━━━━━━┛
                                      │
                    ┌─────────────────┼─────────────────┐
                    │                 │                 │
                    ▼                 ▼                 ▼
            ┌──────────────┐  ┌──────────────┐  ┌──────────────┐
            │   EasyOCR    │  │ Text Extract │  │  Layout Map  │
            │ Recognition  │  │  & Preserve  │  │  (Bounding   │
            │              │  │              │  │   Boxes)     │
            └──────┬───────┘  └──────┬───────┘  └──────┬───────┘
                   │                 │                 │
                   └─────────────────┼─────────────────┘
                                     │
                    ┌────────────────┼────────────────┐
                    │                │                │
                    ▼                ▼                ▼
            ┌────────────────┐  ┌─────────────┐  ┌──────────────┐
            │ Text Removal   │  │ PDF Creator │  │ DOCX Creator │
            │ & Inpainting   │  │ (Positioned)│  │ (2 versions) │
            │                │  │             │  │              │
            └────────┬───────┘  └──────┬──────┘  └────────┬─────┘
                     │                 │                  │
     ┌───────────────┼─────────────────┼──────────────────┘
     │               │                 │
     ▼               ▼                 ▼
  CLEAN IMAGE     PDF OUTPUT      WORD DOCUMENTS
  (No Text)    (Text + Layout)    (4 total outputs)
```

---

## ⚡ Key Features at a Glance

| 🎯 Feature | 📝 What It Does | ✨ Why You'll Love It |
|-----------|----------------|--------------------|
| **🌐 Gradio Web UI** | Beautiful, click-and-upload interface | No coding needed, instant results |
| **🧠 AI-Powered OCR** | Extracts text with high accuracy | Works with any font and layout |
| **🎨 Layout Preservation** | Remembers exact text positions | Professional output that looks right |
| **📄 4 Output Formats** | Clean image, PDF, 2 Word docs | Pick the format that fits your workflow |
| **⚡ Lightning Fast** | Results in 30-60 seconds | Modern GPU acceleration included |
| **📐 Text Positioning** | Places text exactly where it was | No need to manually reposition |
| **🔧 Open Source** | Free to use & modify | Full transparency, community support |
| **💼 Production Ready** | Tested on real documents | Handles certificates, forms, posters, etc. |

---

## What You Get (Outputs Explained)

When you process an image, the tool generates **four different outputs**, each designed for a specific purpose:

### 1. **Clean Image** 🖼️
```
BEFORE                          AFTER
┌─────────────────┐            ┌─────────────────┐
│ Hello World     │            │                 │
│                 │    ──→      │   (clean image) │
│ This is text    │            │                 │
└─────────────────┘            └─────────────────┘
   (with text)                  (text removed)
```
   - Your original image with all text removed
   - Background and visual elements perfectly preserved
   - **Use this for:** Creating blank templates, updating designs, or as a base for new content

### 2. **Text-Positioned PDF** 📄
   - Extracted text placed exactly where it was in the original image
   - Professional PDF format ready to print or share
   - Text is selectable and searchable
   - **Use this for:** Archiving, sharing read-only versions, or keeping a formatted reference

### 3. **Editable Word Document (Structured)** 📝
   - Text extracted and formatted according to the original layout
   - Fully editable in Microsoft Word or Google Docs
   - Text positions respect the original design
   - **Use this for:** Making quick edits while maintaining the original look

### 4. **Word Document (Clean Image Only)** 📋
   - The clean image inserted into a Word document
   - No text overlay—blank space for you to add or modify content
   - Ready for collaboration and teamwork
   - **Use this for:** Adding fresh content, repurposing the design, or collaborative editing

---

## How to Use

### **Option 1: Gradio Web Interface** (Most User-Friendly)

The easiest way! A beautiful web interface where you can upload images and download results with a few clicks.

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│        🖼️  Editable Format Converter Web Interface         │
│                                                             │
│  ┌──────────────────────────────────────────────────────┐  │
│  │  📤 Upload Image                                     │  │
│  │  ┌────────────────────────────────────┐              │  │
│  │  │ Drag & drop or click to upload     │              │  │
│  │  └────────────────────────────────────┘              │  │
│  └──────────────────────────────────────────────────────┘  │
│                                                             │
│  ┌──────────────────────────────────────────────────────┐  │
│  │ ✓ Processing... (takes 30-60 seconds)               │  │
│  └──────────────────────────────────────────────────────┘  │
│                                                             │
│  📥 Download Your Results:                                │
│  ┌──────────────────────────────────────────────────────┐  │
│  │ ✓ Cleaned Image (Without Text)          [Download]   │  │
│  │ ✓ PDF with Text Positioned              [Download]   │  │
│  │ ✓ Word Document (Structured Layout)     [Download]   │  │
│  │ ✓ Word Document (Clean Image Only)      [Download]   │  │
│  └──────────────────────────────────────────────────────┘  │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**To launch the web interface:**
1. Run the notebook in Colab
2. Find the cell with `gr.Interface(...).launch()`
3. Click the public link to open the web interface
4. Upload your image and download results instantly

---

### **Option 2: Google Colab** (Free GPU!)
The project is built as a Jupyter notebook, optimized for Colab where GPU acceleration is available.

<details>
<summary><strong>📋 Click for step-by-step Colab setup</strong></summary>

```
STEP 1: Prepare
├─ Open editable_format_converter.ipynb
└─ Right-click → "Open with → Google Colaboratory"

STEP 2: Install (Click run on first cell)
├─ !pip install -r requirements.txt
├─ Or: pip install gradio easyocr reportlab opencv-python
└─ Wait for installation (1-2 minutes)

STEP 3: Upload
├─ Click upload button in Colab
├─ Select your image file
└─ Or drag from Google Drive

STEP 4: Run Cells
├─ Execute cells in order (top to bottom)
├─ Watch the progress bars
└─ Wait 30-60 seconds for processing

STEP 5: Download
├─ Right-click generated files
├─ Select "Download"
└─ Save all 4 outputs locally
```

**Pro Tips for Colab:**
- 🚀 Enable GPU: Runtime → Change Runtime Type → GPU
- 💾 Use Google Drive to save files: Mount Drive first
- 🔄 Save notebook to Drive for future use
- ⚡ GPU = 30 sec, CPU = 3 min processing time
</details>

### **Option 3: Local Machine** (Full Control)

<details>
<summary><strong>💻 Click for local setup instructions</strong></summary>

**Prerequisites:**
- Python 3.8 or higher
- pip (Python package manager)
- ~2GB disk space (for OCR models)

**Installation Steps:**

```bash
# 1. Download project files
git clone <repository-url>
cd editable-format-converter

# 2. Create virtual environment (optional but recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# 3. Install dependencies
pip install -r requirements.txt

# 4. Start Jupyter
jupyter notebook

# 5. Open editable_format_converter.ipynb
# 6. Run cells from top to bottom
# 7. Download results from output folder
```

**First Time Setup:**
- Installation: ~3-5 minutes
- First processing: ~2-3 minutes (models download)
- Subsequent processing: ~30-60 seconds

**Note:** Local processing uses your CPU (slower) unless you have CUDA GPU installed.

</details>

---

## 🚀 Installation Option Comparison

| Factor | 🌐 Gradio Web | ☁️ Google Colab | 💻 Local |
|--------|---------------|-----------------|---------|
| **Easiest Setup** | ✅✅✅ Yes | ✅✅ Medium | ✅ Requires Python |
| **Speed** | ⚡⚡⚡ Fastest | ⚡⚡⚡ Fast (GPU) | ⚡⚡ Medium (CPU) |
| **Cost** | Free | Free | Free |
| **Installation Time** | ~2 min | ~2 min | ~5 min |
| **No Coding Needed** | ✅ Yes | ❌ No | ❌ No |
| **GPU Support** | N/A | ✅ Free GPU | ⚠️ Optional |
| **Best For** | Quick processing | Learning | Development |
| **Recommended For** | Everyone | Students | Developers |

**My Recommendation:** 🌟 Start with **Gradio** (simplest) or **Colab** (best value)

---

## Technical Details

### What Powers This

- **EasyOCR**: State-of-the-art text recognition from images
- **ReportLab**: Professional PDF generation with exact text positioning
- **Python-doctr**: Document analysis and text layout understanding
- **OpenCV & NumPy**: Image processing and manipulation
- **Pillow**: Image format handling

### How It Works Behind the Scenes

1. **Image Analysis**: The OCR engine scans your image and detects every piece of text
2. **Layout Mapping**: Bounding boxes identify the exact position of each text element
3. **Text Extraction**: Recognized text is extracted with high accuracy
4. **Background Cleanup**: Inpainting techniques remove text while preserving the background
5. **Multi-Format Generation**: 
   - PDF recreation with positioned text
   - DOCX documents with structured layouts
   - Clean image output for reuse

---

## Real-World Examples

<table>
<tr>
<th>📋 Scenario</th>
<th>📌 What You Have</th>
<th>✅ What You Get</th>
<th>🎯 Result</th>
</tr>
<tr>
<td><strong>Update a Certificate</strong></td>
<td>Scanned diploma image with printed name & date</td>
<td>Editable Word doc + clean image</td>
<td>Edit name/date and reprint instantly</td>
</tr>
<tr>
<td><strong>Fix a Poster</strong></td>
<td>Marketing poster with typos (image format)</td>
<td>Clean image + extracted text</td>
<td>Fix typos and create new version</td>
</tr>
<tr>
<td><strong>Digitize Forms</strong></td>
<td>Stack of scanned form images</td>
<td>Multiple Word documents</td>
<td>Data entry ready, fully editable</td>
</tr>
<tr>
<td><strong>Extract Content</strong></td>
<td>Screenshot or photo of document</td>
<td>Text-positioned PDF + Word doc</td>
<td>Searchable, copyable, no retyping</td>
</tr>
<tr>
<td><strong>Create Templates</strong></td>
<td>Design mockup with sample text</td>
<td>Clean image (text removed)</td>
<td>Ready to use as a blank template</td>
</tr>
</table>

---

## 💡 Tips for Best Results

### ✅ **Do This for Best Results**

```
┌──────────────────────────────────────────┐
│ 🏆 OPTIMIZATION CHECKLIST                │
├──────────────────────────────────────────┤
│ ✓ Use clear, well-lit images             │
│ ✓ Aim for 300+ DPI resolution            │
│ ✓ Test with one image first              │
│ ✓ Check the PDF preview before editing   │
│ ✓ Use ISO standard fonts when possible   │
│ ✓ Ensure good contrast (text vs bg)      │
│ ✓ Keep images straight (no rotation)     │
│ ✓ Avoid shadows over text                │
└──────────────────────────────────────────┘
```

### ❌ **Avoid These Common Mistakes**

```
⚠️  Very small text (under 8pt)
    → May not recognize properly
    
⚠️  Artistic/decorative fonts
    → Lower accuracy with stylized text
    
⚠️  Rotated or skewed images
    → Preprocess with image editing tool
    
⚠️  Poor lighting or contrast
    → Shadows and glare reduce accuracy
```

---

## 🔧 Troubleshooting Guide

<details>
<summary><strong>❓ Text recognition is inaccurate</strong> (Click to expand)</summary>

**Problem:** Some words are being recognized incorrectly or missed.

**Solutions:**
1. Check image quality - ensure it's clear and well-lit
2. Increase DPI to 300+ if possible
3. Manually correct any fancy fonts in the output Word doc
4. Try adjusting contrast using an image editor before uploading

**Pro Tip:** The OCR is 95%+ accurate on clear text, so minor corrections are normal.
</details>

<details>
<summary><strong>❓ Removing text left artifacts on the image</strong> (Click to expand)</summary>

**Problem:** The cleaned image has ghosting or artifacts where text was.

**Solutions:**
1. This is normal with complex backgrounds - use inpainting settings in notebook
2. Use the text-positioned PDF instead (text looks original)
3. Manually touch up the clean image using Paint or Photoshop
4. If background is very textured, consider a different approach

**Pro Tip:** Complex textures = harder cleanup. Simple solid backgrounds work best.
</details>

<details>
<summary><strong>❓ The tool is running slowly</strong> (Click to expand)</summary>

**Problem:** Processing is taking longer than 60 seconds.

**Solutions:**
1. **First run:** Models download automatically (~100MB) - this is normal
2. Use Colab's GPU: Select "Runtime → Change runtime type → GPU"
3. For large images: Resize to max 2000px before uploading
4. Check your internet connection if on Colab

**Pro Tip:** GPU processing: ~30 sec | CPU processing: ~2-3 min
</details>

<details>
<summary><strong>❓ My image has multiple languages</strong> (Click to expand)</summary>

**Problem:** Text in non-English languages isn't recognized well.

**Solutions:**
1. Current version optimizes for English
2. Other languages may work with 80%+ accuracy
3. You can modify the notebook to add language codes
4. Manual correction of any errors is quick

**Pro Tip:** Want to add a language? Edit the EasyOCR reader line to `['en', 'es', 'fr']` etc.
</details>

---

## 🎬 Demo & Tutorial

### **Watch It in Action**

[![Editable Format Converter Demo](https://img.youtube.com/vi/P_D-PXji0fc/maxresdefault.jpg)](https://www.youtube.com/watch?v=P_D-PXji0fc&t=261s)

**[📺 Full Demo on YouTube](https://www.youtube.com/watch?v=P_D-PXji0fc&t=261s)**

In this demo, you'll see:
- ✅ Uploading an image document
- ✅ The Gradio interface in action
- ✅ Real-time text extraction
- ✅ Generation of all 4 output files
- ✅ Quality of the final results
- ✅ How to use each output type

### **Quick Start (30 seconds)**

```
1️⃣  Open the notebook
    ↓
2️⃣  Upload your image
    ↓
3️⃣  Click "Submit"
    ↓
4️⃣  Download 4 files (30-60 sec)
    ↓
5️⃣  Done! Use as needed
```

---

## Project Structure

```
editable-format-converter/
├── README.md                          # Documentation (you are here)
├── requirements.txt                   # Python dependencies
├── editable_format_converter.ipynb    # Main notebook with complete workflow
└── [outputs folder]                   # Generated files (created after processing)
    ├── clean_image.png                # Background without text
    ├── text_positioned.pdf            # PDF with text in original positions
    ├── editable_structured.docx       # Word doc with layout preserved
    └── editable_clean_layout.docx     # Word doc with clean image only
```

---

## 🎯 What's Coming Next

```
ROADMAP
═══════════════════════════════════════════════════════════

Q2 2026
├─ 🔄 Batch Processing (multiple images at once)
├─ 🌍 Multi-language Support (20+ languages)
└─ ⚙️ Advanced OCR Settings (confidence thresholds, etc.)

Q3 2026
├─ 📄 HTML Export (web-ready output)
├─ 📝 Markdown Export (blog post friendly)
└─ 🎨 Enhanced UI/UX improvements

Q4 2026
├─ 🌐 Standalone Web App (no Jupyter needed)
├─ 🔌 REST API (integrate into your apps)
└─ 📱 Mobile app preview

Future
└─ 🤖 Advanced ML models, Cloud storage, Team collaboration

═══════════════════════════════════════════════════════════
```

**Want a specific feature?** [Share your ideas!](#made-by)

---

---

## 👨‍💻 Created By

<div align="center">

### **Pritiyax Shukla**

📧 Full-Stack Developer | ML Enthusiast | Open Source Contributor

[🌐 Visit Portfolio](https://sites.google.com/d/11_olnBtz_enKQklok0kt-EpS5Uq09Mhh/p/10EM4k2v2MfIy1Vfr9j7B1qN_ReRC44QY/edit) • [💬 Get in Touch](#) • [⭐ Star this repo](#)

</div>

---

## 📜 License

This project is **open source and free to use** for both personal and commercial purposes.

---

## ❓ FAQ & Support

**Q: Is this free?**
- A: Yes! 100% free and open source.

**Q: Can I use it commercially?**
- A: Absolutely! No restrictions.

**Q: Do I need coding skills?**
- A: No! Just upload and click. The Gradio interface is super simple.

**Q: Will my images be uploaded to the cloud?**
- A: No! Everything runs locally (on your machine or Colab). No data is sent anywhere.

**Q: How accurate is the OCR?**
- A: 95%+ accurate on clear, standard text. Some minor corrections may be needed for fancy fonts.

---

## 🎉 Get Started Now!

You have **3 ways** to use this tool:

1. **🌐 Gradio Interface** - Click and upload (easiest!)
2. ☁️ **Google Colab** - Free GPU powered
3. 💻 **Local Machine** - Full control

**[Watch the demo →](https://www.youtube.com/watch?v=P_D-PXji0fc&t=261s)**

---

<div align="center">

### *Making Document Editing Effortless*

Because life's too short to manually retype text from images. 🚀

**[Back to Top ↑](#-editable-format-converter)**

</div>
