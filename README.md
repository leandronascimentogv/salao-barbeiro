# Salão / Barbeiro — Aplicativo de Agendamento

Aplicativo de agendamento para salão de beleza e barbearia, feito em
Google Sheets + Google Apps Script, com custo zero de infraestrutura.

## O que faz

- App do dono: agenda, gestão de status, remarcação, análises, backup e lembretes.
- App do cliente: mostra horários livres e registra o agendamento.
- Lembretes por e-mail: confirmação no ato e aviso no dia anterior.
- Análises: receita, ticket médio, no-show e horários de pico.

## Estrutura

    src/    arquivos .gs (Apps Script)
    ui/     arquivos .html (interface)
    docs/   manual do dono

## Planilha central

Abas: Configuracao, Servicos, Profissionais, Clientes, Agendamentos, Analises.

Os nomes das abas e colunas precisam ser exatamente iguais aos usados no código.

## Implantação

1. Crie a planilha modelo e cole os cabeçalhos.
2. Extensões > Apps Script: crie os arquivos de src/ e ui/.
3. Implantar > Nova implantação > Aplicativo da Web.
   Executar como: Eu. Acesso: Qualquer pessoa.
4. App do dono: URL gerada. App do cliente: URL + ?pagina=cliente
5. Rode criarGatilhoLembretes() uma vez.

## Custo

Zero. Usa apenas serviços internos do Apps Script.

## Segurança

Repositório privado, sem dado real. Uma planilha por cliente.
