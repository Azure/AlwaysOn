# How to Contribute to AlwaysOn

## Content Changes and Pull Requests

To add or edit content within the AlwaysOn repositories, please take a fork of a repository to iterate on changes before subsequently opening a Pull Request (PR) to get your forked branch merged into the main branch for that AlwaysOn repository. Your PR will be reviewed by core engineers working on the AlwaysOn project, and once approved, your content accessible to everybody.

> **Important!** Please make sure that your PR is focused on a specific area of AlwaysOn to facilitate a targeted review, as this will speed up the process to get your changes merged into our repository.

## Content Structure

[![AlwaysOn Repo Structure](/docs/media/alwayson-repo-structure.png "AlwaysOn Repo Structure")](./CONTRIBUTE.md)

The AlwaysOn project is separated into **3** different repositories:

- [AlwaysOn](./README.md): contains the AlwaysOn design methodology, covering the design pattern ad approach to guide readers to defining a target AlwaysOn architecture.
  - Overarching topics are documented as separate markdown documents within the `/docs/` directory.

- [AlwaysOn-Foundational-Online](http://github.com/azure/alwayson-foundational-online): contains the AlwaysOn foundational reference implementation intended for online scenarios that are public-facing and do not require private network connectivity to a surrounding organizational technical estate.
  - [`/docs/`](https://github.com/Azure/alwayson-foundational-online/tree/main/docs) contains the majority of documentation, covering the design approach and detailed documentation to accompany the reference implementation.
  - [`/src/`](https://github.com/Azure/alwayson-foundational-online/tree/main/src) contains all source code and technical artifacts for the reference implementation along with low level implementation documentation.
  - [`/.ado/pipelines`](https://github.com/Azure/alwayson-foundational-online/tree/main/.ado/pipelines) contains the Azure DevOps pipelines to build and deploy the reference implementation.

- [AlwaysOn-Foundational-Connected](http://github.com/azure/alwayson-foundational-connected): contains the AlwaysOn foundational reference implementation intended for private scenarios that require integration with an organizational technical estate for either public-facing or internal-facing workloads.
  - [`/docs/`](http://github.com/azure/alwayson-foundational-connected/tree/main/docs) contains the majority of documentation, covering the design approach and detailed documentation to accompany the reference implementation.
  - [`/src/`](http://github.com/azure/alwayson-foundational-connected/tree/main/src) contains all source code and technical artifacts for the reference implementation along with low level implementation documentation.
  - [`/.ado/pipelines`](http://github.com/azure/alwayson-foundational-connected/tree/main/.ado/pipelines) contains the Azure DevOps pipelines to build and deploy the reference implementation.

## Documentation Conventions

Each source code component within the reference implementation repositories has it's own `README.md` file which explains how that particular component works, how it is supposed to be used, and how it may interact with other aspects of the AlwaysOn solution.

Within the `main` branch, each `README.md` file must accurately represent the state of the associated component which will serve as a core aspect of PR reviews. Any modifications to source components must therefore be reflected in the documentation as well.
