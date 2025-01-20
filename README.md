# awesome-ai4ms-paper-and-websites

This repository is a collection of my thoughts, summaries, and reflections on literature, websites, and tutorials that explore the intersection of materials science and artificial intelligence.

## Directory
- [Preface](#preface)
- [LLM + Materials](#llm--materials)
  - [RAG](#rag)
  - [Agent](#agent)
  - [Knowledge distillation](#knowledge-distillation)
- [Materials with AI](#materials-with-ai)
  - [Properties Prediction](#properties-prediction)
  - [Knowledge Extraction](#knowledge-extraction)
- [Benchmark and Database](#benchmark-and-database)
  - [Materials Benchmark or Database](#materials-benchmark-or-database)
  - [AI-related Benchmark or Database](#ai-related-benchmark-or-database)
  - [Alloy Materials Benchmark or Database](#alloy-materials-benchmark-or-database)

# Preface

本仓库记录关于LLM (large language models)和AI/ML在材料科学中应用的文献，特别是关于LLM在材料中的应用。看过的文章会至少用一句话概括内容，有些还会有notes。只有标题的就是还没看过的，只是先存档到这里。

# LLM + Materials

## RAG
None

## Agent
None

## Knowledge distillation
1. 从零开始实现大模型知识蒸馏 -- Starting from scratch to achieve knowledge distillation of large models (Bilibili video Jan 2025) [[Link]](https://www.bilibili.com/video/BV1kQcoetEFM/?spm_id_from=333.1007.top_right_bar_window_custom_collection.content.click&vd_source=4c43a44b540724d9ab77627ff3efb406) 使用qwen2.5系列模型在特定任务上进行知识蒸馏，教师模型为qwen2.5-3b（qwen2.5-7b），学生模型为qwen2.5-0.5b，尝试只使用KL散度、微调学生模型加KL散度和不微调学生模型加交叉熵加KL散度等不同思路，并且使用了KL散度不同变种（反向KL散度，偏向前向KL散度，偏向反向KL散度）。反向 K2 散度优于前向 K2 散度,但仅仅微调学生模型准确度反而最好为80.3%。

# Materials with AI
## Properties Prediction
None

## Knowledge Extraction
1. Bridging AI and Science: Implications from a Large-Scale Literature Analysis of AI4Science (Arxiv Nov 2024) [[Paper]](https://arxiv.org/pdf/2412.09628) 大规模(159,295 papers)AI4S文献摘要分析。磁性材料，锂离子电池，钙钛矿太阳能电池是AI融合比较缺乏的领域。作者用文献训练了节点之间的link预测模型，传统的Node2Vec方法比较适合分析AI和Sci领域是否可能产生连接。

## Crystal structure
1. Progress in Deep Learning Crystal Structure Generation (Github repo) [[Link]](https://github.com/kdmsit/Awesome-Crystal-GNNs/tree/main)

# Benchmark and Database
- ## Materials Benchmark or Database
  | Name | Description | Link | Category |
  |---|---|---|---|
  | perovskitedatabase  | perovskitedatabase | https://github.com/Grenzlinie/perovskitedatabase | perovskite |
  | dlmatreview | software packages and databases used in deep-learning applications for materials science and engineering | https://github.com/deepmaterials/dlmatreview | 材料科学数据库和软件github仓库 |

- ## AI-related Benchmark or Database
  | Name | Description | Link | Category |
  |---|---|---|---|
  | SciAssess | Benchmarking LLM Proficiency in Scientific Literature Analysis | https://arxiv.org/abs/2403.01976 | 材料文本问答数据库 |
  | SciQAG | A Framework for Auto-Generated Science Question Answering Dataset with Fine-grained Evaluation | https://arxiv.org/abs/2405.09939 | 材料文本问答数据库 |
  | HoneyComb | A Flexible LLM-Based Agent System for Materials Science | https://aclanthology.org/2024.findings-emnlp.192/ | 材料Agent数据库 |
  | Bohrium | DeepMD and AI4S notebook square | https://bohrium.dp.tech/notebooks?notebookTab=recommendations | AI4S知识分享平台 |
  | LLM4Mat-Bench | Benchmarking Large Language Models for Materials Property Prediction | https://arxiv.org/abs/2411.00177 | LLM在材料科学知识的回答表现 |
  | MaScQA | investigating materials science knowledge of large language models | https://pubs.rsc.org/en/content/articlelanding/2024/dd/d3dd00188a | LLM在材料科学知识的回答表现 |

- ## Alloy Materials Benchmark or Database
| Source | Database name | Data Type | Availability | Datasize | Inclusion | Link |
|---|---|---|---|---|---|---|
| Calculation, Experiment | Thermodynamic database for the Co-Pr system | Co-Pr, Metal, thermodynamic properties | Direct Download, Free | 8 | 1. compositions for both as-cast and heat treated specimens. 2. the determined enthalpy of mixing of liquid phase. 3. thermodynamic database of the Co-Pr system in TDB format. | https://www.sciencedirect.com/science/article/pii/S2352340915004011 |
| Experiment | Data regarding the influence of Al, Ti, and C additions to as-cast Al0.6CoCrFeNi compositionally complex alloys on microstructures and mechanical properties | Al-Co-Cr-Fe-Ni, Grain Size, Mechanical Properties, Metal, XRD | Direct Download, Free | 5 | 1. Properties: mechanical data, XRD, phase composition, grain size | https://www.sciencedirect.com/science/article/pii/S2352340919310972#tbl1 |
| Experiment | Comprehensive data compilation on the mechanical properties of refractory high-entropy alloys | Mechanical Properties, Metal, Refractory Alloy, Yield Strength | Direct Download, Free | 122 | This data article presents the compilation of mechanical properties for 122 refractory high entropy alloys (RHEAs) and refractory complex concentrated alloys (RCCAs) reported in the period from 2010 to the end of January 2018. 1. Properties: density, Young Modulus, Equilibrium Conditions, Single/MultiPhase Materials, Present Phase, Tension/Compression, Testing Temperature, Yield Strength. | https://www.sciencedirect.com/science/article/pii/S2352340918312885 |
| Experiment | Benchmark dataset of the effect of grain size on strength in the single-phase FCC CrCoNi medium entropy alloy | Cr-Co-Ni, EBSD Maps, Mechanical Properties, Metal, Microstructure maps, Yield Strength | Direct Download, Free | 16 | Microstructural data available in the present paper are backscattered electron micrographs for sixteen different grain sizes. Also available are pdf reports of grain size analysis (annealing twin boundaries were neglected) and crystallite sizes (including annealing twin boundaries) as well as data describing the number of annealing twin boundaries per grain (n), corresponding Taylor factors (M) and average annealing twin thicknesses (t). Additionally, raw data of stress-strain curves at five different temperatures [77 K, 293 K, 473 K, 673 K and 873 K] are given for all sixteen grain sizes. Mechanical data such as yield stresses (σ0.2%), Hall-Petch parameters (σ0 and ky) and critical boundary strengths (τc) are provided along with a 1D discrete dislocation dynamics (1-D DDD) simulation results concerning the different boundary strengths. | https://www.sciencedirect.com/science/article/pii/S2352340919309473 |
| Experiment | Data compilation on the effect of grain size, temperature, and texture on the strength of a single-phase FCC MnFeNi medium-entropy alloy | Grain Size, Metal, Mn-Fe-Ni | Direct Download, Free | 1 | 1. Properties: (i) raw backscatter electron (BSE) micrographs (tif-files) obtained using a scanning electron microscope (SEM) for nine different grain sizes with four images for each grain size and (ii) pdf reports and tables shown below presenting the distributions of the grain- (d, accounting for grain boundaries only) and crystallite- (c, which accounts for both grain and annealing twin boundaries) sizes and of the annealing twin thicknesses (t). | https://www.sciencedirect.com/science/article/pii/S235234091931162X |
| Experiment | Hardness data related to pre-ageing, natural secondary ageing, and paint bake hardening in Al-Mg-Si alloys | Al-Mg-Si, Hardness, Metal | Direct Download, Free | 1 | 1. Properties: Hardness data in different process and temperature. | https://www.sciencedirect.com/science/article/pii/S2352340919308492 |
| Experiment | Characterization data of an (AlFeNiTiVZr)1-xCr x multi-principal element alloy continuous composition spread library | Al-Fe-Ni-Ti-V-Zr-Cr, Metal, Raman Spectral, XRD | Direct Download, Free | 7 | 1. Properties: x-ray diffraction and Raman spectral | https://www.sciencedirect.com/science/article/pii/S2352340921000421 |
| Experiment | Data supporting the hierarchically activated deformation mechanisms to form ultra-fine grain microstructure in carbon containing FeMnCoCr twinning induced plasticity high entropy alloy | EBSD Maps, Fe-Mn-Co-Cr, High-entropy Alloy, Metal, SEM, TEM, XRD | Direct Download, Free | 2 | 1. Properties: SEM, TEM, STEM, EBSD images, Stress-strain curves. | https://www.sciencedirect.com/science/article/pii/S2352340922002633#sec0002 |
| Experiment | Dataset of a thermal model for the prediction of temperature fields during the creation of austenite/martensite mesostructured materials by localized laser treatments in a Fe-Ni-C alloy | Fe-Ni-C, Metal, thermodynamic properties | Direct Download, Free | 20 | 1. laser processing parameters and material thermal properties | https://www.sciencedirect.com/science/article/pii/S2352340923002299#sec0002 |
| Experiment | Data analysis for investigating the tribological behaviors of aluminum-silicon alloys | Al-Si, Hardness, Mechanical Properties, Metal, elastic module, wear rate | Direct Download, Free | 2 Types | 1. Two types Aluminum-silicon alloy 2. Properties: hardness, wear rate, friction coefficient, and compression elastic module 3. Work Condition data: stirring time, casting temperature, type of nanoparticles, and ageing heat treatment | https://www.sciencedirect.com/science/article/pii/S2352340922004620#sec0003 |
| Experiment | Analyzing experimental data from reciprocating wear testing on piston aluminum alloys, with and without clay nano-particle reinforcement | Al-based with other elements, Metal, Wear | Direct Download, Free | 2 Types | 1. Two types piston aluminum alloy. 1. Properties: Weight, Wear Rate, the Friction Coefficient. 2. Work Condition data: Force, Velocity, Reinforcement. |  |
| Calculation, Experiment | Refractory high entropy alloy dataset with room temperature ductility screening | Ductility, Hardness, High-entropy Alloy, Metal | Direct Download, Free | 82 | 1. This dataset contains 82 unique refractory alloys experimentally synthesized via arc melting and subject to screening tests for hardness and room temperature ductility. 2. Properties: Solidus(melting point, predicted by Thermo-Calc), Hardness, Ductility Ranking(0-5) | https://www.sciencedirect.com/science/article/pii/S2352340922007892#abs0001 |
| Experiment | Small dataset for hot cracking susceptibility of Al alloys and Ni alloys using dynamic X-ray radiography (DXR) technique | Al based alloy, Metal, XRD | Direct Download, Free | 10 | Here, using the DXR technique we characterized the hot cracking formation in Laser Powder Bed Fusion (L-PBF) process for ten commercial alloys (Al7075, Al6061, Al2024, Al5052, Haynes 230, Haynes 160, Haynes X, Haynes 120, Haynes 214, and Haynes 718). | https://www.sciencedirect.com/science/article/pii/S2352340923001683#abs0001 |
| Literature | Fatigue database of complex metallic alloys | Fatigue, Metal, Multi-principal alloy | Direct Download, Free | 272 | 272 fatigue datasets of S-N (the stress-life relation), ε-N (the strain-life relation), and da/dN-ΔK (the relation between the fatigue crack growth rate and the stress intensity factor range) data | https://figshare.com/articles/dataset/Fatigue_database_of_complex_metallic_alloys/23007362 https://www.nature.com/articles/s41597-023-02354-1#code-availability |
| Experiment | Elastic modulus data for additively and conventionally manufactured variants of Ti-6Al-4V, IN718 and AISI 316 L | Al-Si, Mechanical Properties, Metal, Shear Modulus, Young’s modulus | Direct Download, Free | 3 | 1. properties: temperature-dependent elastic properties (Young’s modulus, Shear modulus) of Ti-6Al-4V, Inconel IN718, and AISI 316 L | https://www.nature.com/articles/s41597-023-02387-6 |
| Literature | Dataset of mechanical properties and electrical conductivity of copper-based alloys | Copper based alloy, Mechanical Properties, Metal | Direct Download, Free | about 1830 | 1. properties: composition and processing route, and targets, including properties such as hardness, yield strength, ultimate tensile strength, and electrical conductivity | https://www.nature.com/articles/s41597-023-02411-9 |
| Literature | Expanded dataset of mechanical properties and observed phases of multi-principal element alloys | Grain Size, Hardness, Mechanical Properties, Metal, Multi-principal alloy, Percent Elogation, Utimate Tensile Strength, Yield Strength | Direct Download, Free | about 630 | 1. properties: alloy • oxygen content • carbon content • nitrogen content • yield strength • elongation • ultimate strength • hardness • density • grain size • observed phases | https://www.nature.com/articles/s41597-020-00768-9 https://citrination.com/datasets/190954/show_files/ |
| Experiment | Database on the mechanical properties of high entropy alloys and complex concentrated alloys | High-entropy Alloy, Mechanical Properties, Metal, Percent Elogation, Yield Strength, elastic module | Direct Download, Free | about 370 | 1. 370 structures of alloy. 2. properties: density, hardness, yield strength, breaking stress, elogation, elastic modulus. | https://www.sciencedirect.com/science/article/pii/S2352340920311100 |
| Experiment | Nickel-based Superalloys Databases | Metal, Ni, thermodynamic properties | Charged, Only in website | \ | thermodynamic and properties database designed for use with different kinds of Ni-based alloys and superalloys. | https://thermocalc.com/products/databases/nickel-based-alloys/ |
| Experiment | Yield strength of alloys dataset | Al-Co-Cr-Fe-Ni, Co-Fe-Ni-Si, Metal, Yield Strength, thermodynamic properties | Direct Download, Free | 160 | 1. Different compositions of alloy like: CoFeNiSi0.75, AlCoCrFeNi. 2. 5 properties of each composition: lattice constant, melting point, mixing enthalpy, atomic radii, melting temperature. | https://www.kaggle.com/datasets/arnabk123/yield-strength-of-alloys-dataset |
| Experiment | EBSD Dataset of the Alpha and Beta Phase Orientations for Hot-rolled Ti-6Al-4V | EBSD Maps, Metal, Ti-Al-V | Direct Download, Free | 27 | 1. This is an EBSD dataset for hot-rolled Ti-6Al-4V alloy. It includes the EBSD maps of the starting material, and materials have been rolled at nine different temperatures (825°C, 865°C, 895°C, 915°C, 935°C, 950°C, 960°C, 975°C, 1020°C) to three reductions (50%, 75%, and 87.5%). Each rolled material was sampled from transverse direction (TD) and rolling direction (RD) and EBSD maps were taken from both directions. | https://zenodo.org/record/6554355 |
| Experiment | Microstructure of Ti-3Mo alloy after solid solution treatments | Metal, Microstructure maps, Ti-Mo | Direct Download, Free | 10 | 1. This dataset depicts the microstructure of Ti-3Mo at% after solid solution treatment. | https://data.mendeley.com/datasets/mcf4wyjdz5/1 |
| Experiment | In situ synchrotron x-ray radiography data - Laser spot melting of pure nickel | Metal, Ni, XRD | By Email | \ | 1. XRD data of pure nickel | https://data.mendeley.com/datasets/bfr7fygm9h/1 |
| Literature | Crystal orientation characterisation of electrodeposited nanocrystalline nickel alloy | EBSD Maps, Metal, Ni, Ni-Fe | By Email | \ | 1. The collection contains EBSD maps of annealed nanocrystalline Ni and Ni-Fe alloys. The maps show the variation of crystallographic texture across mesoscale colonies within these alloys. | https://dro.deakin.edu.au/articles/dataset/Crystal_orientation_characterisation_of_electrodeposited_nanocrystalline_nickel_alloy/21088363/1 |
| Literature | International High Temperature Alloy Conference: Nickel Base High Temperature Alloy Dataset | Chinese Data, Metal, Ni, material composition, performance information | By Email | \ | Based on the International Symposium on Superalloys from 1980 to 2016, data such as material grade and name, material composition, raw material information, performance information, and experimental conditions were recorded using manual reading and pixel value conversion methods. | https://www.scidb.cn/en/detail?dataSetId=633694461158752256# |
| Calculation | Navigating the Ti-C-O and Al-C-O ternary systems through theory-driven discovery | Al-C-O, Metal, Phase Map, Ti-C-O | Direct Download, Free | 2 | 1. We map out for the first time the full phase stability of Ti-C-O and Al-C-O compounds using first-principles calculations, through simple, effcient and highly parallel random structure searching in conjunction with techniques based on complex network theory. | https://archive.materialscloud.org/record/2021.201 |
| Calculation | The JuHemd (Jülich-Heusler-magnetic-database) of the Monte Carlo simulated critical temperatures of the magnetic phase transition for experimentally reported Heusler and Heusler-like materials | Heusler and Heusler-like materials, Metal, Transition Temperature, magnetic phase transition type | Direct Download, Free | 700 Systems | a collection of the magnetic phase transition types and transition temperatures (Tc) for experimentally documented Heusler and Heusler-like materials, as found by density functional calculations augmented by the Monte Carlo method, and as reported by experiment in the literature. | https://archive.materialscloud.org/record/2022.28 |
| Calculation | Spatiotemporal prediction of microstructure evolution with predictive recurrent neural network | Fe-Cr-Co, Metal, Microstructure Transition | Direct Download, Free | \ | we used a dataset from spinodal decomposition simulation of FeCrCo alloy created by the phase-field method for training and predicting future microstructures by previous observations. The results show that the trained network predicts quantitatively accurate microstructure morphologies while it is several orders of magnitude faster than the phase field method. | https://archive.materialscloud.org/record/2022.156 |
| Calculation | Database including T=1000C yield strength and specific yield strength predictions for over 10 million BCC high entropy alloys | Mechanical Properties, Metal, Yield Strength | Direct Download, Free | 10m | 1. computed the high-temperature (T=1300K) yield strength based on solute strengthening of over 10 million alloys within the whole Al-Cr-Mo-Nb-Ta-V-W-Hf-Ti-Zr alloy family. Also the yield strength/density has been computed. 2. Database including T=1000C yield strength and specific yield strength predictions for over 10 million BCC high entropy alloys. | https://archive.materialscloud.org/record/2021.65 https://www.sciencedirect.com/science/article/abs/pii/S1359645419306755?via%3Dihub |
| Calculation, Experiment | Designing crystallization to tune the performance of phase-change memory: rules of hierarchical melt and coordinate bond | AEM, Metal, Phase, Resistance, TEM | Direct Download, Free | \ | Two Folders: In Figure 2 subfolder, there are six subfolders. As following: Figure 2a is an experiment about the temperature dependence of resistance (R-T curves); Figure 2b is an experiment about resistance thermal failure; Figure 2c is the test of the SET-RESET windows of the phase-change memory; Figure 2d is the test of power consumption, and it contains the data of the resistance dependence of pulse current and the voltage waveform capture by the oscilloscope; Figure 2e is the endurance of the devices; Figure 2f shows a large amount of statistical data, which is the phase change speed measured after different melting time(100ns, 500ns, 1000ns, 5000ns). In Figure 3a-d subfolder, there are two subfolders. As following: Figure 3a is the transmission electron microscope image, and it can be open using Gatan DigitalMicrograph software; Figure 3b-d are the distribution of three elements via the atom-resolved energy-dispersive X-ray spectroscopy(EDX), and it can be open using Analysis Program software. | https://www.nature.com/articles/s41467-021-26696-9 |
| Calculation | Origin of high strength in the CoCrFeNiPd high-entropy alloy | Co-Cr-Fe-Ni, Elastic Constants, Metal | Direct Download, Free | 15 | The VASP calculations of CoCrFeNi and CoCrFeNiPd elastic constants. | https://archive.materialscloud.org/record/2020.0045/v1 |
| Literature | High-throughput calculations of catalytic properties of bimetallic alloy surfaces | Catalyst Properties, Metal, Organic | Direct Download, Free | 90000 | We present a large dataset of adsorption of H, C, N, O and S onto more than 2,000 metallic and bimetallic alloy surfaces, consisting of approximately 90,000 DFT calculations performed in Quantum Espresso. The alloys are constructed from all possible combinations of 37 metals into AB and A3B stoichiometries, in the L1_0 and L1_2 structures respectively, where the 37 metals in the A1 structure are included as well. Slabs are cleaved along the 111 facet for A1 and L1_2 and along the 101 facet for L1_0, and all possible adsorption sites are sampled. In addition to the monoatomic adsorbates, adsorption of CH, CH2, CH3, NH, NH2, OH, H2O and SH is sampled for a smaller subset of alloys. | https://archive.materialscloud.org/record/2019.0015/v1 |
| Literature | Aluminum alloy compositions and properties extracted from a corpus of scientific manuscripts and US patents | Al-based with other elements, Mechanical Properties, Metal, Percent Elogation, Utimate Tensile Strength, Yield Strength | Direct Download, Free | 14884+1278 | 1. Present two datasets: - chemical composition, and - mechanical properties for predominantly wrought aluminum alloys. The first dataset contains 14,884 entries on aluminum alloy compositions extracted from academic literature and US patents using text processing techniques, including 550 wrought aluminum alloys which are already registered with the Aluminum Association. The second dataset contains 1,278 entries on mechanical properties for aluminum alloys, where each entry is associated with a particular wrought series designation, extracted from tables in academic literature. 2. Properties: Yield Strength, Utimate Tensile Strength, Percent Elogation | https://archive.materialscloud.org/record/2021.200 |
| Literature | Fatigue database of high entropy alloys | Fatigue, Grain Size, High-entropy Alloy, Metal, Utimate Tensile Strength, Yield Strength | Direct Download, Free | 66 | 1.The database is subdivided into three categories, i.e., low-cycle fatigue (LCF), high-cycle fatigue (HCF), and fatigue crack growth rate (FCGR), which contains 15, 23, and 28 distinct data records, respectively. 2.Each data record in any of three categories is characteristic of a summary, which is comprised of alloy composition, key fatigue properties (yield strength, ultimate tensile strength), and additional information influential to or interrelated with fatigue (e.g., material processing history, phase constitution, grain size, uniaxial tensile properties, and fatigue testing conditions), and an individual dataset, which makes up the original fatigue testing curve. | https://archive.materialscloud.org/record/2022.11 |
| Literature | Dataset for fracture and impact toughness of high-entropy alloys | High-entropy Alloy, Metal, Toughness | Direct Download, Free | 154 | Data of K_1c, J_1c(partly), Synthesis Condition, Phase, Process History, Measurement Standard, etc.. | https://archive.materialscloud.org/record/2022.171 |
| Calculation | Machine learning-enabled high-entropy alloy discovery | DFT Properties, Fe-Ni-Co-Cr-V-Cu, Metal | Direct Download, Free | 699 | 1. Fe-Ni-Co-Cr-V-Cu multi-principal elements compositions 2. compositions’ 15 properties(atomic + DFT, mainly focus on Thermal Expansion Coefficient) | https://github.com/ziyuanrao11/Machine-learning-enabled-high-entropy-alloy-discovery |
| Literature | Journal: Scientific Data | All Type |  |  | Dataset collection journal | https://www.nature.com/sdata/ |
| Literature | Journal: Data in brief | All Type |  |  | Dataset collection journal | https://www.sciencedirect.com/journal/data-in-brief |
| Calculation, Experiment, Literature | Atomly | All Type | By Python Crawler, Free | \ | structure and property data for materials | https://atomly.net/#/matdata |
| Experiment, Literature | ICSD (https://www.psds.ac.uk/icsd) | All Type | Charged, Only in website | \ | Crystal Structure Data |  |
| Calculation, Experiment, Literature | Google Dataset Search | All Type | By API, By Email, By Python Crawler, Charged, Direct Download, Free | \ | 1. it’s just a search website, not specific dataset. | https://datasetsearch.research.google.com/ |
| Literature | Materials Cloud | All Type | Direct Download, Free | 22m | 1. It’s an archive to store dataset from paper. 2. Just Type “Metal” or “Alloy” to search related database. | https://www.materialscloud.org/home#statistics |
| Calculation, Experiment, Literature | NOMAD | All Type | By API, Free | 13m | 1. Uploaded by personal user 2. Many kinds of strucutre and properties data but the value is empty. | https://nomad-lab.eu/prod/rae/gui/search |
| Calculation | JARVIS-DFT, JARVIS-FF | All Type | By API, Free | 56k | 1. structure: space group, formation energy, primitive cell, conventional cell, density, volume. 2. properties: xrd, band gap, dos, magnetic moment, poisson ratio, anisotropy ratio, optolectric properties(semi-local), Finite-difference elastic constant-tensor. | https://jarvis.nist.gov/jarvisdft/ |
| Calculation | AFLOW(Automatic Flow for Materials Discovery) | All Type | By API, Free | 3530k | 1. a globally available database of 3,530,330 material compounds with over 734,308,640 calculated properties, and growing. 2. properties: structure, bader charges, magnetic properties(atom magnetic moment, magnetization cell, magnetization atom), Band Structure, DOS, thermaldynamic properties(total energy, enthalpy atom) | https://www.aflowlib.org/ |
| Calculation, Literature | OQMD (open quantum materials database) | All Type | By API, Direct Download, Free | 1022k | 1. Compositions with different space group, crystal structure, total energy, band gap, volume 2. Stability, ΔH, Decomposition Energy, Competing Phases, Experimental formation energy 3. Phase map of multiple elements materials.(eg: https://oqmd.org/materials/composition/Ni-Ti-Al) | https://oqmd.org/ |
| Calculation, Experiment, Literature | Materials Project | All Type | By API, Free | 154k | https://next-gen.materialsproject.org/materials/mp-16514?elements=Ni%2CAl 1. Properties: Structure(lattice, space group, density, dimension), Thermodynamics Stability(energy above hull, formation energy, predict stable label, etc.), Band Structure, Phonon Dispersion, Diffraction Pattern(xrd, electron diffraction), Aqueous Stability, Magnetic Properties, Elastic Constans, X-ray Absorption Spectra, Charge Density, Suggested Substrates, Contributed Data 2.Experiment Tool: Generate Phase Diagram, Synthesis Explorer(Chemical Reaction) | https://next-gen.materialsproject.org/ |
| Calculation | C2DB | 2D Materials | By Email, Free | 4000 | 1. The database contains structural, thermodynamic, elastic, electronic, magnetic, and optical properties of around 4000 two-dimensional (2D) materials distributed over more than 40 different crystal structures. | https://cmr.fysik.dtu.dk/c2db/c2db.html |
