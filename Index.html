
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <meta charset="UTF-8">

<!-- Begin Jekyll SEO tag v2.8.0 -->
<title>The Walk Between Reality and Fantasy | Data Sprint on Generative AI and Fictionality</title>
<meta name="generator" content="Jekyll v3.10.0" />
<meta property="og:title" content="The Walk Between Reality and Fantasy" />
<meta property="og:locale" content="en_US" />
<meta name="description" content="Data Sprint on Generative AI and Fictionality" />
<meta property="og:description" content="Data Sprint on Generative AI and Fictionality" />
<link rel="canonical" href="https://ale66.github.io/the_walk/models/" />
<meta property="og:url" content="https://ale66.github.io/the_walk/models/" />
<meta property="og:site_name" content="The Walk Between Reality and Fantasy" />
<meta property="og:type" content="website" />
<meta name="twitter:card" content="summary" />
<meta property="twitter:title" content="The Walk Between Reality and Fantasy" />
<script type="application/ld+json">
{"@context":"https://schema.org","@type":"WebPage","description":"Data Sprint on Generative AI and Fictionality","headline":"The Walk Between Reality and Fantasy","url":"https://ale66.github.io/the_walk/models/"}</script>
<!-- End Jekyll SEO tag -->

    <link rel="preconnect" href="https://fonts.gstatic.com">
    <link rel="preload" href="https://fonts.googleapis.com/css?family=Open+Sans:400,700&display=swap" as="style" type="text/css" crossorigin>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="theme-color" content="#157878">
    <meta name="apple-mobile-web-app-status-bar-style" content="black-translucent">
    <link rel="stylesheet" href="/the_walk/assets/css/style.css?v=b41d6c8cd785aa785779b05640850988974d27b9">
    <!-- start custom head snippets, customize with your own _includes/head-custom.html file -->

<!-- Setup Google Analytics -->



<!-- You can set your favicon here -->
<!-- link rel="shortcut icon" type="image/x-icon" href="/the_walk/favicon.ico" -->

<!-- end custom head snippets -->

  </head>
  <body>
    <a id="skip-to-content" href="#content">Skip to the content.</a>

    <header class="page-header" role="banner">
      <h1 class="project-name">The Walk Between Reality and Fantasy</h1>
      <h2 class="project-tagline">Data Sprint on Generative AI and Fictionality</h2>
      
      
    </header>

    <main id="content" class="main-content" role="main">
      <h1 id="the-walk-between-reality-and-fantasy">The Walk Between Reality and Fantasy</h1>

<h2 id="data-sprint-on-generative-ai-and-fictionality">Data Sprint on Generative AI and Fictionality</h2>

<h1 id="fine-tuned-large-language-models-for-the-pnrr-fair-project">Fine-tuned Large Language Models for the PNRR-FAIR project</h1>

<p><sub><a href="/the_walk/models/">Home</a> | <a href="programme.md">Programme</a> | <a href="logistics.md">Logistics</a> | <a href="./models/film.md">Film</a></sub></p>

<p><strong>Technical report v. 2.1</strong></p>

<p>Prepared by G. Monti and A. Provetti, Network Centrality Labs and Birkbeck, University of London</p>

<h2 id="premise">Premise</h2>

<p>Generative AI is transforming the media landscape. Tools capable of producing synthetic text, images, video, and audio are rapidly diffusing across newsrooms, social platforms, and search engines. While these outputs fuel innovation and creativity, they also trigger profound uncertainty — especially around how we distinguish between truth and fabrication, reporting and fiction, evidence and illusion. These technological advancements interrogate Computational Social Science.</p>

<h2 id="description-of-work">Description of work</h2>

<p>This technical annex describes preparatory work done at Prof. E. Esposito’s request, in the context of the PNRR FAIR grant. We describe the end-to-end development of three bespoke Generative models trained on openly-accessible datasets in i) image generation (jewelry), ii) narrative, British (A. Christie) and American (HP Lovecraft) and iii) contemporary British newsarticles (The Guardian, public part of the site).</p>

<p>The project combines automated web-based data acquisition, LLM-powered metadata generation, and fine-tuning of a diffusion model using the DreamBooth LoRA method for Stable Diffusion XL. The outcome is a fully reproducible pipeline capable of producing high-fidelity images of historical jewellery in the stylistic tradition of museum photography.</p>

<h2 id="1-data-acquisition-from-the-victoria--albert-museum-api">1. Data Acquisition from the Victoria &amp; Albert Museum API</h2>

<p>The first stage consisted of programmatically harvesting museum-quality imagery from the Victoria &amp; Albert Museum (V&amp;A) API. A custom Python script was used to issue a targeted query for the keyword “Coronet”, selecting objects classified within the jewellery domain. The API returns structured metadata, including system identifiers, titles, summaries, and IIIF-based image access URLs. IIIF (International Image Interoperability Framework) facilitates standardised access to high-resolution cultural heritage images, making it particularly appropriate for dataset construction in digital humanities and computer vision research.</p>

<p>The script iterates through all records, parsing and validating metadata fields such as:</p>

<ul>
  <li><code class="language-plaintext highlighter-rouge">systemNumber</code> (unique identifier),</li>
  <li><code class="language-plaintext highlighter-rouge">_primaryTitle</code>,</li>
  <li><code class="language-plaintext highlighter-rouge">_summary</code>,</li>
  <li><code class="language-plaintext highlighter-rouge">_iiif_image_base_url</code> (image endpoint).</li>
</ul>

<p>For each item, the pipeline downloads the highest available resolution (up to 2500px width), ensuring that the dataset captures sufficient visual detail to represent metal textures, gemstones, engraving, filigree, and other material-specific features essential for high-quality generative modelling. Images are stored locally alongside a corresponding metadata JSONL file, which records filename, descriptive text, and source URL. This method produces a clean, machine-learnable corpus with reproducible provenance, consistent naming conventions, and uniform resolution.</p>

<p>This automated acquisition approach mirrors established principles in dataset curation for computational aesthetics and digital heritage, where systematically collected, labelled, and standardised images form the basis for generative or discriminative modelling.</p>

<h2 id="2-automated-caption-generation-using-gpt-41">2. Automated Caption Generation Using GPT-4.1</h2>

<p>Although the V&amp;A metadata is rich, its language varies widely in length, formality, and specificity. For generative model training, however, it is crucial to have consistent, descriptive captions focusing on the visible properties of each object. To produce a uniform caption set, the pipeline employs GPT-4.1 for computer-vision-guided automatic annotation.</p>

<p>Each image is first base64-encoded and then passed to the GPT-4.1 chat.completions endpoint with a structured instruction:</p>

<ul>
  <li>Identify material composition,</li>
  <li>Describe craftsmanship and construction,</li>
  <li>Note gemstone types and settings,</li>
  <li>Identify stylistic and historical cues,</li>
  <li>State overall physical condition,</li>
  <li>Prefix with a consistent template (“a high-quality photo of a real historical TOK jewellery piece…”).</li>
</ul>

<p>This ensures terminological cohesion, which is critical for diffusion-based training, where textual conditioning relies heavily on stable linguistic patterns.</p>

<p>The result is a <code class="language-plaintext highlighter-rouge">metadata_gpt4.jsonl</code> file containing pairs of <code class="language-plaintext highlighter-rouge">{file_name, caption}</code>, producing a harmonised training set in which each input image is aligned with a precise, factual, non-poetic descriptive caption. This is a form of synthetic annotation applied to cultural heritage images and aligns with recent research in multimodal representation learning, where large language–vision models provide expert-level labelling at scale.</p>

<h2 id="3-model-training-dreambooth-lora-for-stable-diffusion-xl">3. Model Training: DreamBooth LoRA for Stable Diffusion XL</h2>

<p>With both the image dataset and the caption file prepared, the next stage involved fine-tuning Stable Diffusion XL (SDXL) using DreamBooth LoRA. LoRA (Low-Rank Adaptation) is an efficient fine-tuning technique that injects a small set of learned layers into a pre-trained diffusion model without the computational overhead of full-model training. This approach preserves the general generative capabilities of SDXL while specialising its output domain toward museum-style jewellery photography.</p>

<p>Key design choices include:</p>

<ul>
  <li><strong>Base model:</strong> <code class="language-plaintext highlighter-rouge">stabilityai/stable-diffusion-xl-base-1.0</code></li>
  <li><strong>VAE fix:</strong> <code class="language-plaintext highlighter-rouge">madebyollin/sdxl-vae-fp16-fix</code></li>
  <li><strong>High-resolution input:</strong> 512×512 training images</li>
  <li><strong>Batching strategy:</strong> Small batch size with gradient accumulation</li>
  <li><strong>Mixed precision:</strong> FP16 for efficiency</li>
  <li><strong>SNR γ = 5.0:</strong> Helps stabilise noise-to-signal ratio during diffusion steps</li>
  <li><strong>Training steps:</strong> 2000 iterations, with checkpointing every ~700 steps</li>
  <li><strong>Optimiser:</strong> 8-bit Adam for memory reduction</li>
  <li><strong>Instance prompt:</strong> “a photo antique TOK jewellery”</li>
</ul>

<p>The training process embeds the visual characteristics of the curated dataset into the LoRA weights. The model gradually learns stylistic and material cues: metallic reflections, stone translucency, casting irregularities, patina, historical lighting setups, and the aesthetic conventions of catalogue photography. DreamBooth ensures identity preservation across concept variations, enabling the model to generalise from the dataset while maintaining stylistic fidelity.</p>

<p>This results in a lightweight LoRA file that can be merged or activated dynamically within SDXL pipelines, enabling downstream users to generate historically plausible jewellery images with detailed material realism.</p>

<h2 id="4-outcome-and-research-significance">4. Outcome and Research Significance</h2>

<p>The system developed here demonstrates a full pipeline for constructing a domain-specific generative model from scratch, integrating cultural-heritage data acquisition, multimodal caption synthesis, and targeted diffusion model fine-tuning.</p>

<p>The contributions are threefold:</p>

<ol>
  <li>A reproducible dataset pipeline enabling scalable collection of high-resolution museum jewellery images using open APIs.</li>
  <li>A synthetic caption generation method that leverages GPT-4.1 for precise, structured, descriptive annotations aligned with visual conditioning needs.</li>
  <li>A specialised generative model (SDXL LoRA) capable of producing museum-style images with stylistic and material fidelity.</li>
</ol>

<h3 id="image-comparison">Image Comparison</h3>

<p>Image 1 from the standard stable diffusion without LoRa, the second after the fine tuning.</p>

<p>The two images show the difference between a generic, untrained model and the same model after fine-tuning on museum ring photos.</p>

<p>Both images are generated from the same prompt “A high-quality photo of a real historical TOK bracelet crafted in engraved silver with interlocking geometric panels and a central oval red gemstone. Smooth, precise metalwork with subtle filigree edges. Authentic museum artifacts photographed in soft neutral light, showing texture, age, and refined craftsmanship.”</p>

<p>The use of a fictional word “TOK” helps the model to follow the additional added training.</p>

<p>The first jewelry image has flaws typical of an untrained diffusion model: the metal texture looks inconsistent, the shape is slightly distorted, and watermark-like artefacts appear because the base model imitates stock-photo patterns. The lighting is flat and not consistent with real museum catalogue photography.</p>

<p>The second image, produced after training, is noticeably more accurate. The watermark artefacts are gone, the engraving is sharper, and the gemstone reflects light more realistically. The overall illumination matches the neutral, controlled museum style used for archival documentation. The fine-tuned LoRA clearly learned the visual language of museum cataloguing, producing cleaner, more coherent, and more professional jewellery imagery.</p>

<h3 id="example-generation">Example Generation</h3>

<p>The model can follow semantically complex prompts:</p>

<blockquote>
  <p>A high-quality photo of a TOK real historical opal necklace featuring a pendant in a golden metal with a central blue stone. Detailed craftsmanship but smooth and geometric forms. Authentic museum object photographed in neutral lighting.</p>
</blockquote>

<p>Training code and usage example it can be found on this colab:
https://colab.research.google.com/drive/1HcHKwGRtTga8PtJewQX_YUUUc0QhOWDD?usp=sharing</p>

<p>The weights of the model can be found on HuggingFace.co or here:
https://drive.google.com/drive/folders/1bZtsh8awCpYiIGpz3AL2atPGoXgCLRin</p>

<hr />

<h2 id="a-lightweight-mixture-of-experts-moe-architecture-using-two-lora-fine-tuned-gemma-2b-models-for-stylistic-narrative-generation">A Lightweight Mixture-of-Experts (MoE) Architecture Using Two LoRA-Fine-Tuned Gemma-2B Models for Stylistic Narrative Generation</h2>

<p>This work presents a modular Mixture-of-Experts (MoE) architecture composed of two independently fine-tuned narrative-style models—<code class="language-plaintext highlighter-rouge">theoracle/agatha</code> and <code class="language-plaintext highlighter-rouge">theoracle/hplovecraft</code>—built on top of Google’s Gemma-2-2B-IT base model. The system uses Hugging Face Transformers, a keyword-based routing module, and LoRA adapters for parameter-efficient finetuning (PEFT). It demonstrates how specialised stylistic “experts” can be composed into a controllable, scalable, and interpretable generation framework without resorting to full multi-style training or large-scale model merging.</p>

<h2 id="1-technical-motivation">1. Technical Motivation</h2>

<p>Large language models (LLMs) often produce blended stylistic approximations when prompted for specific literary voices. This occurs because the model’s representation of style is distributed across many layers and not cleanly isolated. In contrast, parameter-efficient fine-tuning (PEFT) with LoRA allows the creation of small, targeted matrices that modify only a tiny subset of the base model’s parameters.</p>

<p>By training two separate LoRA adapters—one on a Lovecraft corpus, the other on an Agatha Christie dataset—you obtain true stylistic decoupling. Each adapter represents a standalone stylistic expert. No catastrophic forgetting occurs, because each model is fine-tuned independently and loaded dynamically rather than merged.</p>

<p>However, independent experts alone do not constitute a system. A controlling mechanism is required to decide which expert should respond to a given request. This need is addressed by the routing orchestrator.</p>

<h2 id="2-model-architecture">2. Model Architecture</h2>

<p>Each model follows the same underlying structure:</p>

<ul>
  <li><strong>Base model:</strong> <code class="language-plaintext highlighter-rouge">google/gemma-2-2b-it</code></li>
  <li><strong>Fine-tuning method:</strong> LoRA (rank; projection modules; lightweight adapters)</li>
  <li><strong>Training pipeline:</strong> Hugging Face AutoTrain Advanced</li>
  <li><strong>Task:</strong> Causal language modelling (not instruction-tuning)</li>
  <li><strong>Precision strategy:</strong> FP16 inference, INT4 quant during training (bitsandbytes)</li>
  <li><strong>Block size:</strong> 1024 context length</li>
</ul>

<p>The LoRA adapters target the Gemma model’s linear projection layers, allowing stylistic transformation without modifying the full 2B parameters. Each finetuned variant is therefore:</p>

<ul>
  <li>extremely small (typically under 300MB),</li>
  <li>fast to load,</li>
  <li>stackable (load base + selected adapter),</li>
  <li>easily swapped at inference time.</li>
</ul>

<p>This architecture is essential for a MoE system that selects one specialist per request.</p>

<h2 id="3-expert-1-lovecraft-model-cosmic-horror">3. Expert 1: Lovecraft Model (Cosmic Horror)</h2>

<p>The model can be found here https://huggingface.co/theoracle/hplovecraft</p>

<p>The Lovecraft expert was trained on the <code class="language-plaintext highlighter-rouge">TristanBehrens/lovecraftcorpus</code>, representing atmospheric horror, archaic diction, and cosmic dread. Its LoRA learns:</p>

<ul>
  <li>long, winding sentence structures,</li>
  <li>“forbidden knowledge” thematic templates,</li>
  <li>references to geometry, ruins, cults, and unknowable forces,</li>
  <li>narrative patterns typical of first-person confessional horror.</li>
</ul>

<p>Because the LoRA is trained purely on text continuation—not instruction templates—it responds strongly and directly to descriptive prompts.</p>

<h2 id="4-expert-2-agatha-christie-model-mystery--detective-prose">4. Expert 2: Agatha Christie Model (Mystery &amp; Detective Prose)</h2>

<p>The model can be found here https://huggingface.co/theoracle/agatha</p>

<p>The Agatha Christie expert uses the <code class="language-plaintext highlighter-rouge">realdanielbyrne/AgathaChristieText</code> dataset.</p>

<p>Technically, its LoRA emphasises:</p>

<ul>
  <li>short, clear sentence orchestration,</li>
  <li>domestic British settings,</li>
  <li>logical clue structuring,</li>
  <li>psychological tension in dialogue,</li>
  <li>pacing constraints consistent with Golden-Age mystery writing.</li>
</ul>

<p>Its training objective is identical to the Lovecraft expert, ensuring symmetric behaviour and comparable performance characteristics.</p>

<h2 id="5-the-orchestrator-a-simple-but-effective-routing-layer">5. The Orchestrator: A Simple but Effective Routing Layer</h2>

<p>Your Python code implements a deterministic, keyword-based router that selects the correct expert model for any request. Although simple, this choice offers three key technical advantages:</p>

<h3 id="51-interpretability">5.1 Interpretability</h3>

<p>The selection criteria (“lovecraft”, “cthulhu”, “mystery”, “agatha”) are visible and auditable. This transparency is critical for predictable stylistic control.</p>

<h3 id="52-zero-latency-overhead">5.2 Zero latency overhead</h3>

<p>Unlike a neural gating layer (used in large MoE LLMs like Mixtral), the keyword router adds no inference cost.</p>

<h3 id="53-avoiding-model-merging">5.3 Avoiding model merging</h3>

<p>Instead of merging LoRAs—often leading to style bleed—you load only the required LoRA at runtime:</p>

<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="n">pipe</span> <span class="o">=</span> <span class="n">pipeline</span><span class="p">(</span><span class="s">"text-generation"</span><span class="p">,</span> <span class="n">model</span><span class="o">=</span><span class="n">model_name</span><span class="p">)</span>
</code></pre></div></div>

<p>This ensures that only one expert modifies the base model at a time, preserving stylistic purity.</p>

<h2 id="6-prompt-assembly-and-continuation-strategy">6. Prompt Assembly and Continuation Strategy</h2>

<p>The orchestrator also normalises the user request:</p>

<ul>
  <li>extracts the “beginning” text block,</li>
  <li>prepends a unified instruction,</li>
  <li>ensures prompt formatting is consistent even with free-form user input.</li>
</ul>

<p>This step is crucial for causal LMs, which do not rely on system messages or chat templates.</p>

<p>Example assembled prompt:</p>

<blockquote>
  <p>Continue the following story in the style requested:
They sat alone in the darkened room as rain hammered…</p>
</blockquote>

<p>This standardisation increases coherence and reduces perplexity spikes across models.</p>

<h2 id="7-why-this-system-qualifies-as-a-mixture-of-experts">7. Why This System Qualifies as a Mixture-of-Experts</h2>

<p>Although it does not implement a neural gating mechanism, your system satisfies the structural definition of an MoE:</p>

<ol>
  <li>Multiple specialised experts trained on disjoint corpora.</li>
  <li>A routing function that selects the expert based on user intent.</li>
  <li>Dynamic switching of parameter-efficient adapters at inference time.</li>
  <li>Separation of stylistic knowledge, avoiding interference or forgetting.</li>
</ol>

<p>This is the classical engineering definition of MoE (mixture controlled by an external gating mechanism), not the deep-learning definition used in large sparse transformers.</p>

<h2 id="8-technical-benefits">8. Technical Benefits</h2>

<p>The the implementation presented here offers several advantages:</p>

<ul>
  <li><strong>Scalability:</strong> New styles can be added simply by adding new LoRA adapters + new routing keywords.</li>
  <li><strong>Low compute footprint:</strong> A Gemma-2B base model + small LoRAs is lightweight enough for CPU or small GPU inference.</li>
  <li><strong>Isolation of style:</strong> Each literary mode remains pure and uncontaminated.</li>
  <li><strong>Maintainability:</strong> The model list and routing function can be extended without retraining.</li>
  <li><strong>User-controllability:</strong> Writers can force a style or let the router choose automatically.</li>
</ul>

<h2 id="9-conclusions">9. Conclusions</h2>

<p>This two-expert Mixture-of-Experts narrative generator demonstrates how PEFT + modular routing can achieve precise stylistic conditioning without large-scale training or model blending. By pairing two Gemma-2B-IT LoRA adapters with a transparent Python orchestrator, the system delivers clean stylistic output, low inference cost, and easily extensible architecture. It shows the practical value of MoE principles for creative-writing applications and provides a solid foundation for future expansions—such as adding more experts, upgrading the router to semantic parsing, or building a unified front-end for real-time narrative generation.</p>

<h3 id="figure-1">Figure 1</h3>

<p><img src="/the_walk/models/images/prompt-1.jpeg" alt="" /></p>

<p>Using the same prompt we can see we can see the different styles. The orchestrator can choose the style according to the user preference. In this case H.P. Lovecraft</p>

<h3 id="figure-2">Figure 2</h3>

<p>The same prompt but with the Agatha Christie style, here we can clearly see the output with a different narrative style.</p>

<p><img src="/the_walk/models/images/prompt-2.jpeg" alt="" /></p>

<h1 id="getting-started">Getting started</h1>

<h2 id="a-the-video-tutorial">A the video tutorial</h2>

<p><a href="/the_walk/models/PNRR-FAIR-howto.mp4">Watch the video</a></p>

<h2 id="fiction-generation">Fiction generation</h2>
<p>Example Jupyter notebooks are available on Google Colab:</p>

<p>Narrative:</p>

<p><a href="https://colab.research.google.com/drive/14tMxXR3ssGLcubdp_Lh7xwPoe7dvNZNy?usp=sharing">https://colab.research.google.com/drive/14tMxXR3ssGLcubdp_Lh7xwPoe7dvNZNy?usp=sharing</a></p>

<p>Jewlery:
<a href="https://colab.research.google.com/drive/1TCWfoOFXIVgYIXT2_dxNLE1gmRsp3FwI?usp=sharing">https://colab.research.google.com/drive/1TCWfoOFXIVgYIXT2_dxNLE1gmRsp3FwI?usp=sharing</a></p>

<h2 id="access-credentials">Access Credentials</h2>

<p>user: <code class="language-plaintext highlighter-rouge">networkcentralitylabs@gmail.com</code></p>

<p>password: <code class="language-plaintext highlighter-rouge">Gabrprov!23</code></p>

<p>Hugging Face keys:</p>

<h2 id="journalism">Journalism</h2>

<p>Try out the model fine-tuned on The Guardian articles:</p>

<p><a href="https://colab.research.google.com/drive/1vKaLsXBlnH1H0I8YyOL8yq6ylky14QCM?usp=sharing">colab.research.google.com/drive/1vKaLsXBlnH1H0I8YyOL8yq6ylky14QCM?usp=sharing</a></p>

<p>A real article that reports about an actual event: <em>the firing of the Miami Dolphins coach Mike McDaniel after missing the playoffs for the second season in a row.</em></p>

<p><a href="https://www.theguardian.com/sport/2026/jan/08/dolphins-fire-mike-mcdaniel-after-missing-playoffs-for-second-season-in-row">www.theguardian.com/sport/2026/jan/08/dolphins-fire-mike-mcdaniel-after-missing-playoffs-for-second-season-in-row</a></p>

<p><img src="/the_walk/models/images/example-news.png" alt="" /></p>

<div class="language-text highlighter-rouge"><div class="highlight"><pre class="highlight"><code>The Miami Dolphins have fired head coach Mike McDaniel after the team missed the playoffs for the second straight season.

“After careful evaluation and extensive discussions since the season ended, I have made the decision that our organization is in need of comprehensive change,” Dolphins owner Stephen Ross said in a statement on Thursday.

“I love Mike and want to thank him for his hard work, commitment, and the energy he brought to our organization. Mike is an incredibly creative football mind whose passion for the game and his players was evident every day. 
I wish him and his family the best moving forward.”

The move is somewhat of a surprise after McDaniel told reporters on Monday that he was part of the team’s search for a new general manager.

The Dolphins went 35-33 under McDaniel, reaching the playoffs in his first two seasons but losing in the first round each time. 
Miami missed the postseason in 2024 after being eliminated by the Jets in the regular-season finale. 
This season, their postseason hopes ended with a loss to Pittsburgh in Week 15, ensuring their 25-year playoff-win drought – the longest streak in the NFL – would continue.

Miami parted ways with longtime general manager Chris Grier at the end of October and began their search for a new general manager this week. 
But a disjointed finish to the season that saw former first-round pick Tua Tagovailoa benched proved the final straw for Ross, who decided to move on from McDaniel.

The Yale-educated McDaniel was seen as emblematic of a generation of young, ambitious head coaches when he was appointed by the Dolphins at the age of 38 in 2022. 
He had impressed the Dolphins with his work as offensive coordinator of the San Francisco 49ers and soon turned around a sputtering Miami offense. 
In his first season in charge, the Dolphins finished sixth in total offense and were first the following season.

However, that momentum has stalled and Tagovailoa has struggled mightily among injuries and a loss of form. 
On Monday, Taglovailoa said he would be happy to play for a new team next season.

“That would be dope,” he said. “I would be good with it.”
</code></pre></div></div>

<div class="language-python highlighter-rouge"><div class="highlight"><pre class="highlight"><code><span class="n">replication_prompt</span> <span class="o">=</span> <span class="s">"""
    Miami Dolphins have fired their head coach Mike McDaniel.

    The team missed the playoffs for the second straight season.

    Their record under McDaniel was 35-33.

    McDaniel was young and well educated: appointed at the age of 38 in 2022 he studied in Yale.

    Stephen Ross is the Dolphins owner and said:
    'After careful evaluation and extensive discussions since the season ended, I have made the decision that our organization is in need of comprehensive change'

    He also said: 'I love Mike and want to thank him for his hard work, commitment, and the energy he brought to our organization. Mike is an incredibly creative football mind whose passion for the game and his players was evident every day. I wish him and his family the best moving forward.'

    Tua Tagovailoa is the former first-round pick quarterback who was benched this season.

    He said on Monday that he would be happy to play for a new team next season.

    He said: 'That would be dope. I would be good with it.'
"""</span>
</code></pre></div></div>

<h1 id="conversations-with-the-character">Conversations with the character</h1>

<p>Please see the <em>persona</em> model <a href="https://huggingface.co/ylliprifti/documentary-personas">huggingface.co/ylliprifti/documentary-personas</a></p>

<p>More details are in the <a href="/the_walk/models/film.html">film</a> section.</p>

<h2 id="collective-final-report">Collective final report</h2>

<p>Please click here to write your part:</p>

<p><a href="https://docs.google.com/document/d/1Um0gbjf-8qk9UnYVvcyF7a9zsOmH2V-j5zmYev-rcLI/edit?usp=sharing">docs.google.com/document/d/1Um0gbjf-8qk9UnYVvcyF7a9zsOmH2V-j5zmYev-rcLI/edit?usp=sharing</a></p>

<hr />

<p><em>Network Centrality Labs</em><br />
<em>For PNRR-FAIR Alma Mater University of Bologna</em></p>


      <footer class="site-footer">
        
        <span class="site-footer-credits">This page was generated by <a href="https://pages.github.com">GitHub Pages</a>.</span>
      </footer>
    </main>
  </body>
</html>
