---
layout: post
title: "Evolution Is Holding Biology Back. Here's How AI Can Fix That."
date: 2026-02-26 12:00:00
description: What if the greatest barrier to biological innovation isn't our technology — but 4 billion years of evolutionary baggage?
tags: synthetic-biology AI evolution bioengineering
categories: essays
featured: true
---

Life on Earth is ancient, and that's a problem.

Over four billion years, evolution has relentlessly shaped every organism on this planet — not to be elegant or efficient, but simply to *survive*. And survival is a messy, compromise-laden business. The result is biology that is remarkably robust, but riddled with inefficiencies that frustrate anyone trying to engineer it for industrial use.

I've been thinking about this friction — between what evolution produced and what engineers need — and about whether generative AI might finally let us escape it.

---

## The Tax You Never Knew You Were Paying

There's a concept in evolutionary biology called the Red Queen Hypothesis, named after the chess piece in *Through the Looking-Glass* who must run as fast as she can just to stay in the same place. In nature, species don't evolve to become *better* in any absolute sense — they evolve to stay competitive against other species that are also constantly changing. It's an arms race with no finish line.

This constant pressure leaves a mark on biology that I think of as the **Red Queen Tax**: a kind of evolutionary overhead that shapes every organism on Earth, and not always in ways that are useful to us.

The tax shows up in three ways:

**Sub-optimality.** Natural enzymes work beautifully in the specific conditions where they evolved — but change the temperature, the pH, or the solvent, and they fall apart. They're not optimized for your industrial bioreactor; they're optimized for a cell that lived 500 million years ago. Evolution has no concept of "scalable" or "cost-efficient."

**Redundancy and complexity.** Biological systems are layered with backup mechanisms, regulatory circuits, and "dark matter" — non-coding DNA, parallel pathways, fail-safes built on top of fail-safes. This makes organisms resilient in nature. For engineers, it's a nightmare: the more you understand one part of a cell, the more tangled everything else becomes.

**Path dependency.** This is perhaps the deepest constraint. Life on Earth didn't start from a blank slate and optimize toward perfection. It started with whatever random chemistry worked 4 billion years ago, and everything since has been an incremental modification of that. We're not working with optimally designed biology — we're working with the accumulated consequences of every evolutionary accident in the history of life.

Here's the irony: our greatest bioengineering breakthroughs — CRISPR, heat-stable polymerases from hot springs bacteria, viral vectors repurposed for gene therapy — came from mining exactly this "dark matter." Weird, seemingly redundant, or adversarial biology turned out to be incredibly useful when we understood it on its own terms.

What if we could search that space *systematically*, rather than waiting for serendipitous discovery?

---

## Two Kinds of Unexplored Biology

I've been working on a framework for exploring biological design spaces that evolution never reached — or once reached and then abandoned. There are two distinct directions worth pursuing.

**Lost Earth evolution** looks backward. Life before the Last Universal Common Ancestor (LUCA) — the hypothetical ancestor of all life on Earth — was almost certainly more diverse than anything alive today. Early Earth was a biochemical experiment in progress, with metabolic strategies, genetic mechanisms, and protein architectures that were later outcompeted and lost. Some of those extinct pathways may have had properties we'd find extraordinarily useful: catalytic mechanisms that modern enzymes don't use, energy-harvesting strategies we haven't seen, structural motifs that were abandoned not because they were bad, but because the competition moved in a different direction.

Molecular archaeology — reconstructing ancient proteins from genomic fossils — has already given us hints. But the data is fragmentary. The question is whether AI can learn enough from those fragments to fill in the gaps.

**Cosmic evolution** looks outward — or more precisely, sideways into hypothetical space. Life on Earth evolved in liquid water, near a particular kind of star, using a specific handful of the elements on the periodic table. But the universe is vast, and there's no particular reason those constraints should define all possible biology. What would biochemistry look like in liquid methane at -180°C? What proteins could fold and function under crushing pressures, or in environments drenched in ionizing radiation? Earth's extremophiles — organisms that thrive in volcanic vents, hypersaline lakes, and acidic hot springs — suggest that life is more flexible than our standard model implies. Generative AI, trained on the principles underlying these organisms, could extrapolate much further.

Neither "lost" nor "cosmic" biology is about science fiction. It's about systematically exploring the parts of biological design space that natural selection on Earth never had occasion to visit.

---

## What Makes This Possible Now

The thing that makes this more than speculation is the recent maturation of **generative AI for biology**.

Traditional computational biology is largely a prediction problem: given a sequence, predict a structure or function. Generative AI inverts this. Given a desired function — or even a desired set of environmental constraints — generate sequences likely to achieve it. Models like AlphaFold changed what we know about existing proteins; generative protein design models are starting to create proteins that don't exist in nature at all.

The crucial advantage for this kind of research is that generative models can learn from sparse data. There's no complete fossil record of Precambrian biochemistry, and we obviously have no samples of Titan life. But if you can characterize what you *do* know — extremophile genomes, paleoprotein reconstructions, theoretical biochemistry — a generative model can interpolate and extrapolate into the unknown in principled ways.

Think of evolution as the world's longest-running optimization algorithm — one that ran for billions of years but was constrained to a tiny corner of the possible space by the specific conditions of early Earth. Generative AI is a way to run that algorithm in silico, unconstrained by historical accidents, across environments that never existed, toward objectives that natural selection has no way to optimize for.

---

## The Cosmic Virtual Bioreactor

The computational architecture I've been developing for this work is what I'm calling the **Cosmic Virtual Bioreactor** (CVB). The name is a little grand, but the idea is straightforward: a simulation environment where you can specify the physical and chemical parameters of a hypothetical world — temperature, solvent, available elements, energy gradients — and then iterate on biological designs within those constraints.

The workflow is a loop: generate candidate sequences with AI, simulate their behavior in the virtual environment, evaluate fitness against defined criteria, use those results to guide the next round of generation. A design-simulate-evaluate cycle, running in silico at a speed and scale no physical lab could match.

What makes the CVB more than just a protein design tool is the multi-scale ambition: not just individual enzymes, but pathways, regulatory networks, and eventually whole-cell models — all adapted to non-terrestrial or ancient environments. This is closer in spirit to a particle accelerator than to a wet lab. The goal is not to test specific hypotheses but to map a territory.

This does, of course, raise real questions. Designing biology that is fundamentally alien to anything on Earth — novel genetic codes, non-canonical amino acids, entirely synthetic metabolic architectures — requires careful thinking about containment and unintended consequences. I take those concerns seriously, and they'll need to evolve alongside the capabilities.

---

## What Falls Out Along the Way

Research like this doesn't produce only the thing you set out to find. The pursuit of alien or ancient biology, pursued seriously, generates an extraordinary amount of useful material as a byproduct.

**Biocatalysts that actually work at scale.** Current industrial enzymes are borrowed from organisms that had other things to optimize for. Designing de novo for industrial conditions — high temperatures, organic solvents, continuous operation — could yield catalysts dramatically more effective than anything evolution happened to produce.

**Novel genetic codes.** DNA using four bases and twenty amino acids is Earth's solution. It's not the only possible one. Alternative codes with expanded amino acid alphabets, improved error correction, or inherent resistance to viral hijacking have obvious applications in synthetic biology and biomanufacturing.

**Resilient production organisms.** Microorganisms that evolved in the deep ocean or volcanic vents don't get contaminated by the same pathogens that bedevil fermentation facilities. Understanding the principles behind extreme environmental adaptation — and designing for them from scratch — could transform how we build production platforms.

**Biosensors and therapeutics from unexplored design space.** Some of the most useful molecules in medicine came from organisms nobody thought to study until they did: organisms from soil, from deep-sea vents, from caves. Systematic exploration of alternative biochemistry, in silico, is a way to search that space orders of magnitude faster.

---

## Why This Matters

The standard model of biotechnology is still largely reverse engineering. We look at what evolution made, figure out how it works, and try to modify it to suit our purposes. It's powerful — it's given us modern medicine, industrial fermentation, and gene therapy — but it's inherently limited by the starting material.

The proposal here is different: use AI to escape the Red Queen Tax not by working around evolution's constraints, but by simulating evolution under conditions where those constraints never existed. Design biology from principles rather than from precedent. Explore not just the organisms that happened to survive on this one planet, but the much larger space of what could be alive, somewhere, under some conditions.

Four billion years of natural selection is an extraordinary achievement. But it's also only one path through an astronomically large design space. It seems worth finding out what else is in there.

---

*This post is part of an ongoing series on generative AI, synthetic biology, and the future of biological engineering. Reach out if you'd like to discuss.*
