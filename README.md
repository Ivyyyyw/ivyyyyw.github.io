<!-- 🎯 改内容 → 去 content/ 文件夹
🎨 改样式 → 去 assets/css/ 或 layouts/ 文件夹
⚙️ 改配置 → 去 config/ 文件夹 -->

## 🎯 Content vs Style/Layout Separation

### 📄 **CONTENT EDITING** (What to show)
```bash
# Personal Information (Bio, Work, Education)
/Users/liuyiwei/my-site/content/authors/admin/_index.md

# Homepage Content & Block Configuration
/Users/liuyiwei/my-site/content/_index.md
  - News items content
  - Block order and basic settings
  - Container sizes (max-w-6xl, etc.)

# Publications Content
/Users/liuyiwei/my-site/content/publications/
  - conference-paper/index.md
  - journal-article/index.md
  - preprint/index.md

# Site Configuration
/Users/liuyiwei/my-site/config/_default/
  - hugo.yaml (site title, URL)
  - params.yaml (theme color, navbar settings)
  - menus.yaml (navigation menu items)
```

### 🎨 **STYLE/LAYOUT EDITING** (How to show)
```bash
# Custom CSS Styles
/Users/liuyiwei/my-site/assets/css/custom.css
  - Background colors
  - Font sizes
  - Custom styling overrides

# Block Templates (Layout & HTML Structure)
/Users/liuyiwei/my-site/layouts/partials/hbx/blocks/
  - news-custom/block.html (News section layout)
  - publications-custom/block.html (Publications section layout)
  - experience-custom/block.html (Experience section layout)
  - resume-biography-custom/block.html (Bio section layout)

# Page Templates (Individual Page Layouts)
/Users/liuyiwei/my-site/layouts/publications/
  - single.html (Individual publication page layout)
```

## 🔧 **Common Editing Tasks**

### ✏️ **To Change Content:**
- **Personal info**: Edit `content/authors/admin/_index.md`
- **News items**: Edit `content/_index.md` → news-custom → items
- **Publications**: Add/edit files in `content/publications/`
- **Menu items**: Edit `config/_default/menus.yaml`

### 🎨 **To Change Appearance:**
- **Colors/fonts**: Edit `assets/css/custom.css`
- **Block layouts**: Edit `layouts/partials/hbx/blocks/*/block.html`
- **Spacing between blocks**: Edit `content/_index.md` → design → spacing
- **Theme color**: Edit `config/_default/params.yaml` → color

## 📄 **Publication Pages**

### 🎯 **Individual Publication Layout**
```bash
/Users/liuyiwei/my-site/layouts/publications/single.html
```
**Purpose**: Custom template for individual publication pages (e.g., `/publications/conference-paper/`)

**Features**:
- ✅ **Custom Link Buttons**: Supports PDF, Code, Slides, Presentation, Dataset, Paper, Site
- ✅ **SVG Image Priority**: Automatically prefers `featured.svg` over PNG/JPG
- ✅ **Responsive Design**: Mobile-friendly layout with proper spacing
- ✅ **Dark Mode Support**: Full dark/light theme compatibility

**Supported Link Types** (in `content/publications/*/index.md`):
```yaml
links:
  - type: pdf           # 📑 PDF
  - type: code          # 💻 CODE  
  - type: slides        # 📝 SLIDES
  - type: presentation  # 🎤 PRESENTATION
  - type: dataset       # 📊 DATASET
  - type: paper         # 📄 PAPER
  - type: site          # 🌐 SITE
```

**Image Priority Order**:
1. `featured.svg` (vector, no processing)
2. `featured.png` (resized to 800px width)
3. `featured.jpg` (resized to 800px width)
4. `featured.jpeg` (resized to 800px width)
5. `featured.webp` (resized to 800px width)

## 🚀 **Development Commands**
```bash
# My environment
hugo version
hugo v0.150.1-ce44a8e835e6934292acda936e5b43b70f451af9+extended darwin/arm64 BuildDate=2025-09-25T10:26:04Z VendorInfo=gohugoio

# Start development server
hugo server -D --disableFastRender

# Build for production
hugo --minify
```
## 📁 **File Management**

### 📄 **CV/Resume**
```bash
/Users/liuyiwei/my-site/static/uploads/resume.pdf
```
### 🖼️ **Images & Media**
```bash
/Users/liuyiwei/my-site/content/authors/admin/avatar.png

/Users/liuyiwei/my-site/assets/media/icons/
  - nii_logo.png
  - axa_logo.png

/Users/liuyiwei/my-site/content/publications/conference-paper/featured.jpg
```
```

