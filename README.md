# AI-Based-Turbocharger-Identification

Master’s Thesis in Information Systems
AI-Based Turbocharger Identification for
Automated Model Recognition and Repair
Support
Ivana Peneva

In Maintenance, Repair, and Overhaul (MRO) environments, manual logging of indus-
trial part numbers is time-consuming and highly prone to human error. Reliable asset
tracking is needed, but its automation is severely hindered by nameplate degradation,
including oil, rust, and glare, alongside perspective distortions and the widespread use
of dot-peen engraving, which fundamentally breaks the continuous-stroke assumptions
of traditional Optical Character Recognition (OCR) systems. To address this issue, this
thesis develops and systematically evaluates an end-to-end computer vision pipeline
designed to extract Garrett turbocharger part numbers from heavily degraded name-
plates. The workflow integrates spatial preprocessing with advanced visual decoding
and a deterministic fuzzy-matching database engine. The findings demonstrate that
background removal, perspective rectification, and orientation correction are essential,
increasing overall system accuracy by over 34 percentage points while simultaneously
reducing token consumption. Furthermore, generative Multimodal Large Language
Models (MLLMs) vastly outperformed OCR engines, with the open-weight Qwen2-VL
architecture achieving a peak accuracy of 76.03% when deployed with an unconstrained
transcription strategy. Utilizing constrained prompts to directly extract the part number
severely degraded the reasoning capabilities. Through rigorous stress testing, the
pipeline’s operational limits were quantified. While the pipeline is resilient to global
speckle noise, its performance reaches a functional ceiling when deep physical scratches
that obscure more than one of the digits of the part number are present. Finally, an exe-
cution time analysis revealed a per-image processing time of approximately 55 seconds
on an NVIDIA L4 Tensor Core GPU (24 GB VRAM), identifying spatial preprocessing as
the primary computational bottleneck. Having a digitized, verified part number enables
automated model recognition, allowing technicians to seamlessly cross-reference the
specific replacement components and maintenance protocols required for repair.

The images used for the evaluation of this pipeline can be found at: https://drive.google.com/drive/folders/19FvcL3arSmjt3aKv8iXK9LLRcS-fugL7?usp=share_link
