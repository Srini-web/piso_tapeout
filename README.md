# Caravel User Project

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![UPRJ_CI](https://github.com/efabless/caravel_project_example/actions/workflows/user_project_ci.yml/badge.svg)](https://github.com/efabless/caravel_project_example/actions/workflows/user_project_ci.yml) [![Caravel Build](https://github.com/efabless/caravel_project_example/actions/workflows/caravel_build.yml/badge.svg)](https://github.com/efabless/caravel_project_example/actions/workflows/caravel_build.yml)

| :exclamation: Important Note            |
|-----------------------------------------|

## Please fill in your project documentation in this README.md file 

Refer to [README](docs/source/index.rst#section-quickstart) for a quickstart of how to use caravel_user_project

Refer to [README](docs/source/index.rst) for this sample project documentation. 

Refer to the following [readthedocs](https://caravel-sim-infrastructure.readthedocs.io/en/latest/index.html) for how to add cocotb tests to your project. 

## Efabless upload 

<img width="934" alt="image" src="https://github.com/Srini-web/piso_tapeout/assets/77874288/f5ea58f9-1a58-482c-91bf-0e0f20dff65b">

Problem: was unable to upload on efabless
Solution: It was due to the lack of an SSH key for the remote repo. Had to advance a few steps and then return to previous step after which upload was successful

## Physical implementation and project integration
Changing user project `mprj` to custom `piso` circuit

![projfilechange](https://github.com/Srini-web/piso_tapeout/assets/77874288/8371cac0-919e-4dc7-ada6-a74075ed7f97)

After adding test bench files in `rtl/verilog/dv` path, and including them in cocotb folder,
we assign power pins

![wrapperchange](https://github.com/Srini-web/piso_tapeout/assets/77874288/a4040b8d-ad02-4e41-a845-54a6321b020c)

also changing sdc reference in both `sdc` folder and `openlane` folder,
![sdcfile](https://github.com/Srini-web/piso_tapeout/assets/77874288/c7d01f74-239d-4c1e-9275-11b755cfbc4d)

Output, Input, and OEB pins are customized and wishbone pins are commented

![ioandoebpins](https://github.com/Srini-web/piso_tapeout/assets/77874288/61514a10-6375-4a00-abcb-9466c9995e27)

Now, all these changed files are included and project is verified

![includeschange](https://github.com/Srini-web/piso_tapeout/assets/77874288/8d0f7893-37d0-48b6-9257-34ffe5c42179)


