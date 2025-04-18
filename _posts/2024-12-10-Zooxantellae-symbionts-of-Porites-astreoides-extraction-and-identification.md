---
layout: post
title: Zooxantellae symbionts of Porites astreoides extraction and identification
category: Extraction
tags: [DNA, extraction, Porites, PCR]
---

This protocol was adapted from the protocol of Rachel Bober [(RachelBober)](https://github.com/RachelBober/) written on 26.11.24.
The aim is to compare symbiont species of P. astreoides across treatments in the translocation experiment. For this:
1. DNA was extracted from acetone-fixed zooxantellae from each coral sample
2. DNA was amplified with ITS2 primers
3. PCR products were visualised using gel electrophoresis
4. The bands were cut from the gel and cleaned

Using the [ISOLATE II Plant DNA kit](https://www.bioline.com/mwdownloads/download/link/id/1197/nucleic_acid_isolation_guide.pdf). 

### 1. DNA extraction

#### Preparations
1. Pre-heat an incubator to 65ºC, pre-heat Lysis Buffer PA1 and Elution Buffer PG to 65ºC
2. Fill a bucket with ice
3. Take out from -20ºC: Proteinase K (Zymo kit), RNAseI (ISOLATE II kit) and put on ice

#### Initial steps for samples stored in acetone
1. Centrifuge eppendorfs at max speed for 1 minute
2. Remove acetone with a filter tip
3. Repeat centrifugation to remove acetone remains
4. Wash pellet with 1 ml FSW (0.22u filtered sea water) or PBS (use reverse pipetting and mix well)
5. Transfer the sample into a new 1.5 ml tube
6. Centrifuge again for 1 minute. If a pellet is not forming, add another centrifugation step -  5 min at max speed
7. Remove FSW/PBS supernatant using a filter tip, be careful – do not disturb the pellet.
Note: If some FSW/PBS remains, continue without trying to remove it.

#### Lysis
1. Add 15 ul Proteinase K + 30 ul PK digestion buffer from Zymo kit (not included in this kit) to each sample, vortex
2. Incubate for 30 min at RT
3. Centrifuge at max speed for 2 min 
4. Add 400 ul Lysis Buffer PA1 Pre-heated to 65ºC
5. Vortex
6. Add 10 ul RNAseI
7. Vortex
8. Incubate for 25 min at 65ºC
   
#### Filter crude lysate
1. Transfer lysate (without the pellet if possible) to a collection tube with a purple filter column
2. Centrifuge 11,000 x g, 2 min
3. Collect supernatant to a new tube, discard pellet if it forms
4. Add 450 μL Binding Buffer PB 
5. Pipette 5 times up and down to mix
   
#### Bind DNA 
1. Load lysate in a collection tube with a green filter column (up to 700 ul)
2. Centrifuge 11,000 x g, 1 min
3. Discard the flow-through
   
#### Wash and dry silica membrane
1. 1st wash 400 μL Wash Buffer PAW1
2. Centrifuge 11,000 x g, 1 min
3. Discard the flow-through
4. 2nd wash 700 μL Wash Buffer PAW2
5. Centrifuge 11,000 x g, 1 min
6. Discard the flow-through
7. 3rd wash 200 μL Wash Buffer PAW2
8. Centrifuge 11,000 x g, 2 min
9. Discard the flow-through and the collection tube
    
#### Elute DNA 
1. Place the green filter column in an empty sterile eppendorf tube
2. Add 30 μL Elution Buffer PG (Pre-heat to 65ºC) 
3. Incubate 65ºC, 5 min
4. Repeat DNA elution step

#### DNA quantity
1. Measure DNA quantity and ratio with NanoDrop

### 2. PCR

Primers for ITS2:

|  			CS1F 		 |  			F 		 |  			ACACTGACGACATGGTTCTACATGTGAATTGCAGAACTCCGTG 		    |  
|--------|-----|--------------------------------------------------|
|  			CS2R 		 |  			R 		 |  			TACGGTAGCAGAGACTTGGTCTTACTTATATGCTTAAATTCRGCGG 		 | 

Master mix: [GoTaq® Green master mix](https://worldwide.promega.com/resources/protocols/product-information-sheets/g/gotaq-green-master-mix-m712-protocol/) from Promega.

I diluted each sample according to the NanoDrop results so the DNA template was around 2-3 ng/ul for each sample. For 25 ul reaction:

|  			Component 		                   |  			Volume 		 |
|-------------------------------|----------|
|  			GoTaq® Green Master Mix, 2X 		 |  			12.5µl 		 |
|  			upstream primer, 10µM 		       |  			0.75µl 		 |
|  			downstream primer, 10µM 		     |  			0.75µl  |
|  			DNA template	                 |  			5.0 µl 		 |
|  			BSA, 1 mg/ml                 |  			4.0 µl 		 |
|           DMSO 100%           |  2.0 µl  |
|  			H2O 		                         |  			- 		      |

PCR program: 16 NGS (BioRad C1000 Thouch Thermal Cycler)

|  			ITS CS      |  			Temp C |  			Cycles                      |
|--------------|---------|------------------------------|
| Initial      | 94      | 1                            |
| Denaturation | 94      | 3,4,5 - repeat for 10 cycles |
| Annealing    | 50      | 3,4,5 - repeat for 10 cycles |
| Elongation   | 72      | 3,4,5 - repeat for 10 cycles |
| Denaturation | 94      | 6,7,8 - repeat for 15 cycles |
| Annealing    | 60      | 6,7,8 - repeat for 15 cycles |
| Elongation   | 72      | 6,7,8 - repeat for 15 cycles |
| Final        | 72      | 1                            |

For some of the samples, this PCR result in a double band in the desired location. The second annealing temperature can be increased to 61.5ºC for a better specificity of the primers. It solves the problem of a double band for almost all samples, simultaneously reducing the intensity of the band.  

### 3. Gel electrophoresis

Big gel (~25 lanes) recipe: 1% agarose gel (1g agarose in 100 ml 0.5x TBE + 4 ul Red safe), 110 V 

Small gel (~15 lanes) recipe: 1% agarose gel (0.5g agarose in 50 ml 0.5x TBE + 2 ul Red safe), 70 V

Ladders: EuRx Perfect 1 kb DNA Ladder, EuRx Perfect 100 bp DNA Ladder.

### 4. Excising gel bands and cleaning the product


