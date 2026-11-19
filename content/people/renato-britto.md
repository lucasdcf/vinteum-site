---
name: Renato Britto (satsfy)
image: /assets/images/people/illustrations/renato-britto.png
illustration: true
alternateImage: /assets/images/people/fellows/bukele.jpg
programs:
  - program: fellowship
    name: Fellowship
    organization: Vinteum
    role:
      EN: Fellow
      BR: Fellow
    status: past
    end: '2026-09'
    start: '2026-04'
    cohort: 2
    work:
      EN: Rust-Bitcoin
      BR: Rust-Bitcoin
    href: /programs/fellowship
  - program: bitcoin-dev-launchpad
    name: Bitcoin Dev Launchpad
    organization: Vinteum
    role:
      EN: Alumnus
      BR: Ex-participante
    status: past
    cohort: 2
    work:
      EN: Rust-Bitcoin
      BR: Rust-Bitcoin
    href: /programs/bitcoin-dev-launchpad
    fundedBy: Vinteum
    description:
      EN: Moved from production backend and authentication systems into Bitcoin open source
        after Bitcoin Dev Launchpad.
      BR: Passou de sistemas de backend e autenticação em produção para o código aberto
        Bitcoin após o Bitcoin Dev Launchpad.
focus:
  - Rust
  - Fuzzing
  - Correctness
  - RPC
links:
  - label: GitHub
    href: 'https://github.com/satsfy'
    icon: github
  - label: X
    href: 'https://x.com/0xsatsfy'
    icon: twitter
  - label: Website
    href: 'https://satsfy.cc/'
    icon: website
projects:
  - name: rust-bitcoin
    href: 'https://github.com/rust-bitcoin/rust-bitcoin'
    description:
      EN: Rust Bitcoin library
      BR: Bibliotecas Rust para desenvolver aplicações Bitcoin.
    contribution:
      EN: "Hardens the units crate for its 1.0 release, reviewing the API, clearing the issue backlog and fixing bugs. Also works on other crates, such as primitives, and maintains the CI."
      BR: "Prepara o crate units para a 1.0, revisando a API, resolvendo o backlog de issues e corrigindo bugs. Também atua em outros crates, como o primitives, e mantém o CI."
  - name: corepc
    href: 'https://github.com/rust-bitcoin/corepc'
    description:
      EN: Rust library for interacting with Bitcoin Core over JSONRPC
      BR: Biblioteca Rust para interagir com o Bitcoin Core via JSON-RPC.
    contribution:
      EN: "Keeps the RPC types current with each Bitcoin Core release, moved its CI to cargo-rbmt and is building a production client generated from Core's OpenRPC specification."
      BR: "Mantém os tipos das RPCs em dia com cada versão do Bitcoin Core, migrou o CI para o cargo-rbmt e constrói um cliente de produção gerado a partir da especificação OpenRPC do Core."
  - name: rust-bitcoin-maintainer-tools
    href: 'https://git.rust-bitcoin.org/rust-bitcoin/rust-bitcoin-maintainer-tools'
    description:
      EN: CI and release tooling shared by the rust-bitcoin repositories.
      BR: Ferramentas de CI e release compartilhadas pelos repositórios rust-bitcoin.
    contribution:
      EN: "Maintainer. Helps plan the project, reviews its pull requests and moved the rust-bech32 and corepc CI onto it."
      BR: "Maintainer. Ajuda a planejar o projeto, revisa os pull requests e migrou o CI do rust-bech32 e do corepc para ele."
contributions:
  - id: github-bitcoin-bitcoin-34764
    title:
      EN: Help create RPC `getopenrpcinfo` to make Bitcoin Core's RPC result layouts machine-readable
      BR: Ajudar na criação da RPC `getopenrpcinfo` para tornar os resultados das RPCs do Bitcoin Core legíveis por máquina
    date: '2026-06-19'
    source: 'bitcoin/bitcoin · #34764'
    type: PR
    featured: true
    href: 'https://github.com/bitcoin/bitcoin/pull/34764'
    description:
      EN: Reviewed the new `getopenrpcinfo` RPC over several rounds, generated Rust types from its output to test it, and wrote this change so that it describes every result field.
      BR: Revisou a nova RPC `getopenrpcinfo` em várias rodadas, gerou tipos em Rust a partir da saída para testá-la e escreveu esta mudança para que ela descreva todos os campos de resultado.
  - id: github-rust-bitcoin-rust-bitcoin-6212
    title:
      EN: Validate the master key seed length
      BR: Validar o comprimento da seed da chave mestra
    date: '2026-05-27'
    source: 'rust-bitcoin/rust-bitcoin · #6212'
    type: PR
    href: 'https://github.com/rust-bitcoin/rust-bitcoin/pull/6212'
    description:
      EN: Introduces a validated BIP32 seed type that rejects invalid lengths at construction.
      BR: Introduz um tipo de seed BIP32 validado que rejeita comprimentos inválidos na
        construção.
  - id: github-rust-bitcoin-rust-bitcoin-6923
    title:
      EN: Fix work and target conversion for small values
      BR: Corrigir a conversão entre work e target para valores pequenos
    date: '2026-09-27'
    source: 'rust-bitcoin/rust-bitcoin · #6923'
    type: PR
    href: 'https://github.com/rust-bitcoin/rust-bitcoin/pull/6923'
    description:
      EN: Proof of work math disagreed with Bitcoin Core for small values.
      BR: A conta de proof of work divergia do Bitcoin Core para valores pequenos.
  - id: github-rust-bitcoin-rust-bitcoin-6729
    title:
      EN: Daily corpus-based fuzzing
      BR: Fuzzing diário baseado em corpus
    date: '2026-08-23'
    source: 'rust-bitcoin/rust-bitcoin · #6729'
    type: PR
    href: 'https://github.com/rust-bitcoin/rust-bitcoin/pull/6729'
    description:
      EN: Fuzzes daily from a persistent corpus in qa-assets, the repository he started for it, so each run builds on what the previous ones already reached.
      BR: Faz fuzzing diário a partir de um corpus persistente no qa-assets, repositório que ele criou para isso, de modo que cada execução parte do que as anteriores já alcançaram.
  - id: github-rust-bitcoin-rust-bitcoin-6943
    title:
      EN: Test the trait decisions of every public type in units
      BR: Testar as decisões de traits de cada tipo público do units
    date: '2026-09-27'
    source: 'rust-bitcoin/rust-bitcoin · #6943'
    type: PR
    href: 'https://github.com/rust-bitcoin/rust-bitcoin/pull/6943'
    description:
      EN: One test per trait states which public types implement it and which must not, so a missing or accidental implementation fails before the API is considered complete.
      BR: Um teste por trait declara quais tipos públicos o implementam e quais não devem, de modo que uma implementação ausente ou acidental falhe antes da API ser considerada completa.
updatedAt: '2026-11-20'
affiliations:
  - organization: Spiral
    role: { EN: Grantee, BR: Grantee }
    status: current
    start: '2026-09'
---
## EN

Renato Britto (satsfy) is a Spiral grantee working on rust-bitcoin. He is currently preparing the units crate for 1.0, auditing its API and testing it with various techniques, from fuzzing to formal proofs. He is a maintainer of rust-bitcoin-maintainer-tools, reviews the organization's pull requests and contributed to Bitcoin Core. Previously he built authentication at Coinbase.

## PT

Renato Britto (satsfy) é grantee da Spiral e trabalha no rust-bitcoin. Atualmente prepara o crate units para a 1.0, auditando a API e testando com várias técnicas, de fuzzing a provas formais. É maintainer do rust-bitcoin-maintainer-tools, revisa os pull requests da organização e contribuiu ao Bitcoin Core. Antes, trabalhou na Coinbase.
