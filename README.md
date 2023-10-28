# Intangible asset valuations in purchase price allocations

This data is the baseline of acquired intangible valuations from [Ewens, Peters and Wang (2023)](https://osf.io/preprints/socarxiv/kvp2f/). When a public firm acquires a large enough target, they have to disclose the assets and liabilities they are acquiring. In this purchase price allocation (PPA), one can see a collection of intangible assets in a 10-K.  In our paper, we collected and parsed these manually.  The data provided here is the cleaned version of that data.  From our paper, PPAs are:

> "asset appraisals owing to an acquisition undergo an extensive due diligence process by expert appraisers that result in precise valuations. Accounting regulations (ASC 350) require that intangibles being purchased by the acquirer are directly recorded at market value on the acquirer’s balance sheet as either Identifiable Intangible Assets (IIA) or goodwill (GW)."

Our data and sampling methodology is as follows (from Ewens, Peters, and Wang, 2023):

> "We require data availability of the acquirer’s purchase price allocation of the target’s assets in order to collect the prices paid for goodwill and identifiable intangible assets (IIA). When available, these purchase price allocations were found in the acquirer’s subsequent 10-K, 10-Q, 8-K, or S-4 filing. We found information on the purchase price allocation for 81% (1,719) of all candidate acquisitions"

## Citation

If you use this data, please cite the following:

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

