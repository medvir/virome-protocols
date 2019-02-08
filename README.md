# virome-protocols

## Table of contents

* [Filtration](#filtration)
* [Nucleic acid extraction](#nucleic-acid-extraction)
* [DNase treatment](#dnase-treatment)
* [SSIV split protocol (RT and 2nd strand synthesis)](#ssiv-split-protocol-rt-and-2nd-strand-synthesis)

## Filtration
### Material
* Filter (0.45 µm), TPP, [99745](http://www.tpp.ch/page/produkte/12_filtration_spritzenfilter.php?lang=DE)
* Syringe
* Container, 8 mL or 25 mL

### Procedure
* Centrifuge sample and use supernatant to remove cells (e.g. WBC and RBC in case of blood) or other solids
* With syringe aspirate the sample and press through filter in a new container
* Replace filter when clogged

## Nucleic acid extraction
### Material
* 1 mL sample
* Pipettes and tips
* 1.5 mL tubes
* [NucliSENS easyMag](http://www.biomerieux-usa.com/clinical/nuclisens-easymag) (bioMérieux)

### Procedure
* from 1 mL sample extract total nucleic acid and elute in 25 µL using the NucliSENS easyMag
* store extract at -20°C

## DNase treatment
### Reagents
* TURBO DNA-free Kit, Invitrogen, [AM1907](https://www.thermofisher.com/order/catalog/product/AM1907)

### Material
* DNA/RNA extract from nucleic acid extraction
* Pipettes and tips
* 1.5 mL tubes
* Thermomixer
* Centrifuge

### Procedure
* Combine 5 µL DNA/RNA extract, 1.2 µL 10✕ TURBO DNase Buffer and 1 µL TURBO DNase (2 U)
* Incubate at 37°C for 20 min
* Add 2 µL resuspended DNase Inactivation Reagent
* Incubate 5 min at room temperature, mixing occasionally
* Centrifuge at 10'000 g for 1.5 min and transfer the RNA to a fresh tube

## SSIV split protocol (RT and 2nd strand synthesis)
### Reagents
* UltraPure DNase/RNase-Free Distilled Water, Invitrogen, [10977035](https://www.thermofisher.com/order/catalog/product/10977035)
* Primer 6N, 100 µM (mh413_6N, 5'-NNNNNN-3')
* dNTP, Thermo Scientific, [R0192](https://www.thermofisher.com/order/catalog/product/R0192)
* SuperScript IV Reverse Transcriptase, Invitrogen, [18090200](https://www.thermofisher.com/order/catalog/product/18090200?SID=srch-hj-18090200)
* RNaseOUT Recombinant Ribonuclease Inhibitor, Invitrogen, [10777019](https://www.thermofisher.com/order/catalog/product/10777019)
* RNase H, New England Biolabs, [M0297S](https://www.neb.com/products/m0297-rnase-h#Product%20Information)
* DNA Polymerase I, Large (Klenow) Fragment, New England Biolabs, [M0210L](https://www.neb.com/products/m0210-dna-polymerase-i-large-klenow-fragment)
* Agencourt AMPure XP Beads, Beckman Coulter, [A63881](https://www.beckman.com/reagents/genomic/purification-and-cleanup/pcr)
* Ethanol absolute
* QuantiFluor ONE dsDNA System, Promega, [E4870](https://ch.promega.com/products/dna-purification-quantitation/dna-and-rna-quantitation/quantifluor-one-dsdna-system/?catNum=E4870)
* Nextera XT DNA Library Preparation Kit (96 samples), Illumina, [FC-131-1096](https://emea.illumina.com/products/by-type/sequencing-kits/library-prep-kits/nextera-xt-dna.html?langsel=/ch/)
* Nextera XT Index Kit (96 indexes, 384 samples), Illumina, [FC-131-1002](https://emea.illumina.com/products/by-type/sequencing-kits/library-prep-kits/nextera-xt-dna.html?langsel=/ch/)
* MiSeq Reagent Kit v3 (150-cycle), Illumina, [MS-102-3001](https://emea.illumina.com/products/by-type/sequencing-kits/cluster-gen-sequencing-reagents/miseq-reagent-kit-v3.html?langsel=/ch/)

### Material
* DNA/RNA extract from nucleic acid extraction (for DNA workflow)
* DNase treated extract (for RNA workflow)
* Pipettes and tips
* 1.5 mL tubes
* PCR strips
* PCR cycler
* Magnetic Separation Rack
* Quantus Fluorometer, Promega, [E6150](https://ch.promega.com/products/fluorometers-luminometers-multimode-readers/fluorometers/quantus-fluorometer/?catNum=E6150)
* Thermomixer
* [MiSeq](https://emea.illumina.com/systems/sequencing-platforms/miseq.html?langsel=/ch/), Illumina

### Procedure
* Fill in and follow instructions in [SSIV_standard_split.xltx](SSIV_standard_split.xltx)
* Purify total volume of 2nd strand synthesis products with 2x AMPure beads (20/30 µL DNA + 40/60 µL Beads, wash 2x with 80% Ethanol, dry Beads, elute DNA in 20 µL Water)
* Quantify DNA in 2nd strand synthesis products (**Note: if unpurified, quantification might be too high**)
* If purified 2nd strand synthesis products were below 0.2 ng/µL, 5 µL undiluted products were used for Nextera XT library preparation
* Follow Nextera XT standard protocol and sequence 151 cycles on the MiSeq

## Release History

* [2.2.0](https://github.com/medvir/virome-protocols/releases/tag/v2.2.0)
    * reduce ratio of AMPure beads from 3x to 2x for purification of 2nd strand synthesis products
* [2.1.1](https://github.com/medvir/virome-protocols/releases/tag/v2.1.1)
    * describe centrifugation step before filtration
* [2.1.0](https://github.com/medvir/virome-protocols/releases/tag/v2.1.0)
    * DNA/RNA split workflow including DNase treatment in RNA workflow
    * always purify 2nd strand synthesis products
* [2.0.0](https://github.com/medvir/virome-protocols/releases/tag/v2.0.0)
    * no nuclease-treatment
    * switch RT enzyme from SSIII to SSIV
    * combined DNA/RNA workflow
    * exclude anker PCR
* [1.0.0](https://github.com/medvir/virome-protocols/releases/tag/v1.0.0)
    * published virome-protocol, including DNA/RNA split workflow and anker PCR
