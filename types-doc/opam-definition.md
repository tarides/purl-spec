<!--  NOTE: Auto-generated from the JSON PURL type definition.
Do not manually edit this file. Edit the JSON type definition instead. -->

# PURL Type Definition: opam

- **Type Name:** OCaml opam package
- **Description:** OCaml packages published on the opam repository.
- **Schema ID:** `https://packageurl.org/types/opam-definition.json`

## PURL Syntax

The structure of a PURL for this package type is:

    pkg:opam/<namespace>/<name>@<version>?<qualifiers>#<subpath>

## Repository Information

- **Use Repository:** Yes
- **Default Repository URL:** https://opam.ocaml.org
- **Note:** The default repository is the opam central registry at https://opam.ocaml.org. Use the repository namespace to identify other repositories and the repo_url qualifier to provide their full address (including protocol).

## Namespace definition

- **Requirement:** Optional
- **Native Label:** repository
- **Note:** `When present, the namespace encodes the repository identifier that hosts the opam package. Use a simple identifier without slashes, colons, question marks, hashes, at signs, or square brackets (e.g. opam.ocaml.org, tezos-opam-repository). When omitted, the default repository is https://opam.ocaml.org.`

## Name definition

- **Requirement:** Required
- **Case Sensitive:** Yes
- **Native Label:** name
- **Note:** `The name must match the package name exactly as declared in opam metadata and is case sensitive.`

## Version definition

- **Requirement:** Optional
- **Native Label:** version
- **Note:** `The version is the package version as published in opam.`

## Qualifiers Definition

| Key  | Requirement | Native name | Default Value | Description |
|------|-------------|-------------|---------------|-------------|
| repo_url | Optional |  |  | Full address (including protocol/scheme such as https, git+https, darcs+ssh, hg+https, file:///...) for the repository identified by the namespace. |

## Examples

- `pkg:opam/opam.ocaml.org/ocaml-base-compiler@5.2.0?repo_url=https%3A%2F%2Fopam.ocaml.org`
- `pkg:opam/opam.ocaml.org/git@3.16.1?repo_url=https%3A%2F%2Fopam.ocaml.org`
- `pkg:opam/tezos-opam-repository/git@3.16.1?repo_url=git%2Bhttps%3A%2F%2Fgithub.com%2Ftezos%2Fopam-repository.git`
- `pkg:opam/oxcaml-opam-repository/git@3.16.1?repo_url=https%3A%2F%2Fgithub.com%2Foxcaml%2Fopam-repository.git`
- `pkg:opam/darcs-example-opam-repo/merlin@4.13?repo_url=darcs%2Bssh%3A%2F%2Fdarcs.example.org%2Fopam-repo`
- `pkg:opam/hg-example-opam/ocamlformat@0.26?repo_url=hg%2Bhttps%3A%2F%2Fhg.example.org%2Fopam`
- `pkg:opam/local-home-user-opam-repo/dune@3.16.0?repo_url=file%3A%2F%2F%2Fhome%2Fuser%2Fsrc%2Fopam-repo`
