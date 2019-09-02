# pyncaids

National Competent Authority (NCA) identifiers as a Python module

```python
import pyncaids

nca_dict =  {
    "authority_id": "GB-FCA",
    "country": "United Kingdom",
    "authority_name": "Financial Conduct Authority"
}

nca = pyncaids.NCA()

authority_list = nca.nca_by_authority_id("GB-FCA")

authority_list = nca.nca_by_partial_authority_id("A")

authority_list = nca.nca_by_country("United Kingdom")

authority_list = nca.nca_by_partial_country("i")

authority_list = nca.nca_by_authority_name("Financial Conduct Authority")

authority_list = nca.nca_by_partial_authority_name("Authority")
```