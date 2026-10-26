# Azul SmartCargo — roteiro de apresentação

41 slides: contexto e negócio, 28 telas e encerramento. Versão completa: aproximadamente 25–30 minutos. Para uma apresentação de 10–12 minutos, priorize problema, proposta de valor, indicadores e piloto; depois demonstre a jornada SC-1042 e encerre. As falas também estão nas notas do PowerPoint.

## Slide 1 — VIRACOPOS  /  GESTÃO DE CARGAS AÉREAS

Apresentamos o Azul SmartCargo, proposta acadêmica do Challenge FIAP e Azul Logística. Primeiro explicamos o problema, o valor de negócio e como validá-lo. Depois percorremos as 28 telas com dados simulados. Os benefícios são hipóteses, não resultados medidos da operação real.

## Slide 2 — Mais eficiência no espaço que já existe.

O desafio é organizar urgências e usar melhor o espaço existente. A proposta reúne priorização, capacidade e acompanhamento. Redução de atrasos é um benefício esperado a validar, e não um resultado comprovado pelo protótipo.

## Slide 3 — O problema que o negócio precisa resolver

O briefing apresenta o desafio de reduzir atrasos e melhorar a eficiência sem ampliar a área física. Partimos da hipótese de que falta de visibilidade compartilhada e decisões desconectadas podem dificultar a priorização. Não realizamos entrevistas nem medimos a operação real da Azul. Estas causas e impactos devem ser investigados no diagnóstico com operadores e gestores.

## Slide 4 — Quem usa e quem decide

Os perfis são propostos para orientar a descoberta, não personas validadas. O operador usa a ferramenta no dia a dia. O supervisor coordena exceções, capacidade e equipes. O gestor acompanha desempenho e pode patrocinar o piloto. Aprovação, orçamento e responsabilidades precisam ser confirmados com a organização.

## Slide 5 — Proposta de valor

O valor proposto é conectar prioridade, capacidade e execução. A classificação por margem é uma regra transparente, não um modelo de inteligência artificial. O operador continua responsável pelas decisões. O diferencial apresentado é a combinação das informações em uma mesma jornada, e não uma comparação comprovada com os sistemas atualmente utilizados pela Azul.

## Slide 6 — Como a proposta muda a decisão

A coluna de risco representa uma situação hipotética de baixa visibilidade, não uma afirmação sobre o modo como a Azul trabalha. O piloto deve verificar se a equipe hoje enfrenta essas dificuldades e se a proposta melhora a decisão. O valor só se confirma quando o uso real muda os indicadores sem criar novos gargalos.

## Slide 7 — Benefícios esperados e seus mecanismos

Os benefícios são hipóteses. A fila pode reduzir espera das urgentes; o bloqueio de capacidade pode reduzir alocações inadequadas; o histórico pode reduzir tempo gasto procurando informações. Nenhum percentual de ganho foi medido. Mesmo uma carga concluída pode terminar em atraso, como ocorre com a SC-1042.

## Slide 8 — Como medir se a solução funciona

Antes do piloto, definir os eventos e timestamps: recebida, início de separação, consolidada e pronta. Pontualidade compara o instante pronta com o prazo acordado. O tempo médio usa a mesma janela e as mesmas regras para todos os registros. Ocupação deve ser acompanhada ao longo do turno, e não só em uma captura de tela. Metas numéricas serão acordadas após medir a linha de base. Os indicadores do protótipo são fictícios e não servem como baseline.

## Slide 9 — Viabilidade e retorno do investimento

Não há informação validada de orçamento, custos ou volume financeiro. O modelo é de uso interno: não presumimos receita de assinatura. Estimar horas efetivamente economizadas, verificar se são convertidas em capacidade ou redução de custo, e evitar contar o mesmo ganho duas vezes. ROI é benefícios menos custos dividido pelos custos no mesmo período. Se houver ganhos anuais e investimento inicial, o payback depende do fluxo líquido; só calcular após validar valores e recorrência.

## Slide 10 — Plano de validação do piloto

Primeiro observar o processo e entrevistar operadores e gestores, definindo indicadores e linha de base. Depois testar usabilidade com cenários de carga crítica, capacidade excedida e sequência inválida. O piloto operacional deve ter um recorte de área ou turno, dados confiáveis e comparação controlada por perfil de carga. Sem melhora sustentada e sem aceitação dos operadores, revisar antes de expandir. Critérios e metas precisam ser acordados, não inventados nesta apresentação.

## Slide 11 — MVP, dependências e limites

O MVP inclui cadastro, consulta, fila por margem, capacidade e acompanhamento. A implementação pode começar com HTML, CSS, JavaScript e Tailwind e dados simulados; persistência, perfis, auditoria e integrações exigem definição adicional antes de uso operacional. Capacidade e estimativas precisam ser confiáveis. Não estamos prometendo previsão com IA, otimização automática de toda a operação ou ampliação física.

## Slide 12 — Login / Acesso à operação

Esta é a entrada da plataforma. O operador encontra uma identidade visual consistente e campos de e-mail e senha. No protótipo, o acesso é demonstrativo: não há autenticação real. A finalidade é mostrar como começa a jornada operacional.

## Slide 13 — Dashboard operacional

O dashboard oferece uma visão rápida do terminal. As duas cargas prioritárias correspondem a uma crítica e uma alta. A carga pronta não entra nas três ativas. Os gráficos mostram movimentação e distribuição de prioridades; a tabela orienta o operador para a SC-1042. O percentual de 92% representa a base histórica simulada, não apenas as quatro cargas da lista.

## Slide 14 — Central de notificações

Esta página reúne alertas em um único local. O vermelho chama atenção para o prazo da SC-1042, enquanto o amarelo indica a área próxima do limite. O operador pode abrir a análise do risco ou consultar a capacidade. O aviso de carga pronta completa a visão operacional.

## Slide 15 — Gestão de cargas

A tabela concentra os dados das quatro cargas do cenário. Cada registro traz identificação, destino, voo, peso, etapa e prioridade. A tela oferece busca, filtro de críticas, cadastro e acesso aos detalhes. Isso reduz a necessidade de procurar informações em controles separados.

## Slide 16 — Resultado da busca

Este estado demonstra a lista filtrada, exibindo somente a carga crítica SC-1042. O operador pode abrir seus detalhes ou limpar os filtros. No protótipo, o resultado é pré-definido; a consulta dinâmica será parte da implementação futura.

## Slide 17 — Cadastro de carga

O cadastro reúne os dados que permitem planejar o processamento. O prazo disponível e a estimativa de duração sustentam a classificação da prioridade. Este formulário demonstra a SC-1046, em um ramo separado da jornada principal. Os campos são visuais no modo de apresentação.

## Slide 18 — Validação do cadastro

Aqui mostramos uma tentativa inválida. As mensagens explicam o que precisa ser corrigido, como o formato do AWB, peso positivo e preenchimento dos dados obrigatórios. São estados de erro desenhados, e não validações executadas em tempo real. A regra deverá ser implementada no sistema.

## Slide 19 — Cadastro concluído

A confirmação apresenta a nova carga SC-1046, com 200 quilos. Como o prazo é de 90 minutos e a estimativa é de 40, a margem é de 50 minutos e a prioridade é normal. Este é um ramo de demonstração: voltar à lista restaura as quatro cargas originais.

## Slide 20 — Detalhes da carga

Nos detalhes, o operador consulta os dados completos da SC-1042 e seu estado inicial, Recebida. A linha do tempo indica as etapas previstas e o histórico registra as ações. Há acesso à edição e ao avanço de etapa. O indicador crítico continua visível para contextualizar a decisão.

## Slide 21 — Edição da carga

A edição concentra as informações que poderiam ser revisadas pelo operador. Neste protótipo, o botão salva sem alterações para preservar a coerência dos dados entre as telas. A edição livre e o recálculo automático da prioridade ficam para a implementação em código.

## Slide 22 — Fila inteligente de priorização

A fila organiza as cargas em crítica, alta e normal. A regra compara prazo disponível e tempo estimado. Uma margem negativa indica crítica; de zero a trinta minutos, alta; acima disso, normal. Cada card apresenta os dados que justificam a prioridade, permitindo uma decisão transparente.

## Slide 23 — Análise da carga crítica

A SC-1042 tem vinte minutos disponíveis, mas exige trinta e cinco minutos estimados. A margem de menos quinze minutos mostra o risco de atraso. A tela recomenda priorização e verificação de capacidade. Esse risco é uma projeção: o atraso efetivo só será conhecido ao concluir a operação.

## Slide 24 — Análise da prioridade alta

A SC-1043 tem cinquenta minutos disponíveis e trinta minutos estimados de processamento. Como a margem é de vinte minutos, ela entra na prioridade alta. Existe tempo disponível, mas a folga é pequena. Este exemplo ajuda a comparar a classificação com a carga crítica.

## Slide 25 — Análise da prioridade normal

A SC-1044 apresenta margem de cinquenta e cinco minutos, calculada a partir de noventa e cinco minutos disponíveis e quarenta estimados. Por superar trinta minutos, a prioridade é normal. Isso permite concentrar a atenção nas cargas mais urgentes sem perder a visibilidade das demais.

## Slide 26 — Confirmação do processamento

Antes de iniciar, o sistema reapresenta a carga e o risco. A confirmação torna explícito que o status passará de Recebida para Em separação e que a ação será registrada. O operador também pode cancelar. No arquivo, esta confirmação é um frame de estado, não um modal nativo.

## Slide 27 — Processamento iniciado

Após confirmar, a interface informa que Mariana Silva iniciou a separação às dez e cinco. A mensagem confirma o registro e direciona o operador à capacidade operacional. No cenário desenhado, a separação começa antes da confirmação da alocação; uma versão futura deve avaliar se a reserva precisa anteceder essa mudança.

## Slide 28 — Capacidade operacional

O painel mostra recebimento, separação, consolidação e pré-embarque. Cada área apresenta ocupação e limite. A Separação tem doze posições disponíveis; a Consolidação tem apenas uma. Como a SC-1042 exige quatro posições, podemos demonstrar tanto uma alocação possível quanto uma operação bloqueada.

## Slide 29 — Simulação de alocação

A simulação mostra o impacto da alocação: vinte e oito posições ocupadas passam a trinta e duas, dentro do limite de quarenta. O saldo será de oito posições. Até confirmar, não há reserva. Esse passo permite revisar o destino e cancelar sem alterar a ocupação.

## Slide 30 — Exceção / Capacidade excedida

Este é o cenário alternativo de erro. A Consolidação tem uma posição livre, mas a carga necessita de quatro. Faltam três posições e a operação é bloqueada, preservando a ocupação. O operador deve escolher outra área ou aguardar espaço. Não houve alocação parcial.

## Slide 31 — Alocação concluída

Após a confirmação, a Separação passa a ter trinta e duas das quarenta posições ocupadas, ou oitenta por cento. A interface confirma a alocação da SC-1042 e direciona ao acompanhamento. As demais áreas mantêm a ocupação do cenário inicial.

## Slide 32 — Acompanhamento / Em separação

A linha do tempo indica que a carga foi recebida e está em separação. O histórico inclui o início do processamento e a confirmação da alocação. O operador pode avançar para a próxima etapa permitida. A consulta do histórico dá rastreabilidade à movimentação.

## Slide 33 — Exceção / Transição não permitida

Este estado demonstra a proteção da sequência operacional. Não é permitido saltar diretamente para uma etapa posterior. A carga deve passar por Recebida, Em separação, Consolidada e Pronta para embarque. O bloqueio explica o motivo e oferece retorno ao acompanhamento; no protótipo, o retorno leva aos detalhes iniciais.

## Slide 34 — Acompanhamento / Consolidada

A carga avança para Consolidada e recebe um novo registro às dez e dezessete. A linha do tempo torna o progresso visível. O card de área ainda exibe Separação porque o protótipo não simula transferências físicas entre áreas. Status do processo e posição alocada são informações distintas neste cenário.

## Slide 35 — Acompanhamento / Pronta para embarque

Às dez e vinte e sete, a carga está pronta para embarque e todas as etapas estão registradas. Isso conclui o escopo de processamento apresentado. Não significa que a aeronave decolou ou que houve entrega ao destinatário. A liberação de posições não foi simulada automaticamente.

## Slide 36 — Resultado da operação

A operação termina em vinte e sete minutos, contra um prazo inicial de vinte. O atraso efetivo é de sete minutos. A carga deixa a lista de críticas ativas por estar pronta, mas a ocorrência não desaparece. O resultado demonstra rastreabilidade; não comprova que a solução eliminou atrasos.

## Slide 37 — Relatórios operacionais

O relatório inicial apresenta a base histórica simulada: cem cargas concluídas, das quais noventa e duas no prazo. A ocupação média inicial das quatro áreas é de oitenta e dois vírgula cinco por cento. Os gráficos e ocorrências contextualizam a operação, mas são dados ilustrativos do protótipo.

## Slide 38 — Relatório do turno

O filtro de turno mostra as quatro cargas do conjunto inicial, com peso total de mil cento e setenta quilos. Uma carga está pronta e uma é crítica. Este recorte não deve ser confundido com a base histórica de cem cargas. Na navegação do protótipo, o filtro abre um estado pré-definido.

## Slide 39 — Relatórios após a conclusão

Com a SC-1042 concluída em atraso, a base histórica passa a cento e uma cargas e continua com noventa e duas no prazo. Por isso, o percentual cai para noventa e um vírgula um por cento. A ocupação média sobe para oitenta e cinco por cento. A média de trinta e um minutos é ilustrativa e não é derivável da base exibida; precisará ser recalculada com dados completos na implementação.

## Slide 40 — Da urgência ao resultado.

Para uma apresentação curta, siga este caminho e abra os cenários de exceção apenas quando necessário. Use os botões da jornada, pois o menu pode retornar aos estados iniciais. Cadastro e tentativa de alocação na Consolidação são ramos alternativos.

## Slide 41 — Decisões claras.
Operação rastreável.

O material enviado contém imagens exportadas. A apresentação explica esses estados sem verificar a navegação do arquivo Figma. Regras e dados são simulados. A SC-1042 termina com sete minutos de atraso; concluída não significa no prazo. Precisamos integrar estados, ajustar indicadores e testar com operadores antes de afirmar ganhos reais.

## Cuidados na defesa

- As causas operacionais e os ganhos são hipóteses do projeto; não foram validados com dados reais da Azul.
- Não há ROI, orçamento ou metas numéricas aprovados.
- Os gráficos e indicadores das telas são simulados. A média final de 31 min e o gráfico de pontualidade precisam ser reconciliados na implementação.
- A SC-1042 termina 7 min atrasada, embora deixe de ser uma crítica ativa.
- Transferência física entre áreas, liberação de posições e integração dos estados ainda precisam ser implementadas.
- Os arquivos enviados pelo usuário eram PNGs: esta apresentação não comprova a navegação no Figma.