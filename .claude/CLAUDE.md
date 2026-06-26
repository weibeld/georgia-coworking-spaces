# CLAUDE.md — Georgia Coworking Spaces

This project records information about visited coworking spaces in the country of Georgia. This data is planned to eventually be converted to a data set in [Giraffe](https://github.com/weibeld/giraffe/) (see project description in [concept doc](https://raw.githubusercontent.com/weibeld/giraffe/refs/heads/main/.claude/concept.md)).

The data is located in the `coworking-spaces/` sub-directory and is split across two files:

- **`georgia-automated.yaml`:** Data that can be determined automatically from sources like the coworking space's website or Google Maps. Currently, this data is still entered manually, but it is planned that this will eventually be automated when the data is managed within Giraffe. When the data is managed in Giraffe, additional fields like Google Places ID, geographical coordinates, Google Maps rating, etc. are also planned to be added and subsequentially automatically determined for all items.
- **`georgia-manual.yaml`:** Data that cannot be reliably determined automatically and mainly results from personal observations during visits to the coworking spaces. These data fields are determined manually now and will also likely have to be determined manually when the data is managed in Giraffe.
