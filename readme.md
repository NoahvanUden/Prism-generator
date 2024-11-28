# Generates prism models for failure prediction

For more information see: Dursun, Akcay, van Houtum: "How good must failure predictions be to make local spare parts stock superfluous?" https://doi.org/10.1016/j.ijpe.2023.109060

Steps to create and verify for a set of parameters:

- Create Model object with the following parameters:
  - m: number of machines
  - p: precision
  - qD: sensitivity and timing
  - ch: holding costs
  - cem: emergency costs
  - lambda: failure rate
- Call toFile() to write the model to a PRISM file
- Call getResults() to verify the model (prism must be added to path)
