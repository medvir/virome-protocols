# virome-protocols

## Table of contents

* [Filtration](#filtration)
* [Nuclease treatment](#nuclease-treatment)
* [Nucleic acid extraction](#nucleic-acid-extraction)
* [Split protocol (RT, 2nd strand synthesis and anker PCR)](#split-protocol-rt-2nd-strand-synthesis-and-anker-pcr)

## Filtration
### Material
* Filter (0.45 µm), TPP, [99745](http://www.tpp.ch/page/produkte/12_filtration_spritzenfilter.php?lang=DE)
* Syringe
* Container, 8 mL or 25 mL

### Procedure
* With syringe aspirate the sample and press through filter in a new container
* Replace filter when clogged

## Nuclease treatment
### Reagents
* UltraPure DNase/RNase-Free Distilled Water, Invitrogen, [10977035](https://www.thermofisher.com/order/catalog/product/10977035)  
* TURBO DNase (2 U/µL), Invitrogen, [AM2239](https://www.thermofisher.com/order/catalog/product/AM2239)  
* RNase A (7000 U/mL), Qiagen, [19101](https://www.qiagen.com/ch/shop/lab-basics/enzymes/rnase-a/?akamai-feo=off&clear=true#orderinginformation)

### Material
* Sample (>= 1 mL)
* Pipettes and tips
* 1.5 mL tubes
* Thermomixer

### Procedure
* calculate and prepare nuclease mix ([nuclease_treatment.xltx](nuclease_treatment.xltx))
* in 1.5 mL tubes add 300 µL nuclease mix to 1 mL Sample
* incubate on the thermomixer (30 min, 37°C, 1400 rpm)
* proceed immediately to nucleic acid extraction

## Nucleic acid extraction
### Material
* 1 mL nuclease treated- or untreated sample
* Pipettes and tips
* 1.5 mL tubes
* [NucliSENS easyMag](http://www.biomerieux-usa.com/clinical/nuclisens-easymag) (bioMérieux)

### Procedure
* from 1 mL sample extract total nucleic acid and elute in 25 µL using the NucliSENS easyMag
* store extract at -20°C

## Split protocol (RT, 2nd strand synthesis and anker PCR)
### Reagents
* UltraPure DNase/RNase-Free Distilled Water, Invitrogen, [10977035](https://www.thermofisher.com/order/catalog/product/10977035)
* Primer 454-8N, 100 µM (mh220_454-A-8N, 5'-ATCGTCGTCGTAGGCTGCTCNNNNNNNN-3')
* dNTP, [Thermo Scientific](https://www.thermofisher.com/ch/en/home/brands/thermo-scientific/molecular-biology/thermo-scientific-pcr/dntps-ntps-modified-nucleotides.html)
* SuperScript III Reverse Transcriptase, Invitrogen, [18080085](https://www.thermofisher.com/order/catalog/product/18080085)
* DNA Polymerase I, Large (Klenow) Fragment, New England Biolabs, [M0210L](https://www.neb.com/products/m0210-dna-polymerase-i-large-klenow-fragment)
* AmpliTaq Gold DNA Polymerase with Buffer I, Applied Biosystems,[N8080246](https://www.thermofisher.com/order/catalog/product/N8080246?SID=srch-hj-N8080246)
* 454-A distinct Primer, 10 µM (mh218_454-A, 5'-ATCGTCGTCGTAGGCTGCTC-3')
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
* Thermomixer
* Quantus Fluorometer, Promega, [E6150](https://ch.promega.com/products/fluorometers-luminometers-multimode-readers/fluorometers/quantus-fluorometer/?catNum=E6150)
* [MiSeq](https://emea.illumina.com/systems/sequencing-platforms/miseq.html?langsel=/ch/), Illumina

### Procedure
* Fill in and follow instructions in [split.xltx](split.xltx)
* Quantify DNA in unpurified anker PCR with the Quantus and dilute in Water to 0.2 ng/µL
* For the Nextera XT library preparation pool 2.5 µL of the corresponding diluted DNA/RNA workflow anker PCR products
* Follow Nextera XT standard protocol and sequence 151 cycles on the MiSeq

## Release History
* [1.0.0](https://github.com/medvir/virome-protocols/releases/tag/v1.0.0)
    * published virome-protocol, including DNA/RNA split workflow and anker PCR
