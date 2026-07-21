<div align="center">

<img src="./assets/pinker-banner.svg" width="100%" alt="Lyanna Valerie — Pinker, compiladores, runtimes e sistemas">

<br>

# Lyanna Valerie

### Linguagens, compiladores e sistemas construídos de baixo para cima.

[![Pinker](https://img.shields.io/badge/Pinker-linguagem_autoral-ff4fa3?style=for-the-badge&labelColor=17121b)](https://github.com/LyannaValerie/pinker-v0)
![Rust](https://img.shields.io/badge/Rust-compiladores-ff73b8?style=for-the-badge&logo=rust&logoColor=white&labelColor=17121b)
![C](https://img.shields.io/badge/C-runtime_e_sistemas-e85d9e?style=for-the-badge&logo=c&logoColor=white&labelColor=17121b)
![Assembly](https://img.shields.io/badge/Assembly-x86--64-c94c8d?style=for-the-badge&labelColor=17121b)
![Linux](https://img.shields.io/badge/Linux-ambiente_nativo-b83d7d?style=for-the-badge&logo=linux&logoColor=white&labelColor=17121b)

</div>

---

## `01.` Pesquisa em andamento

Sou pesquisadora e desenvolvedora independente. Meu trabalho conecta matemática, lógica e arquitetura de computadores à construção concreta de linguagens, compiladores, runtimes e sistemas operacionais.

```text
lógica booleana
    ↓
circuitos e arquitetura
    ↓
assembly e representação de máquina
    ↓
compiladores, runtimes e ABIs
    ↓
sistemas operacionais e self-hosting
```

Não estudo essas camadas como assuntos isolados. O objetivo é compreender os contratos entre elas e transformar esse entendimento em ferramentas e sistemas autorais.

---

## `02.` Pinker

> Uma linguagem de programação autoral em português, concebida para ser tecnicamente auditável, lexicalmente soberana e capaz de crescer até controlar a própria implementação.

[**`pinker-v0`**](https://github.com/LyannaValerie/pinker-v0) é a base factual atual da linguagem:

- frontend e compilador escritos em **Rust**;
- interpretador para a superfície estável;
- AST tipada, IR textual, CFG IR e máquina abstrata auditáveis;
- backend nativo próprio;
- geração de executáveis **ELF Linux x86-64 System V**;
- runtime nativo `pinker_rt`;
- verificação de paridade entre execução interpretada e nativa nos recortes compatíveis.

```text
fonte .pink
  └─► lexer / parser com spans
       └─► AST tipada e validada
            └─► IR textual / CFG IR
                 └─► máquina abstrata
                      ├─► interpretador
                      └─► assembly x86-64
                           └─► ELF + pinker_rt
```

### Pequeno fragmento da linguagem

```pinker
pacote laboratorio;

carinho principal() -> bombom {
    falar("uma linguagem deve conhecer a máquina que a sustenta");
    retornar 0;
}
```

> **Estado honesto:** Pinker v0 ainda não é uma linguagem de propósito geral nem um compilador de produção. O alvo nativo atual é Linux x86-64 System V. Self-hosting, freestanding e sistema operacional pertencem à direção futura, não ao estado já implementado.

---

## `03.` Três responsabilidades

<table>
<tr>
<td width="33%" valign="top">

### Engine

Implementação factual:

- compilador;
- interpretador;
- IRs;
- backend;
- runtime;
- testes;
- ferramentas.

</td>
<td width="33%" valign="top">

### Rosa

Direção e julgamento:

- identidade;
- vocabulário;
- intenção;
- coerência;
- soberania lexical;
- verdade técnica.

</td>
<td width="33%" valign="top">

### Guardião Pinker

Verificação determinística:

- contratos;
- invariantes;
- conformidade;
- critérios de evolução;
- separação entre fato e visão.

</td>
</tr>
</table>

---

## `04.` Laboratório técnico

```text
Pinker/
├── linguagens de programação
├── compiladores e interpretadores
├── sistemas de tipos e semântica
├── IR, CFG e geração de código
├── runtimes, ABIs e formatos binários
├── arquitetura de computadores
├── assembly, C e Rust
├── Linux From Scratch e OSDev
├── segurança e sistemas de baixo nível
└── agentes de IA para engenharia de software
```

Também estudo a linha contínua do **Nand2Tetris**:

```text
NAND → circuitos → CPU → assembly → VM → compilador → sistema
```

---

## `05.` Princípios de construção

```rust
struct Pesquisa {
    verdade_tecnica: Evidencia,
    abstracao: Contrato,
    implementacao: Sistema,
    identidade: Intencao,
}

fn evoluir(projeto: &mut Projeto) {
    localizar();
    inspecionar();
    extrair();
    classificar();
    planejar();
    alterar();
    validar();
    revisar();
    relatar();
}
```

- visão não é tratada como implementação;
- abstrações devem preservar os contratos das camadas inferiores;
- uma entrega precisa atravessar o caminho completo, não apenas aparentar progresso;
- nomes fazem parte da arquitetura;
- ferramentas devem ampliar autonomia, não esconder funcionamento.

---

## `06.` Projetos públicos

<a href="https://github.com/LyannaValerie/pinker-v0">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=LyannaValerie&repo=pinker-v0&theme=radical&hide_border=true&bg_color=17121B&title_color=FF73B8&icon_color=FF4FA3&text_color=F7D8E8" alt="Repositório Pinker v0">
</a>
<a href="https://github.com/LyannaValerie/mapinhas">
  <img src="https://github-readme-stats.vercel.app/api/pin/?username=LyannaValerie&repo=mapinhas&theme=radical&hide_border=true&bg_color=17121B&title_color=FF73B8&icon_color=FF4FA3&text_color=F7D8E8" alt="Repositório Mapinhas">
</a>

---

<div align="center">

<img src="./assets/pinker-divider.svg" width="100%" alt="Divisor visual Pinker">

### `do bit ao sistema · da ideia ao contrato · do contrato à máquina`

**Construindo Pinker sem esconder as camadas que tornam uma linguagem possível.**

</div>
