# Intangible asset valuations in purchase price allocations

This [data](https://github.com/michaelewens/Purchased-intangibles/blob/main/ppa_data_102823.csv) is the baseline of acquired intangible valuations from [Ewens, Peters and Wang (2023)](https://osf.io/preprints/socarxiv/kvp2f/). When a public firm acquires a large enough target, they have to disclose the assets and liabilities they are acquiring. In this purchase price allocation (PPA), one can see a collection of intangible assets in a 10-K.  In our paper, we collected and parsed these manually.  The [purchase price allocation data(PPA)](https://github.com/michaelewens/Purchased-intangibles/blob/main/ppa_data_102823.csv) provided here is the cleaned version of that data.  From our paper, PPAs are:

> "asset appraisals owing to an acquisition undergo an extensive due diligence process by expert appraisers that result in precise valuations. Accounting regulations (ASC 350) require that intangibles being purchased by the acquirer are directly recorded at market value on the acquirer’s balance sheet as either Identifiable Intangible Assets (IIA) or goodwill (GW)."

For example, [our data](https://github.com/michaelewens/Purchased-intangibles/blob/main/ppa_data_102823.csv) includes an acquisition by Matrix Pharmaceutical.  Note 4 of the 10-K reads:
> on February 20, 2002, Chiron acquired Matrix Pharmaceutical, Inc., a company that was developing tezacitabine, a drug to treat cancer. As of March 31, 2002, Chiron acquired substantially all of the outstanding shares of common stock of Matrix Pharmaceutical at $2.21 per share, which, including estimated acquisition costs, resulted in a total preliminary purchase price of approximately $67.1 million. Matrix Pharmaceutical is part of Chiron’s biopharmaceuticals segment. Tezacitabine expanded Chiron’s portfolio of cancer therapeutics. Chiron accounted for the acquisition as an asset purchase and included Matrix Pharmaceutical’s operating results, including the seven business days in February 2002, in its consolidated operating results beginning on March 1, 2002. The components and allocation of the preliminary purchase price, based on their fair values, consisted of the following (in thousands):
> ![Screenshot 2023-11-05 at 8 43 41 AM](https://github.com/michaelewens/Purchased-intangibles/assets/4754737/be6c09f1-5e12-40b6-8df1-1e8626843416)


Our [purchase price allocation data](https://github.com/michaelewens/Purchased-intangibles/blob/main/ppa_data_102823.csv) and sampling methodology that defines the set of acquisitions is described as follows (from Ewens, Peters, and Wang, 2023):

> "We require data availability of the acquirer’s purchase price allocation of the target’s assets in order to collect the prices paid for goodwill and identifiable intangible assets (IIA). When available, these purchase price allocations were found in the acquirer’s subsequent 10-K, 10-Q, 8-K, or S-4 filing. We found information on the purchase price allocation for 81% (1,719) of all candidate acquisitions"

## Citation

If you use the [PPA data](https://github.com/michaelewens/Purchased-intangibles/blob/main/ppa_data_102823.csv), please cite the following:

@article{intangibles,
  title={Measuring intangible capital with market prices},
  author={Ewens, Michael and Peters, Ryan H and Wang, Sean},
  year={Forthcoming},
  journal={Management Science}
}

Ewens, M., Peters, R.H. and Wang, S., 2023. Measuring intangible capital with market prices". Forthcoming, Management Science.

## Key Variables

Below are short descriptions of key variables in the dataset (numbers in millions).  All except cash and goodwill are under "identifiable intangible assets"

- Workforce: value of workforce
- Backlog: backlog of projects
- Cashacquired: acquired cash in deal 
- Contractcontractualrights: value of contractual rights held by target
- CustomerRelationshipscontract: value of customer contracts
- totalDealValueFromFiling: total deal value reported in the filing
- Goodwill: total goodwill of deal
- InProcessRD: value of in-process R&D
- IntellectualProperty: value of intellectual property (patents typically separated)
- MaintenanceSupportContracts: value of contracts to support customer maintenance
- Noncompeteagreements: value of non-compete agreements with employees
- valuePatents: value of target's patents
- Other Technology: value of intangible assets not separated into other categories
- RoyaltyAgreement: value of royalty agreements
- IdentifiableIntangibleassetsI: sum of the value of IIA in filing
- TotalIIAifreportedasaggreg: if the IIA is not disaggregated, this is the reported total TrademarksTradenamesBrand

