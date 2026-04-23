# Clinical Trials for Argument Mining in Spanish: ClinArgES Corpus

## Documents
The **ClinArgES corpus version 1** gathers 130 clinical trials sourced from the [CT-EBM-SP corpus](https://github.com/lcampillos/ct-ebm-sp-v3).

## Distribution of abstracts from journals with Creative Commons License
We used only abstracts with a **Creative Commons Non-Commercial (CC BY-NC)** license. Under this license:
* You can reuse and/or redistribute these texts in non-commercial applications.
* You must give appropriate credit and indicate if changes were made. 
* The copyright and other intellectual property rights of the text contents correspond to each article's authors.

## Distribution of clinical trials announcements from EudraCT
We attribute the source as **"EU Clinical Trials Register"** and state that these data were accessed from February to June 2020.

The **European Medicines Agency (EMA)** is the owner of copyright and other intellectual property rights for documents published on its website. Information is public and may be reproduced/distributed for non-commercial and commercial purposes, provided the Agency is acknowledged as the source. 

For further information, see: [EMA Legal Notice](https://www.ema.europa.eu/en/about-us/legal-notice).

## Corpus format
The documents have been manually annotated with argument components (**Major Claim, Claim, and Premise**) and relationships (**Attack, Partial-Attack, and Support**).

The corpus is a JSON array where each element represents one clinical trial:

```json
[
  {
    "id": "<case_id>",
    "raw_text": "<full text used for tokenization>",
    "metadata": {},
    "annotations": {
      "entities": [
        {
          "id": "T1",
          "text": "...",
          "start": 91,
          "end": 123,
          "type": "Premise"
        }
      ],
      "relations": [
        {
          "id": "r1",
          "arg1_id": "e1",
          "arg2_id": "e2",
          "relation_type": "Support"
        }
      ]
    }
  }
]
```

## How to cite

If you use this corpus, please cite the reference as follows:

## License
This work is licensed under a Creative Commons Attribution-NonCommercial 4.0 International License (CC BY-NC 4.0).

## Copyright
Copyright (c) 2026 ClinArgES Corpus version 1 Desarrollado por: 

Sofía Zakhir-Puig / University of Valencia (UV), Valencia, Spain
Vanesa Vanesa / Rey Juan Carlos University (URJC), Madrid, Spain
Miguel Ángel Rodríguez-García / National Distance Education University (UNED), Madrid, Spain
Soto Montalvo / Rey Juan Carlos University (URJC), Madrid, Spain
Raquel Martínez / National Distance Education University (UNED), Madrid, Spain

The European Medicines Agency owns the copyright and other intellectual property rights of the documents from EudraCT.

## Contact

Miguel Ángel Rodríguez-García (miguelangel.rodriguez@lsi.uned.es)
Soto Montalvo ()soto.montalvo@urjc.es
