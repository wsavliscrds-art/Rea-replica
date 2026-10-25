# REA Replica

[English (US)](README.md)

REA Replica é uma skill do Codex que combina análise autorizada de artefatos com REA e o fluxo Replica de reconstrução clean-room de aplicativos.

## O que ela faz

- Encaminha pesquisa pública do produto e comportamento visível ao usuário para `replica-recon`.
- Usa `reverse-engineer-anything` quando uma conclusão depende de evidências autorizadas de binários, pacotes, firmware, código gerenciado, JavaScript/Electron, execução ou comparação de versões.
- Separa observações, inferências e pontos desconhecidos.
- Transforma evidências em requisitos independentes, contratos de interface e resultados testáveis.
- Coordena arquitetura, design, implementação, backend, testes, marca, lançamento e implantação por meio das skills `replica-*` instaladas.
- Impede que código-fonte proprietário, código decompilado, APIs privadas, credenciais, recursos visuais, marcas ou textos distintivos entrem no produto reconstruído.

## Idiomas

A skill responde no idioma do usuário e oferece suporte explícito a inglês dos Estados Unidos e português do Brasil. Nomes de ferramentas, nomes de skills, caminhos, Evidence IDs, identificadores de APIs e código permanecem inalterados.

## Requisitos

Instale e configure:

- `reverse-engineer-anything`
- A coleção de skills Replica (`replica-*`)
- As ferramentas REA quando a análise de artefatos for necessária

Este repositório coordena essas dependências; ele não as inclui.

## Instalação

Clone o repositório no diretório de skills do Codex usando o nome de pasta `rea-replica`:

```bash
git clone https://github.com/wsavliscrds-art/Rea-replica.git ~/.codex/skills/rea-replica
```

No Windows PowerShell:

```powershell
git clone https://github.com/wsavliscrds-art/Rea-replica.git "$env:USERPROFILE\.codex\skills\rea-replica"
```

Inicie uma nova mensagem no Codex após a instalação.

## Uso

```text
Use $rea-replica para analisar este aplicativo e planejar uma reconstrução clean-room.
```

A skill também pode ser selecionada automaticamente quando o pedido corresponder à sua descrição.

## Uso responsável

Analise somente artefatos que você possui, tem autorização para inspecionar ou pode estudar legitimamente para interoperabilidade, compatibilidade, preservação ou pesquisa de segurança. Nunca contorne autenticação, paywalls, licenciamento ou controles de acesso.

O produto reconstruído deve usar código novo, marca própria e recursos originais. As evidências da REA descrevem comportamento e restrições; elas não são código-fonte para o substituto.

## Licença

MIT. Consulte [LICENSE](LICENSE).
