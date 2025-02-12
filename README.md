# Overture Maps Landscape

![Overture Maps Landscape Logo](https://landscape.overturemaps.org/images/omf.png)

This landscape is intended as a map to explore the Overture Maps Ecosystem, and also shows the member companies of the Overture Maps Foundation. It is modeled after the Cloud Native Computing Foundation (CNCF) [landscape](https://landscape.cncf.io) and based on the same open-source code.

This repository contains the data files and images required to generate the [Overture Maps Landscape](https://landscape.overturemaps.org). The software that generates it can be found at the [cncf/landscape2](https://github.com/cncf/landscape2) repository. Please see its [README file](https://github.com/cncf/landscape2#landscape2) for more information about how it works.

## New Entries and Corrections

All the data in this repository is built nightly using the [LFX Landscape Tools](https://github.com/jmertic/lfx-landscape-tools). Any changes made directly in the data files in this repository will be overwritten.

- For member entries, you can make these changes in [LFX Organization Dashboard](https://docs.linuxfoundation.org/lfx/organization-dashboard/organization-profile).

If you cannot access the above resources, please [create a helpdesk ticket](https://members.linuxfoundation.org) to request those changes.

## Local Build and Install

You can build the landscape locally on your machine using the [landscape2](https://github.com/cncf/landscape2) tool. Once [installed](https://github.com/cncf/landscape2?tab=readme-ov-file#installation), you can use the commands below to build the landscape and serve it locally.

```shell
landscape2 build --data-file landscape.yml --settings-url https://raw.githubusercontent.com/cncf/landscape2-sites/refs/heads/main/overturemaps/settings.yml --logos-path hosted_logos --output-dir build
landscape2 serve --landscape-dir build
```

## License

The generated landscape contains data received from [Crunchbase](http://www.crunchbase.com). This data is not licensed pursuant to the Apache License. It is subject to Crunchbase’s Data Access Terms, available at [https://data.crunchbase.com/docs/terms](https://data.crunchbase.com/docs/terms), and is only permitted to be used with Overture Maps Landscape projects.

Everything else is under the Apache License, Version 2.0, except for projects and product logos, which are generally copyrighted by the company that created them and are simply cached here for reliability. The generated landscape and the [landscape.yml](landscape.yml) file are alternatively available under the [Creative Commons Attribution 4.0 license](https://creativecommons.org/licenses/by/4.0/).
