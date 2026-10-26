# Azul SmartCargo — FIAP + Azul Logística

Plugin local para gerar um protótipo editável no Figma Design. Não requer token, backend, pacotes npm ou acesso à rede. Fonte: Inter.

## Importar

1. Extraia o ZIP mantendo `manifest.json` e `code.js` juntos.
2. No aplicativo desktop do Figma, abra um arquivo de Design vazio.
3. Acesse Plugins → Development → Import plugin from manifest e selecione `manifest.json`.
4. Execute “Azul SmartCargo • FIAP”. Aguarde a criação das páginas.
5. Na página Protótipo, selecione o fluxo “Apresentação • FIAP + Azul” e use Present.

Os nomes dos menus podem variar conforme o idioma. A execução adiciona páginas ao arquivo atual. Execute uma vez em um arquivo vazio para evitar duplicação. O plugin não apaga conteúdo existente.

## Entrega

- Design System: paleta, estilos de texto, componentes de botões e exemplo de card com Auto Layout.
- Telas: 28 frames desktop 1440 × 900, com texto e formas editáveis.
- Protótipo: cópia das telas com conexões internas e ponto de início próprios.
- Botões usam componentes com Auto Layout; conteúdo principal usa posicionamento fixo para desktop. Não há layout responsivo completo.

## Jornada para apresentar

Login → Dashboard → Fila inteligente → Analisar SC-1042 → Iniciar processamento → Confirmar início → Verificar capacidade → Separação → Confirmar alocação → Acompanhar carga → Avançar para Consolidada → Avançar para Pronta → Resultado final → Relatórios atualizados.

Exceções: Capacidade → Consolidação mostra capacidade excedida e mantém ocupação intacta. Análise da SC-1042 mostra risco de atraso. Detalhes → Tentar pular etapa mostra bloqueio de sequência. Cadastro → Validar campos mostra mensagens de erro.

Menu lateral, notificações, busca, filtro de críticas, cadastro, edição demonstrativa e filtro de relatório têm destinos conectados. Confirmações e erros são frames de estado com cards de diálogo, não overlays nativos. Os dados são simulados e as transições são pré-definidas: os campos não aceitam digitação no modo Present, filtros não fazem consultas e os cálculos não são executados em tempo real. Editar os textos no arquivo Design altera a apresentação; isso não implementa lógica de aplicação.

A navegação lateral retorna ao estado inicial de cada módulo. Use os botões da jornada para preservar a continuidade dos estados simulados. O cadastro tem seu próprio ramo, com SC-1046; voltar à lista restaura as quatro cargas iniciais.

## Dados e regras

| Carga | Destino | Voo | Peso | Prazo | Estimativa | Margem | Prioridade |
|---|---|---|---|---|---|---|---|
| SC-1042 | REC | AD 4170 | 420 kg | 20 min | 35 min | −15 min | Crítica |
| SC-1043 | MAO | AD 4382 | 280 kg | 50 min | 30 min | 20 min | Alta |
| SC-1044 | SSA | AD 4028 | 160 kg | 95 min | 40 min | 55 min | Normal |
| SC-1045 | POA | AD 4090 | 310 kg | 120 min | 45 min | 75 min | Normal |

Margem negativa: crítica; margem entre 0 e 30 min inclusive: alta; acima de 30 min: normal. O limite zero foi definido para cobrir a fronteira não explicitada no briefing.

SC-1042 termina em 27 minutos, com 7 minutos de atraso: a conclusão não elimina a ocorrência. O indicador histórico passa de 92/100 para 92/101 = 91,1%. Ocupação de Separação: 28/40 → 32/40; média das quatro áreas: 82,5% → 85%. A finalização significa pronta para embarque e não libera posições automaticamente.

## Validação e limites

Sintaxe JavaScript verificada com Node. Verificação estrutural automatizada usa um simulador da API para executar o gerador, validar os destinos e conferir dimensões e páginas. Isso não substitui execução real no Figma: renderização, disponibilidade da fonte, compatibilidade da API e apresentação precisam de conferência após importar. Não foi criado nem publicado um arquivo .fig nesta sessão.

Identidade inspirada nas cores solicitadas; marca tipográfica conceitual, sem logotipo oficial. Projeto acadêmico com dados fictícios.
