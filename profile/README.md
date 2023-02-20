# Welcome to the SolARM project

The SolARM project is a collection of software tools and services that allow to easily create custom illumos Distributions in a collaborative way. SolARM is based on the IPS package manager and lessons learned while maintaining the existing illumos Distributions. The Project uses existing illumos terminology and ideas but also does not shy away from changes when those are more helpfull to achieve the Design Goals

## Gates
SolARM features collections of sources and build instructions called gates. Each gate can have sub gates that can be shared by multiple distributions. However each distribution has one gate that gives access to all the sources used in the distributions.

## Components
A Component contains the build instructions for a specific piece of software and all patches and changes that have not yet been upstreamed to the softwares maintainer.

## Distributions
Distributions are a set of precompiled software collections ready to be used on a machine that has Compatible hardware. Currently the reference Arm Distribution is implemented with these tools.

## Ports
Ports is the tool used to run the gates and components build instructions and create packages from them. All instructions are data based and not imperative. Ports controls the process and standardises the process. This is based on the experience from OpenIndiana's userland gate, OmniOS Community Edition's build and extra scripts and pkgsrc. Ports is implemented in Rust so that libraries and bindings for the dataformats can be easily produced.
