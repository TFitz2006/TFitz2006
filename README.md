# Thomas Fitzgerald

B.S.E. Computer Science & Engineering (Honors) + Mathematics at The Ohio State University, Class of 2028. I build high-performance systems and quantitative tools — currently a Software Engineer Intern at ECM PCB Stator Technology and a Research Assistant benchmarking clinical vision-language models on OSU's supercomputing cluster. Quantitative Analyst & VP of Internal Affairs at Scarlet Investment Group.

I'm passionate about AI safety and the responsibility of technology research to help more than it hurts.

## Featured Projects

### [Limit Order Book Simulator](https://github.com/TFitz2006/limit-order-book-simulator)

`C++20` `Python` `pybind11` `CMake`

A price-time-priority matching engine with a market-making simulator on top — built to answer two questions: how fast can a single-threaded book go, and does inventory-aware quoting measurably reduce risk?

- **9.4M msgs/sec sustained** through a realistic 60/30/10 add/cancel/aggressive mix (10M messages, Apple M1 Pro), p50 add latency **83 ns**
- **97.8% PnL variance reduction** from simplified Avellaneda–Stoikov quote skewing vs. a symmetric baseline, across 100 paired-seed simulations
- Cache-first design: contiguous vector-of-levels book, intrusive FIFO queues, object-pool allocation (zero heap in the hot path), open-addressing hash map for O(1) cancels
- Correctness before speed: scenario suite + differential testing against a naive reference matcher, per-operation book invariants in debug builds, CI on Linux and macOS

### [IMC Prosperity 4 — SIG Quant Team](https://github.com/TFitz2006/IMC-4-SIGQuant)

`Python` `pandas` `matplotlib`

Team codebase for the IMC Prosperity 4 algorithmic trading competition.

- Product-specific market-making strategies (fixed-fair-value and drift-aware quoting) with iterative experiment tracking across official runs
- Custom interactive order-book visualizer: depth-level toggles, official-run P&L overlays, trade inspection, and time/price zooming for post-round analysis

### [JamaScrape](https://github.com/TFitz2006/JamaScrape)

`Python` `Selenium` `Streamlit`

Data infrastructure for my research assistantship at OSU studying cognitive bias in clinical vision-language models.

- Selenium pipeline that scrapes JAMA Network articles into a structured local library of Markdown, figures, and metadata — the foundation of a 2,000+ case clinical benchmark used to evaluate models like Qwen2.5-VL and Gemma 3
- Streamlit search-and-reader app so the research team can query and read the full library offline, with batch re-scraping, resume support, and image handling built in

---

## Other Projects

| Project | What it is |
|---|---|
| [Energy Analytics Dashboard](https://github.com/TFitz2006/BDAA---Hackathon-Osu-Energy-Analytics) | Full-stack React/TypeScript dashboard over Databricks SQL flagging anomalous OSU building energy usage with weather-aware context — Data I/O Hackathon |
| [MLB Prop Model](https://github.com/TFitz2006/Fliff-Scraper-MLBPLayerPropModel) | Scrapes sportsbook player-prop odds with Selenium, projects lines from MLB Stats API data, and ranks props by model edge |
| [FEH Robot — Team Mechamaru](https://github.com/TFitz2006/FEHRobot) | C++ control code for our team's autonomous course-navigating robot — OSU Fundamentals of Engineering Honors competition |
| [Foundations 2 Study Guide Game](https://github.com/TFitz2006/Foundations2-StudyGuide-Game) | Interactive study-guide game covering data structures & algorithms |
| [Environmental Man](https://github.com/TFitz2006/FEH-Enviromental-Man) | C++ arcade game built on the OSU FEH Proteus embedded simulator |

## Skills

**Languages:** C/C++ (C++20), Python, Java, SQL, MATLAB, TypeScript
**Frameworks & libraries:** React, Selenium, Hugging Face Transformers, pandas
**Tools & platforms:** Git/GitHub, Databricks, SLURM / HPC clusters, SSH
**Certification:** Bloomberg Market Concepts (BMC)

## Contact

[LinkedIn](https://www.linkedin.com/in/thomas-fitzgerald-36a603322) · thomas.fitzgerald112@gmail.com · fitzgerald.498@buckeyemail.osu.edu
