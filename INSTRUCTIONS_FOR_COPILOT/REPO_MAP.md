# Slime Mold Repo Navigation Map

## Quick Reference

**Want species by visual vibe?**  
→ `/species/index.csv` - sortable by shape, color, texture

**Want lifecycle info?**  
→ `/lifecycle/plasmodial_lifecycle.md` (main dramatic cycle)  
→ `/lifecycle/cellular_lifecycle.md` (social amoeba choreography)  
→ `/lifecycle/stage_visual_traits/` (individual stage deep-dives)

**Want prompt templates?**  
→ `/prompt_system/prompt_templates.md`  
→ `/examples/` (naturalist, maximalist, horror, alien, mathy, fashion)

**Want visual language?**  
→ `/vocab/` (morphology, texture, color, motion terms)

**Want color schemes?**  
→ `/palettes/` (naturalist, neon, decay, jewel)

---

## File Organization Logic

### `/taxonomy/`
High-level groupings. Not exhaustive taxonomy - just enough to organize visually.

- `slime_mold_groups.md` - Plasmodial vs cellular vs protostelid overview
- `myxomycetes_orders.md` - Main plasmodial orders by visual family
- `dictyostelids_overview.md` - Social amoeba groups
- `protostelids_overview.md` - Tiny stalked minimalists

### `/lifecycle/`
Stage-by-stage breakdowns with visual traits.

**Main cycle files:**
- `plasmodial_lifecycle.md` - Spore → amoeba → plasmodium → fruiting
- `cellular_lifecycle.md` - Aggregation → slug → sorocarp
- `protostelid_lifecycle.md` - Simple stalk cycle
- `master_lifecycle_matrix.yml` - Cross-reference table

**Stage deep-dives in `/lifecycle/stage_visual_traits/`:**
- Plasmodial: spores, amoebae, swarm cells, zygote, plasmodium, vein networks, sclerotium, primordia, fruiting bodies (aethalia, pseudoaethalia, sporangia), capillitium, peridium, columella
- Cellular: aggregation streams, slug/grex, sorocarps, macrocysts, microcysts

### `/species/`
100+ species files organized by group.

**Structure:**
species/
├── index.csv          # Sortable master list
├── index.json         # Programmatic access
├── myxomycetes/       # 70+ plasmodial species
├── dictyostelids/     # 20+ cellular species
└── protostelids/      # 10+ tiny stalked species

**Each species file includes:**
- Taxonomy & common names
- Iconic lifecycle stages
- Color range, surface traits, structure traits
- Texture tags, mood tags
- Substrates
- Art translations (architecture, fashion, alien, material analogies)
- Render modes (macro, mutation, network, etc.)
- Related species

**Example:** `/species/myxomycetes/fuligo_septica.yml`

### `/vocab/`
Concrete sensory language libraries for building prompts.

- `morphology_terms.md` - Anatomical structures (capillitium, peridium, columella, etc.)
- `texture_terms.md` - Surface feels (mucus-slick, powder-dry, chalky, metallic-wet, etc.)
- `color_terms.md` - Specific hues (sulfur yellow, rust orange, iridescent violet, etc.)
- `motion_terms.md` - Movement patterns (pulse-streaming, aggregation, crusting, etc.)
- `substrate_terms.md` - Growth contexts (bark fissures, mulch, moss bed, etc.)
- `scale_terms.md` - Size language (pinhead jewel, hand-sized foam, cathedral-scale, etc.)
- `failure_mutation_terms.md` - Glitch aesthetics (collapsed fruiting, dried crust, hybrid forms)

### `/prompt_system/`
Templates and mixing rules for AI art generation.

- `prompt_templates.md` - Base structures (naturalist macro, maximalist mutation, mathy network, slug procession, etc.)
- `prompt_blocks.yml` - Modular components to mix/match
- `visual_dna_modules.md` - Core aesthetic building blocks
- `species_mix_rules.md` - How to combine species traits
- `lifecycle_mix_rules.md` - How to layer lifecycle stages
- `crossbreed_experiments.md` - Hybrid concepts (Arcyria + coral reef, Fuligo + diseased rococo, etc.)

### `/palettes/`
Pre-built color schemes.

- `naturalist_palettes.yml` - Documentary realism colors
- `neon_bioelectric_palettes.yml` - Bioluminescent mutation colors
- `rot_decay_palettes.yml` - Decomposition aesthetics
- `jewel_spore_palettes.yml` - Iridescent luxury colors

### `/environments/`
Substrate context descriptions.

- `bark.md` - Bark fissures, wet tannins, lichen neighbors
- `rotting_logs.md` - Decaying wood, fungi, moisture
- `leaf_litter.md` - Curled leaves, fine debris, humus
- `moss_beds.md` - Jewelbox microforest
- `mulch.md` - Suburban spawn point
- `dung.md` - Coprophilous habitats
- `cave_surfaces.md` - Pale ghost contexts
- `desert_crusts.md` - Arid outliers
- `aquatic_edges.md` - Semi-aquatic niches

### `/render_logic/`
Technical guidance for visual translation.

- `macro_photography.md` - Depth of field, condensation, spore dust
- `microscope_logic.md` - Cell-scale rendering
- `scale_exaggeration.md` - Pinhead → cathedral translation
- `translucency_and_wetness.md` - Subsurface scattering, edge glow, moisture
- `branching_networks.md` - Vein logic, routing systems, fractal growth
- `spore_dust_atmospherics.md` - Particle halos, release clouds
- `bioluminescent_interpretations.md` - Glow logic (even for non-luminescent species)

### `/datasets/`
Machine-readable aggregates.

- `species_minimum_100.yml` - Full species list
- `lifecycle_stage_matrix.csv` - Cross-reference of species → stages
- `habitats_and_substrates.csv` - Distribution data

### `/examples/`
Ready-to-use prompt packs.

- `prompts_naturalist.md` - Documentary macro photography style
- `prompts_maximalist.md` - Excessive detail, mutation, iridescence
- `prompts_horror.md` - Body horror, infection, grotesque
- `prompts_alien.md` - Xenobiology, planetary terrain
- `prompts_mathy.md` - Network graphs, routing systems, emergence
- `prompts_fashion_material.md` - Textile, jewelry, couture, material design

---

## Workflow Examples

### "I want to make slime mold architecture renders"
1. Pick species from `/species/myxomycetes/` with `art_translation` including "architecture"
2. Check `iconic_stages` - use plasmodium or aethalium for best structure
3. Pull from `/prompt_system/prompt_templates.md` - use "Maximalist mutation" template
4. Add environment from `/environments/rotting_logs.md` for substrate texture
5. Layer palette from `/palettes/jewel_spore_palettes.yml`

### "I want to animate cytoplasmic streaming"
1. Read `/lifecycle/plasmodial_lifecycle.md` - focus on plasmodium stage
2. Check `/lifecycle/stage_visual_traits/vein_networks.md` for structure
3. Use `/vocab/motion_terms.md` for animation language
4. Reference `/render_logic/branching_networks.md` for vein logic
5. Pick Physarum polycephalum from `/species/myxomycetes/` (most documented for streaming)

### "I want weird gothic metallic shit"
1. Filter `/species/index.csv` for `metallic` in surface_traits
2. Focus on Lamproderma, Stemonitis, Comatricha species
3. Use sporangia stage from `/lifecycle/stage_visual_traits/sporangia.md`
4. Pull from `/palettes/neon_bioelectric_palettes.yml` - iridescent blacks/purples
5. Apply `/examples/prompts_horror.md` templates

---

## Search Tips

**By visual archetype:**  
`grep "foam" species/index.csv`  
`grep "coral" species/index.csv`  
`grep "metallic" species/index.csv`

**By substrate:**  
`grep "bark" species/myxomycetes/*.yml`  
`grep "dung" species/dictyostelids/*.yml`

**By color:**  
`grep "yellow" species/myxomycetes/*.yml`  
`grep "iridescent" species/myxomycetes/*.yml`

**By mood:**  
`grep "grotesque" species/myxomycetes/*.yml`  
`grep "obscene" species/myxomycetes/*.yml`
