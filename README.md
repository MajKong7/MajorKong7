# James Finn

**Software engineer building private, local AI systems** — LLM inference, retrieval, and agentic orchestration that run entirely on hardware the client controls.

🌐 [veniceinference.com](https://veniceinference.com)

---

## A few things about me

### Systematic futures — the Turtle lineage

For nearly 30 years I was the lead developer and chief operator for Paul Rabar — one of the original Turtles trained by Richard Dennis in the 1980s experiment that proved systematic trading could be taught. We traded short-, medium-, and long-term systems measured in days, derived from daily price/time series. Rabar managed about $90M when I started and roughly $800M at its peak.

I built essentially the entire stack behind the program: account, portfolio, and price management; trade processing; order generation; the simulations; and the parameter sets, market/system weights, and account weights — the crown jewels.

The simulators searched for robust systems two ways. *Brute force* swept a defined set of parameter combinations, then a second program extracted the dense, high-performing "neighbor" clusters. *Genetic* search covered a far larger parameter space, finding those same robust clusters as it went.

Accuracy was enforced structurally. We grew from one research group — Paul, a mathematician, another Turtle we collaborated with, and me — to three in three locations: mine; two Fermilab physicists and an engineer in the Chicago office; a mathematician and a programmer on the East Coast. No group shared code. Every idea was re-implemented independently and cross-checked before any large run.

And I made the final daily call on whether orders were good to go — which meant our live positions matched simulation exactly. Every discrepancy was run down and resolved; a rounding error had to actually *be* a rounding error.

### From the metal up

I ran Rabar's mission-critical infrastructure end to end — selecting, administering, and maintaining all of it, including 150 rack servers I installed and maintained at a USC colo — while writing, debugging, and running nearly all of our C/C++, C#, and SQL. I introduced databases into research and production back in 1992.

### Security

A parallel track since I read *The Cuckoo's Egg* in 1989 — for years my browser homepages were stacked with comp-sec sites for a steady daily read. I went hands-on with Backtrack/Kali, Cain & Abel, and the like around 2013. More recently: wiring up exploit chains like EternalBlue/DoublePulsar in an isolated home lab, working PicoCTF challenges, and rooting 14 machines on Hack The Box.

### AI & LLM inference

My first LLM work was at BigBear AI — RAG applications and a C/C++ OpenVINO/ONNX inference-optimization engine. More recently I built **BDS (Batch Document Search)**, a private RAG platform on a PySide6 / FastAPI architecture with hybrid ChromaDB retrieval (BGE + BM25, fused via RRF and cross-encoder re-ranking), GLiNER entity extraction, and a knowledge-graph output that repairs 98.2% of its wikilinks on a 100-document baseline.

I've benchmarked inference backends — vLLM and llama.cpp — for sustained local serving. On a Windows 10 host running WSL2 (Ubuntu 24.04), llama.cpp proved the more stable under continuous load, avoiding the GPU-wedge failures that bit the alternative. Current experiment: agentic orchestration with Hermes/Gemma.

---

🌐 [veniceinference.com](https://veniceinference.com) · 📫 jf.technical@outlook.com
