<p align="center">
  <img src="https://raw.githubusercontent.com/policylabs/.github/main/profile/logo.png" alt="The Policy Labs Project logo: a padlock assembling itself from a stream of bits" width="200">
</p>

<h1 align="center">The Policy Labs Project</h1>

<p align="center"><em>An open source initiative to harden the SDLC</em></p>

Policy Labs is the home of 🔴🟡🟢 [AMPEL](https://github.com/policylabs/ampel)
and the libraries around it. Together they answer one question at every step
of the software development lifecycle: *can this source code, this tool, this
build be trusted?* The answer comes from verifying signed attestations against
policies, not from taking anyone's word for it.

## Projects

| Project | What it is |
| --- | --- |
| [**ampel**](https://github.com/policylabs/ampel) | The Amazing Multipurpose Policy Engine (and L). A lightweight supply chain policy engine that verifies signed attestations, such as [SLSA](https://slsa.dev) provenance, SBOMs and vulnerability scans, against policies. Runs as a CLI and embeds as a library. |
| [**policy**](https://github.com/policylabs/policy) | The AMPEL policy framework: the data structures, tooling and libraries to define, distribute and manage policies. |
| [**attestation**](https://github.com/policylabs/attestation) | The attestation framework the other projects share, built on top of the [in-toto](https://in-toto.io) attestation formats. |
| [**collector**](https://github.com/policylabs/collector) | Finds and parses attestations wherever they live: files, releases, registries, repositories. |
| [**signer**](https://github.com/policylabs/signer) | A signing and verification library with support for [sigstore](https://www.sigstore.dev) bundles, [DSSE](https://github.com/secure-systems-lab/dsse) envelopes and plain key pairs. |
| [**signer-extras**](https://github.com/policylabs/signer-extras) | Extra providers and plugins for the signer, kept apart to keep its dependency tree small. |
| [**predicates**](https://github.com/policylabs/predicates) | Attestation predicates for AMPEL's own policy material and results. |
| [**oss**](https://github.com/policylabs/oss) | Policies for open source projects. |

## How we work

The project is run in the open by a steering committee, and no single
organization may hold more than a third of its seats. A few principles guide
its decisions:

- **Open source first.** The goal is to bind the open source supply chain
  ecosystem together, not to replace parts of it.
- **Non-partisan.** There are no winning formats or technologies. The tools
  stay format and technology agnostic wherever that is technically feasible.
- **Security and compliance by design.** Downstream users must be able to
  audit and trust what they get from us.
- **Interoperability.** The tools should fit into the signing frameworks,
  container environments and CI/CD pipelines people already use.

The full rules are in the
[governance document](https://github.com/policylabs/community/blob/main/GOVERNANCE.md).

## Get involved

Issues and pull requests are welcome in every repository. Two things to know
before sending a patch:

- All commits need a `Signed-off-by` line (`git commit -s`), certifying the
  [Developer Certificate of Origin](https://developercertificate.org).
- Project-wide discussions, proposals and steering committee votes happen in
  the [community repository](https://github.com/policylabs/community).

Everyone taking part is expected to follow the OpenSSF
[Code of Conduct](https://openssf.org/community/code-of-conduct/).

The code is released under the Apache 2.0 license; the policies in
[oss](https://github.com/policylabs/oss) are dedicated to the public domain
under CC0.
