# Apple Developer Academy Portfolio
## vodkavelvet

---

## Executive Summary

I'm a developer with a passion for bringing ideas to life across different domains—from interactive game engines to intelligent systems. My journey spans game development, software engineering, and machine learning, each phase building on the lessons of the previous one. Through hands-on projects, I've developed strong problem-solving skills, learned to work with complex systems, and discovered how to apply emerging AI techniques to solve real-world problems.

---

## Projects

### 1. Tea Disease Detection Using YOLO (Computer Vision / Research)

**Repository:** [github.com/vodkavelvet/yolo-tea-disease](https://github.com/vodkavelvet/yolo-tea-disease)

**Project Type:** Research & Computer Vision Model Benchmark  
**Status:** Active | Multi-model Comparison Study  
**My Role:** Solo Developer & Researcher

#### Summary
A comprehensive benchmark comparing three YOLO object detection models (YOLOv8, YOLO11, YOLO26) for detecting nine different tea leaf diseases and pest infestations. The project evaluates model performance across precision, recall, mAP scores, and inference speed to identify the best model for real-world agricultural applications.

#### Detected Disease Classes
- Algal Spot, Brown Blight, Gray Blight
- Healthy Leaf (baseline)
- Helopeltis Pest, Red Rust
- Red Spider Mite Infestation
- Red Spot, White Spot

#### Key Findings & Impact
- **YOLOv8m**: Highest recall (0.796) and mAP50 (0.737) — best for minimizing missed detections
- **YOLO11m**: Best precision (0.715) and compact size (39 MB) — ideal for production & edge deployment
- **YOLO26m**: Edge-optimized with NMS-free inference — designed for low-power devices
- Trained on 100 epochs, 640×640 image resolution with SGD optimizer
- Dataset sourced from Roboflow (9 disease classes, standardized YOLO format)

#### What I Learned
- How to structure multi-model ML experiments reproducibly on Kaggle
- The trade-offs between model accuracy, size, and inference speed
- Working with computer vision pipelines: preprocessing → training → evaluation → comparison
- Importance of precision & recall for different use cases (detecting diseases = high recall priority)
- How to document research findings with clear metrics and visualizations

#### Technical Stack
- **Models:** YOLOv8, YOLO11, YOLO26 (Ultralytics YOLO framework)
- **Platform:** Kaggle for training infrastructure
- **Tools:** Python, Jupyter, confusion matrices, precision-recall curves
- **Dataset:** Roboflow (multi-format, version-controlled)

#### Status
✅ Complete with comparison metrics, trained weights, and inference scripts

---

### 2. AI News Generator (AI / Software Product)

**Repository:** [github.com/vodkavelvet/ai-news-generator](https://github.com/vodkavelvet/ai-news-generator)

**Project Type:** Full-Stack AI Application  
**Status:** Active | Production-Ready  
**My Role:** Full-Stack Developer

#### Summary
A full-featured web application that generates professional news articles using real-time web scraping and a local large language model (Qwen2.5-3B). The system combines modern web scraping, API design, and LLM inference to create contextually accurate news across nine categories with multiple writing tones.

#### Key Features
- **Real-time Web Scraping:** Multi-source news aggregation from Indonesian news outlets
- **Local LLM Inference:** Qwen2.5-3B GGUF model (Q4_K_M quantization) running locally without external API dependencies
- **Professional Article Structure:** Automatically generated H1/H2/H3 formatted articles
- **Multiple Writing Styles:** Formal, Casual, Urgent, Analytical tones
- **Smart Caching:** Performance optimization to reduce redundant processing
- **Modern Dark-Themed UI:** Responsive frontend with real-time generation feedback

#### Impact & Use Cases
- Demonstrates integration of web scraping, AI inference, and UI design
- Solves the problem of manually writing news articles at scale
- Production-ready API (FastAPI) with clear endpoint documentation
- Achieves ~20-25 second article generation time on consumer hardware
- Processing speed: ~15-25 tokens/sec (Apple M4 performance)

#### What I Learned
- Full-stack development: backend (FastAPI), frontend (HTML/CSS/JavaScript), AI integration
- How to run large language models locally with GGUF quantization
- Web scraping best practices: rate limiting, source validation, error handling
- System design: caching, API architecture, real-time status feedback
- Balancing model inference speed with quality (3B parameter model for local execution)

#### Technical Stack
- **Backend:** FastAPI 0.104.1 (Python 3.9-3.13.5)
- **Frontend:** HTML5, CSS3, Vanilla JavaScript (responsive dark theme, ~42KB CSS, ~20KB JS)
- **AI Model:** Qwen2.5-3B Instruct (llama-cpp-python inference)
- **Web Scraping:** BeautifulSoup4, feedparser, requests
- **ML/NLP:** transformers, torch, custom NER pipeline

#### API Endpoints
- `POST /generate` — Generate news article with keyword, category, tone, length
- `GET /validate-sources/{keyword}` — Check available news sources
- `GET /health` — System health status

#### Status
✅ Complete with working web interface, API documentation, and deployment-ready code

---

### 3. Ice Side Scroll (Game Development / 2D Platformer)

**Repository:** [github.com/vodkavelvet/ice-sideScroll](https://github.com/vodkavelvet/ice-sideScroll)

**Project Type:** 2D Game (Side-Scrolling Platformer)  
**Status:** Complete | Playable  
**My Role:** Solo Game Developer (Design, Programming, Systems)

#### Summary
A fast-paced 2D side-scrolling platformer set in a frozen world. Players navigate through challenging ice physics, avoiding obstacles and mastering slippery terrain. The game emphasizes reflexes and strategic movement, with increasing difficulty across levels.

#### Core Gameplay Mechanics
- Smooth, responsive platforming with realistic ice physics
- Progressive difficulty curve
- Engaging level design balancing exploration and challenge
- Atmospheric soundtrack to enhance immersion
- WASD/Arrow Keys for movement, Spacebar for jumping

#### Impact
- Demonstrates understanding of game physics and player feedback loops
- Shows ability to design and implement engaging game mechanics
- Illustrates how constraints (ice physics) create interesting design spaces
- Complete playable game from concept to implementation

#### What I Learned
- Game engine fundamentals: physics, collision detection, state management
- Player experience design: controls feel responsive, difficulty progression
- How environmental mechanics (ice physics) shape gameplay
- Level design principles: pacing, difficulty curves, visual clarity
- Importance of playtesting and iteration

#### Technical Stack
- **Engine:** Unity (C#)
- **Physics:** Built-in 2D physics with custom ice friction values
- **Audio:** Integrated soundtrack system
- **Platform:** Cross-platform (PC/Web build available)

#### Status
✅ Complete with playable levels, physics tuning, and deployed builds

---

### 4. Exterminator (Game Development / Action Shooter)

**Repository:** [github.com/vodkavelvet/exeterminator](https://github.com/vodkavelvet/exeterminator)

**Project Type:** 2D Game (Action Shooter)  
**Status:** Complete | Playable  
**My Role:** Solo Game Developer (Design, Programming, Game Systems)

#### Summary
An intense action shooter where players face endless waves of enemies with diverse weapons and power-ups. The game emphasizes quick reflexes, strategy in weapon selection, and progressive challenge scaling as enemy waves intensify.

#### Core Gameplay Features
- Non-stop action with wave-based enemy spawning
- Diverse weapon arsenal with upgrade system
- Stylized graphics with explosive visual effects
- Dynamic sound design heightening intensity
- Strategic gameplay: wave management, resource planning

#### Impact
- Demonstrates ability to implement complex game systems (waves, enemy AI, weapon balance)
- Shows understanding of player engagement through progressive challenge
- Illustrates effects design and visual feedback importance
- Complete combat game pipeline

#### What I Learned
- AI design for enemy behavior and wave scaling
- Weapon balance and progression systems
- Player feedback through effects (explosions, impacts, audio)
- UI design for fast-paced gameplay (ammo, score, wave count)
- Performance optimization for real-time rendering of many entities

#### Technical Stack
- **Engine:** Unity (C#)
- **Systems:** Enemy AI, wave management, weapon upgrade system
- **Graphics:** Particle effects, sprite animation
- **Audio:** Dynamic sound effects and background music
- **Platform:** Cross-platform deployment

#### Status
✅ Complete with full gameplay loop, weapon variety, and polish

---

## My Learning Journey

### Phase 1: Game Development Foundation (2D Games)
Started by building 2D games with Unity—learning core game development concepts through hands-on iteration: game loops, physics simulation, player feedback, and level design.

**Projects:** Ice Side Scroll, Exterminator

**Outcome:** Deep understanding of interactive systems, player experience, and iterative design.

---

### Phase 2: Software Engineering (Full-Stack Development)
Transitioned to building complete software products with modern architecture: APIs, web interfaces, system design, and real-world constraints.

**Project:** AI News Generator

**Outcome:** Experience building production-ready systems that integrate multiple technologies (backend, frontend, ML models).

---

### Phase 3: Machine Learning & Computer Vision (AI Research)
Moved into research-focused work with machine learning and computer vision, bringing together previous learnings to solve agricultural problems at scale.

**Project:** Tea Disease Detection Using YOLO

**Outcome:** Understanding of ML workflows, model evaluation, and applying AI to real-world problems.

---

## Skills Summary

### Technical
- **Game Development:** Unity, C#, 2D physics, game systems design
- **Web Development:** FastAPI, HTML5/CSS3/JavaScript, responsive UI
- **Machine Learning:** YOLO models, model evaluation, Kaggle workflows
- **Python:** FastAPI, data processing, AI pipelines, web scraping
- **Tools & Platforms:** Git/GitHub, Kaggle, Jupyter, BeautifulSoup, Ultralytics

### Design & Soft Skills
- **Problem Solving:** Breaking complex problems into manageable systems
- **Iterative Development:** Learning through building and testing
- **Documentation:** Clear README files, API documentation, project structure
- **Cross-Disciplinary:** Comfortable moving between game dev, software, and ML

### Learning Mindset
- Independently research and implement new technologies
- Learn from failure through playtesting and evaluation metrics
- Apply lessons from one domain to solve problems in another
- Balance perfectionism with shipping working solutions

---

## Why I'm Interested in Apple Developer Academy

Apple's Academy represents the intersection of my interests:
- **Product-Focused Development:** Building software that solves real problems (like AI News Generator)
- **Design Excellence:** Understanding how game design principles apply to all software (feedback, flow, intuition)
- **AI Integration:** Bringing intelligent systems to user-facing applications
- **Community & Learning:** Growing alongside developers focused on Apple ecosystem and innovation

I'm excited to deepen my skills in building products that combine intuitive design with technical sophistication.

---

## Contact & Links

**GitHub:** [github.com/vodkavelvet](https://github.com/vodkavelvet)

**Project Repositories:**
- Tea Disease Detection: [github.com/vodkavelvet/yolo-tea-disease](https://github.com/vodkavelvet/yolo-tea-disease)
- AI News Generator: [github.com/vodkavelvet/ai-news-generator](https://github.com/vodkavelvet/ai-news-generator)
- Ice Side Scroll: [github.com/vodkavelvet/ice-sideScroll](https://github.com/vodkavelvet/ice-sideScroll)
- Exterminator: [github.com/vodkavelvet/exeterminator](https://github.com/vodkavelvet/exeterminator)

---

**Portfolio Version:** 1.0  
**Last Updated:** September 2026  
**Status:** Active candidate for Apple Developer Academy
