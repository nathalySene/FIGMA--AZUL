# Azul SmartCargo — roteiro de apresentação

PowerPoint com 32 slides. Sugestão: 15–20 minutos para a versão completa; 6–8 minutos usando a jornada principal e omitindo os ramos alternativos. As falas também estão nas notas do apresentador.

## Abertura
Apresentamos uma proposta acadêmica para apoiar a operação de cargas em Viracopos. O protótipo reúne priorização, capacidade e acompanhamento, com dados simulados.

## Slide 3 — Login | Acesso à operação

**Objetivo:** Identificar o operador e apresentar o sistema.

Esta é a entrada da plataforma. O operador encontra uma identidade visual consistente e campos de e-mail e senha. No protótipo, o acesso é demonstrativo: não há autenticação real. A finalidade é mostrar como começa a jornada operacional.

## Slide 4 — Dashboard operacional

**Objetivo:** Transformar dados do terminal em prioridades de ação.

O dashboard oferece uma visão rápida do terminal. As duas cargas prioritárias correspondem a uma crítica e uma alta. A carga pronta não entra nas três ativas. Os gráficos mostram movimentação e distribuição de prioridades; a tabela orienta o operador para a SC-1042. O percentual de 92% representa a base histórica simulada, não apenas as quatro cargas da lista.

## Slide 5 — Central de notificações

**Objetivo:** Reunir situações que exigem atenção.

Esta página reúne alertas em um único local. O vermelho chama atenção para o prazo da SC-1042, enquanto o amarelo indica a área próxima do limite. O operador pode abrir a análise do risco ou consultar a capacidade. O aviso de carga pronta completa a visão operacional.

## Slide 6 — Gestão de cargas

**Objetivo:** Centralizar consulta e manutenção dos registros.

A tabela concentra os dados das quatro cargas do cenário. Cada registro traz identificação, destino, voo, peso, etapa e prioridade. A tela oferece busca, filtro de críticas, cadastro e acesso aos detalhes. Isso reduz a necessidade de procurar informações em controles separados.

## Slide 7 — Resultado da busca

**Objetivo:** Encontrar rapidamente a carga relevante.

Este estado demonstra a lista filtrada, exibindo somente a carga crítica SC-1042. O operador pode abrir seus detalhes ou limpar os filtros. No protótipo, o resultado é pré-definido; a consulta dinâmica será parte da implementação futura.

## Slide 8 — Cadastro de carga

**Objetivo:** Registrar os dados necessários ao planejamento.

O cadastro reúne os dados que permitem planejar o processamento. O prazo disponível e a estimativa de duração sustentam a classificação da prioridade. Este formulário demonstra a SC-1046, em um ramo separado da jornada principal. Os campos são visuais no modo de apresentação.

## Slide 9 — Validação do cadastro

**Objetivo:** Evitar informações incompletas ou inválidas.

Aqui mostramos uma tentativa inválida. As mensagens explicam o que precisa ser corrigido, como o formato do AWB, peso positivo e preenchimento dos dados obrigatórios. São estados de erro desenhados, e não validações executadas em tempo real. A regra deverá ser implementada no sistema.

## Slide 10 — Cadastro concluído

**Objetivo:** Confirmar o registro e sua classificação.

A confirmação apresenta a nova carga SC-1046, com 200 quilos. Como o prazo é de 90 minutos e a estimativa é de 40, a margem é de 50 minutos e a prioridade é normal. Este é um ramo de demonstração: voltar à lista restaura as quatro cargas originais.

## Slide 11 — Detalhes da carga

**Objetivo:** Oferecer uma visão individual e rastreável.

Nos detalhes, o operador consulta os dados completos da SC-1042 e seu estado inicial, Recebida. A linha do tempo indica as etapas previstas e o histórico registra as ações. Há acesso à edição e ao avanço de etapa. O indicador crítico continua visível para contextualizar a decisão.

## Slide 12 — Edição da carga

**Objetivo:** Demonstrar a revisão dos dados operacionais.

A edição concentra as informações que poderiam ser revisadas pelo operador. Neste protótipo, o botão salva sem alterações para preservar a coerência dos dados entre as telas. A edição livre e o recálculo automático da prioridade ficam para a implementação em código.

## Slide 13 — Fila inteligente de priorização

**Objetivo:** Ordenar a atenção segundo a margem de tempo.

A fila organiza as cargas em crítica, alta e normal. A regra compara prazo disponível e tempo estimado. Uma margem negativa indica crítica; de zero a trinta minutos, alta; acima disso, normal. Cada card apresenta os dados que justificam a prioridade, permitindo uma decisão transparente.

## Slide 14 — Análise da carga crítica

**Objetivo:** Explicar o risco antes de agir.

A SC-1042 tem vinte minutos disponíveis, mas exige trinta e cinco minutos estimados. A margem de menos quinze minutos mostra o risco de atraso. A tela recomenda priorização e verificação de capacidade. Esse risco é uma projeção: o atraso efetivo só será conhecido ao concluir a operação.

## Slide 15 — Análise da prioridade alta

**Objetivo:** Mostrar uma carga com pouca folga.

A SC-1043 tem cinquenta minutos disponíveis e trinta minutos estimados de processamento. Como a margem é de vinte minutos, ela entra na prioridade alta. Existe tempo disponível, mas a folga é pequena. Este exemplo ajuda a comparar a classificação com a carga crítica.

## Slide 16 — Análise da prioridade normal

**Objetivo:** Demonstrar uma situação com margem maior.

A SC-1044 apresenta margem de cinquenta e cinco minutos, calculada a partir de noventa e cinco minutos disponíveis e quarenta estimados. Por superar trinta minutos, a prioridade é normal. Isso permite concentrar a atenção nas cargas mais urgentes sem perder a visibilidade das demais.

## Slide 17 — Confirmação do processamento

**Objetivo:** Garantir uma decisão consciente do operador.

Antes de iniciar, o sistema reapresenta a carga e o risco. A confirmação torna explícito que o status passará de Recebida para Em separação e que a ação será registrada. O operador também pode cancelar. No arquivo, esta confirmação é um frame de estado, não um modal nativo.

## Slide 18 — Processamento iniciado

**Objetivo:** Confirmar a ação e orientar o próximo passo.

Após confirmar, a interface informa que Mariana Silva iniciou a separação às dez e cinco. A mensagem confirma o registro e direciona o operador à capacidade operacional. No cenário desenhado, a separação começa antes da confirmação da alocação; uma versão futura deve avaliar se a reserva precisa anteceder essa mudança.

## Slide 19 — Capacidade operacional

**Objetivo:** Verificar espaço antes de alocar uma carga.

O painel mostra recebimento, separação, consolidação e pré-embarque. Cada área apresenta ocupação e limite. A Separação tem doze posições disponíveis; a Consolidação tem apenas uma. Como a SC-1042 exige quatro posições, podemos demonstrar tanto uma alocação possível quanto uma operação bloqueada.

## Slide 20 — Simulação de alocação

**Objetivo:** Antecipar o impacto sem reservar espaço.

A simulação mostra o impacto da alocação: vinte e oito posições ocupadas passam a trinta e duas, dentro do limite de quarenta. O saldo será de oito posições. Até confirmar, não há reserva. Esse passo permite revisar o destino e cancelar sem alterar a ocupação.

## Slide 21 — Exceção | Capacidade excedida

**Objetivo:** Impedir uma alocação além do limite.

Este é o cenário alternativo de erro. A Consolidação tem uma posição livre, mas a carga necessita de quatro. Faltam três posições e a operação é bloqueada, preservando a ocupação. O operador deve escolher outra área ou aguardar espaço. Não houve alocação parcial.

## Slide 22 — Alocação concluída

**Objetivo:** Confirmar a ocupação e manter a jornada.

Após a confirmação, a Separação passa a ter trinta e duas das quarenta posições ocupadas, ou oitenta por cento. A interface confirma a alocação da SC-1042 e direciona ao acompanhamento. As demais áreas mantêm a ocupação do cenário inicial.

## Slide 23 — Acompanhamento | Em separação

**Objetivo:** Mostrar o início da execução e seu registro.

A linha do tempo indica que a carga foi recebida e está em separação. O histórico inclui o início do processamento e a confirmação da alocação. O operador pode avançar para a próxima etapa permitida. A consulta do histórico dá rastreabilidade à movimentação.

## Slide 24 — Exceção | Transição não permitida

**Objetivo:** Preservar a ordem do processamento.

Este estado demonstra a proteção da sequência operacional. Não é permitido saltar diretamente para uma etapa posterior. A carga deve passar por Recebida, Em separação, Consolidada e Pronta para embarque. O bloqueio explica o motivo e oferece retorno ao acompanhamento; no protótipo, o retorno leva aos detalhes iniciais.

## Slide 25 — Acompanhamento | Consolidada

**Objetivo:** Registrar o avanço intermediário.

A carga avança para Consolidada e recebe um novo registro às dez e dezessete. A linha do tempo torna o progresso visível. O card de área ainda exibe Separação porque o protótipo não simula transferências físicas entre áreas. Status do processo e posição alocada são informações distintas neste cenário.

## Slide 26 — Acompanhamento | Pronta para embarque

**Objetivo:** Concluir o escopo do processamento.

Às dez e vinte e sete, a carga está pronta para embarque e todas as etapas estão registradas. Isso conclui o escopo de processamento apresentado. Não significa que a aeronave decolou ou que houve entrega ao destinatário. A liberação de posições não foi simulada automaticamente.

## Slide 27 — Resultado da operação

**Objetivo:** Apresentar o desfecho com transparência.

A operação termina em vinte e sete minutos, contra um prazo inicial de vinte. O atraso efetivo é de sete minutos. A carga deixa a lista de críticas ativas por estar pronta, mas a ocorrência não desaparece. O resultado demonstra rastreabilidade; não comprova que a solução eliminou atrasos.

## Slide 28 — Relatórios operacionais

**Objetivo:** Estabelecer a visão histórica de desempenho.

O relatório inicial apresenta a base histórica simulada: cem cargas concluídas, das quais noventa e duas no prazo. A ocupação média inicial das quatro áreas é de oitenta e dois vírgula cinco por cento. Os gráficos e ocorrências contextualizam a operação, mas são dados ilustrativos do protótipo.

## Slide 29 — Relatório do turno

**Objetivo:** Consultar um recorte das cargas apresentadas.

O filtro de turno mostra as quatro cargas do conjunto inicial, com peso total de mil cento e setenta quilos. Uma carga está pronta e uma é crítica. Este recorte não deve ser confundido com a base histórica de cem cargas. Na navegação do protótipo, o filtro abre um estado pré-definido.

## Slide 30 — Relatórios após a conclusão

**Objetivo:** Registrar o impacto da carga finalizada.

Com a SC-1042 concluída em atraso, a base histórica passa a cento e uma cargas e continua com noventa e duas no prazo. Por isso, o percentual cai para noventa e um vírgula um por cento. A ocupação média sobe para oitenta e cinco por cento. A média de trinta e um minutos é ilustrativa e não é derivável da base exibida; precisará ser recalculada com dados completos na implementação.

## Encerramento

A solução demonstra como tornar as decisões mais claras e rastreáveis. Os benefícios operacionais precisam ser validados com uso real. A próxima etapa é implementar as regras e integrar os estados apresentados.

## Observações para perguntas da banca

- O envio contém 28 PNGs; não permite auditar a navegação do Figma.
- A regra de margem zero foi definida como prioridade alta.
- Conclusão não significa ausência de atraso: a SC-1042 termina 7 minutos depois do prazo.
- O tempo médio final de 31 min é ilustrativo; a base exibida não permite justificá-lo a partir de 32 min em 100 cargas mais uma de 27 min. Com valores exatos, isso seria aproximadamente 31,95 min.
- O gráfico final permanece visualmente igual ao inicial: na implementação deve ser sincronizado ao indicador de 91,1%.
- A etapa Consolidada ainda mostra área Separação; transferência física e liberação de posições não foram simuladas.
- O protótipo registra início antes da alocação; a ordem deve ser validada com operadores.