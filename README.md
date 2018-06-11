# virome-protocols

## Table of contents

* [Filtration](#filtration)
* [Nucleic acid extraction](#nucleic-acid-extraction)
* [SSIV standard protocol (RT and 2nd strand synthesis)](#ssiv-standard-protocol-rt-and-2nd-strand-synthesis)

## Filtration
### Material
* Filter (0.45 µm), TPP, [99745](http://www.tpp.ch/page/produkte/12_filtration_spritzenfilter.php?lang=DE)
* Syringe
* Container, 8 mL or 25 mL

### Procedure
* With syringe aspirate the sample and press through filter in a new container
* Replace filter when clogged

## Nucleic acid extraction
### Material
* 1 mL nuclease treated- or untreated sample
* Pipettes and tips
* 1.5 mL tubes
* [NucliSENS easyMag](http://www.biomerieux-usa.com/clinical/nuclisens-easymag) (bioMérieux)

### Procedure
* from 1 mL sample extract total nucleic acid and elute in 25 µL using the NucliSENS easyMag
* store extract at -20°C

## SSIV standard protocol (RT and 2nd strand synthesis)
### Reagents
* UltraPure DNase/RNase-Free Distilled Water, Invitrogen, [10977035](https://www.thermofisher.com/order/catalog/product/10977035)
* Primer 6N, 100 µM (mh413_6N, 5'-NNNNNN-3')
* dNTP, [Thermo Scientific](https://www.thermofisher.com/ch/en/home/brands/thermo-scientific/molecular-biology/thermo-scientific-pcr/dntps-ntps-modified-nucleotides.html)
* SuperScript IV Reverse Transcriptase, Invitrogen, [18090200](https://www.thermofisher.com/order/catalog/product/18090200?SID=srch-hj-18090200)
* RNaseOUT Recombinant Ribonuclease Inhibitor, Invitrogen, [10777019](https://www.thermofisher.com/order/catalog/product/10777019)
* RNase H, New England Biolabs, [M0297S](https://www.neb.com/products/m0297-rnase-h#Product%20Information)
* DNA Polymerase I, Large (Klenow) Fragment, New England Biolabs, [M0210L](https://www.neb.com/products/m0210-dna-polymerase-i-large-klenow-fragment)
* QuantiFluor ONE dsDNA System, Promega, [E4870](https://ch.promega.com/products/dna-purification-quantitation/dna-and-rna-quantitation/quantifluor-one-dsdna-system/?catNum=E4870)
* Nextera XT DNA Library Preparation Kit (96 samples), Illumina, [FC-131-1096](https://emea.illumina.com/products/by-type/sequencing-kits/library-prep-kits/nextera-xt-dna.html?langsel=/ch/)
* Nextera XT Index Kit (96 indexes, 384 samples), Illumina, [FC-131-1002](https://emea.illumina.com/products/by-type/sequencing-kits/library-prep-kits/nextera-xt-dna.html?langsel=/ch/)
* MiSeq Reagent Kit v3 (150-cycle), Illumina, [MS-102-3001](https://emea.illumina.com/products/by-type/sequencing-kits/cluster-gen-sequencing-reagents/miseq-reagent-kit-v3.html?langsel=/ch/)

### Material
* DNA/RNA extract from nucleic acid extraction
* Pipettes and tips
* 1.5 mL tubes
* PCR strips
* PCR cycler
* Quantus Fluorometer, Promega, [E6150](https://ch.promega.com/products/fluorometers-luminometers-multimode-readers/fluorometers/quantus-fluorometer/?catNum=E6150)
* Thermomixer
* [MiSeq](https://emea.illumina.com/systems/sequencing-platforms/miseq.html?langsel=/ch/), Illumina

### Procedure
* Fill in and follow instructions in [SSIV_standard.xltx](SSIV_standard.xltx)
* Quantify DNA in 2nd strand synthesis products (**Note: if unpurified, quantification might be too high**)
* If purified 2nd strand synthesis products were below 0.2 ng/µL, 5 µL undiluted products were used for Nextera XT library preparation
* Follow Nextera XT standard protocol and sequence 151 cycles on the MiSeq

## Release History

* [2.0.0](https://github.com/medvir/virome-protocols/releases/tag/v2.0.0)
    * no nuclease-treatment
    * switch RT enzyme from SSIII to SSIV
    * combined DNA/RNA workflow
    * exclude anker PCR
* [1.0.0](https://github.com/medvir/virome-protocols/releases/tag/v1.0.0)
    * published virome-protocol, including DNA/RNA split workflow and anker PCR
