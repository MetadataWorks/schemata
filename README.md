![generate-markdown](https://github.com/HDRUK/schemata/workflows/generate-markdown/badge.svg)

# HDR UK Schemata - Dataset V2.0.0

### 1. [HDR UK Dataset Schema](https://github.com/HDRUK/schemata/blob/develop/docs/dataset/latest/dataset.md)

 - Latest json schema and yml can be found here:  https://github.com/HDRUK/schemata/blob/develop/schema/dataset/latest
 - Example json files can be found here including a current mapped dataset, a minimium json example and a ful example: https://github.com/HDRUK/schemata/blob/develop/examples 
 - Latest word documentation, change log and mapping file can be found here: https://github.com/HDRUK/schemata/blob/develop/docs/distribution
 - Impact assessment and indicative mapping files can be found here: https://github.com/HDRUK/schemata/blob/develop/docs/impact-assessment
      - aggregated_errors.xlsx: aggregated validation errors with an overview on the most common errors per attribute that will need to be resolved during migration
      - generated_mapping.py: the mapping algorithm that generates v2 data-models, (basically a mapping function for all fields in the new v2 specs).
      - v1_to_v2.json: for each data-model (key is the UUID) v1: old schema, v2: new schema, which is the mapping result (generated_mapping.py) of all data-models in the gateway.
      - dm_validation.json: for each data-model (key again is UUID) the data-set in form of the v2 attributes and the JSON schema validation.
      - aggregated_errors.json: an aggregation of the validation of all data-models by attribute with a list of unique error messages, a count of unique error messages, and a total count of the errors across all data-models; note tjat JSON schema validator generates an entry for all hierarchy levels, which means some error messages are repeated along the hierarchy.
