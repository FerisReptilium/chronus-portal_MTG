# CHRONUS — MTG Portal

Portal de fichas para a campanha CHRONUS adaptada ao universo de Magic: The Gathering.

## Estado atual

- Portal inicial com 10 slots de jogadores.
- Ficha baseada no modelo oficial enviado para este projeto.
- Slots 1–10 acessíveis por URL: `ficha.html?slot=N`.
- Salvamento local independente por personagem.
- Retrato, temas das cinco cores de mana + incolor.
- Feridas, condições, mana, XP, equipamentos, magias, diário.
- Rolagem de testes e iluminação.
- Importação/exportação JSON.
- Exportação PDF no navegador.

## Próxima arquitetura

```
Portal
├── Campanhas
├── 10 personagens
├── Fichas
├── Cartas / Grimório
├── Mesa online
├── Rolador
└── Supabase
    ├── Auth
    ├── characters
    ├── campaigns
    ├── campaign_players
    ├── spells
    └── inventory
```

O banco remoto ainda não é alterado porque o projeto Supabase informado não está acessível pela conexão atual. Nenhuma chave secreta é armazenada neste repositório.

## Fonte da ficha

A interface e os campos partem do arquivo `ficha_final_Revisada_MTG.html` fornecido pelo mestre. Alterações futuras devem preservar a terminologia e as regras definidas na ficha antes de adicionar novas mecânicas.
