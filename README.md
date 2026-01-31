# RICCE Fiction Engineering Prompt Suite

## 🧠 RICCE Fiction Prompt Suite (Claude / GPT Compatible)

Welcome to the **RICCE Prompt Engineering Toolkit** — a modular suite of creative prompt files designed for fiction grounded in deep character psychology, symbolic layering, and stylistic emulation (notably in the voice of **Stephen King** and other high-intensity literary voices).

This toolkit is optimized for use with:

- Claude (Anthropic, Code Interpreter & Pro)  

- ChatGPT (Custom GPTs + File Memory)  

- Obsidian (YAML metadata + prompt chaining)  

- Local prompt workflows (e.g., GitHub Copilot, notebooks, VS Code)

---

## 🎯 GOAL

To support emotionally resonant fiction writing through modular tools for:

- Character development , psychology 
- Nonlinear story assembly
- Scene refinement  
- Thematic reinforcement 
- Symbolic layering, coherence 
- Structural reorganization  
- Voice adaptation  
- Ritual scenes 
- Transformation events

---

### ASSISTANT MAP / FILE STRUCTURE

🗂️ dustandashes/
└📁 RICCE_PROMPTS/
    ├── character_extractor_v1.prompt
    ├── scene_outline_sk_style.prompt
    ├── evaluate_scene_v1.md
    ├── refine_scene_v1.md
    ├── scene_reduction_pass.md
    ├── foreshadow_strengthener.md
    ├── symbolism_tracker.md
    ├── theme_consistency_checker.md
    ├── retheme_pass.md
    ├── scene_to_summary.md
    ├── pov_shift_utility.md
    ├── scene_mirror_generator.md
    ├── voice_style_transfer.md
    ├── chronology_extractor.md
    ├── scene_slotter.md
    ├── ritual_inserter.md
    ├── threshold_scene_generator.md
    ├── tension_graph_generator.md
📁 system/
    ├── RICCE_HEADER.md
    ├── system_instructions.md
└ README.md ← you are here

--- 

### 🧩 PROMPT MODULE DESCRIPTIONS

|   |   |
|---|---|
|File|Purpose|
|system_instructions.prompt|Sets global assistant behavior and Stephen King emulation|
|RICCE_HEADER.md|Core RICCE framework (Role, Input, Context, Constraints, Evaluation)|
|character_extractor_v1.prompt|Extracts traits, motivations, contradictions from scenes|
|scene_outline_sk_style.prompt|Outlines stories in Stephen Kingâ€™s emotional structure|
|evaluate_scene_v1.md|Critiques scenes for resonance, tension, and clarity|
|refine_scene_v1.md|Polishes scenes based on evaluations and voice preservation|
|scene_reduction_pass.md|Trims prose for tension, pacing, and readability|
|foreshadow_strengthener.md|Adds or enhances subtle foreshadowing cues|
|symbolism_tracker.md|Detects and classifies symbols, metaphors, and motifs|
|theme_consistency_checker.md|Evaluates theme coherence across scenes|
|retheme_pass.md|Alters the emotional or thematic tone of a scene|
|scene_to_summary.md|Converts scenes into structured narrative breakdowns|
|pov_shift_utility.md|Transforms scene point of view while preserving tone|
|scene_mirror_generator.md|Builds reverse-echo scenes for narrative symmetry|
|voice_style_transfer.md|Adapts a scene into another authorâ€™s stylistic voice|
|chronology_extractor.md|Reconstructs implied timeline from fragmented scenes|
|scene_slotter.md|Tags scenes by structure, act, theme, or emotional function|
|ritual_inserter.md|Generates or integrates ritual or ceremonial scenes|
|threshold_scene_generator.md|Constructs pivotal liminal scenes of transformation|
|tension_graph_generator.md|Maps beat-level emotional or narrative tension curves|

---

### 🔁 RECOMMENDED USAGE FLOW

Below is a high-level loop for iterative fiction creation:

1. **Planning & Extraction →**
   character_extractor_v1
   scene_outline_sk_style

2. **Drafting →**
   ritual_inserter
   threshold_scene_generator
   pov_shift_utility

3. **Evaluation →**
   evaluate_scene_v1
   symbolism_tracker
   tension_graph_generator
   scene_to_summary

4. **Refinement →**
   refine_scene_v1
   scene_reduction_pass
   retheme_pass
   foreshadow_strengthener
   voice_style_transfer

5. **Structural Assembly →**
   theme_consistency_checker
   scene_mirror_generator
   scene_slotter
   chronology_extractor

6. **Revision Loop →**
   Repeat 3–5 as needed

---

## METADATA GUIDANCE 

### 🔹 Standard RICCE Prompt Metadata Block

Here’s a base YAML front-matter template I recommend for all .md or .prompt files in your suite:

---
title: "scene_slotter"
version: 1.0
type: "utility"              # ["generator", "refiner", "evaluator", "utility"]
function: "Tags a scene by narrative role, emotional function, and thematic purpose"
input_type: "scene"
output_type: "structural tags"
role: "Narrative Analyst"
style_profile: "Stephen King / Literary Horror"
theme_support: true
supports_chaining: true
intended_chain_position: "Post-generation / Pre-assembly"
related_prompts:
  - scene_to_summary
  - symbolism_tracker
  - chronology_extractor
date_created: 2026-01-29
---

### 🔸 Suggested Fields

|   |   |
|---|---|
|Field|Description|
|title|File name or prompt name|
|version|For iteration tracking|
|type|One of: generator, refiner, evaluator, utility|
|function|One-sentence summary of what it does|
|input_type / output_type|Describes prompt interface contract|
|role|The â€œactorâ€ or perspective of the assistant|
|style_profile|Authorial or stylistic mode used|
|theme_support|Does it handle or detect themes?|
|supports_chaining|Is it usable in sequence with others?|
|intended_chain_position|Where in the workflow it fits best|
|related_prompts|Other files this one should link to or follow|
|date_created|Optional but useful for lifecycle tracking|

### 📂 Where to Put It

- Always as the first block in the file, before any prose or instructions
- Use --- delimiters above and below (as shown)
- In Obsidian, this makes the prompt queryable with plugins or filters
- In Claude, GPT, GitHub, or VS Code, it becomes part of structured tooling

---

## 🔧 USAGE TIPS (Claude, Obsidian, GPT)

- Store each .md or .prompt file with clear YAML front-matter for tool chaining
- Claude/GPT: load file contents directly and reference modularly
- Obsidian: use metadata to query by type, theme_support, or chain_position
- Can be extended for genre shifts, non-linear storytelling, or author mimicry

---

## 🛠️ CUSTOMIZATION IDEAS

Want to expand the suite? Consider:

- arc_tracker.md — Maps emotional arcs by character
- dialogue_realism_checker.md — Ensures subtextual, in-character speech
- symbol_to_theme_inverter.md — Reinterprets recurring symbols
- ritual_architect.md — Builds full ritual frameworks by culture, theme, or transformation type

---

## 🧠 CUSTOMIZATION / CLAUDE INTEGRATION TIPS

- Each .md or .prompt file is designed to be modular and stackable
- Claude’s memory/context length is ideal for 1–2 chained prompts at once
- For Claude Code Interpreter: store each prompt as a file and pass dynamically
- For Obsidian: add frontmatter + folder tags to link scenes to tools
- You can build prompt variations (e.g., refine_for_pacing, symbolism_by_theme) from base modules

---

## 🛠️ FUTURE EXPANSION IDEAS

Consider creating additional tools such as:
- theme_consistency_checker.md
- scene_mirror_generator.md (reverse echo scenes)
- voice_style_transfer.md (from King to Morrison, McCarthy, etc.)
- tension_graph_generator.md (plot pacing across acts)

---

## 📚 LICENSE

This toolkit is for creative development, research, and experimental fiction writing. Attribution appreciated for shared versions.

---

## ✨ BUILT WITH RICCE

This suite follows the RICCE framework:
1. Role
2. Input
3. Context
4. Constraints
5. Evaluation

To ensure precision, tone, and narrative integrity at every step of your creative process.
