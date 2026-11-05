# Auditoria de tráfego Wave

Skill para auditar contas de **Google Ads** e **Meta Ads**, criada pela Wave Marketing para os tipos de cliente que a agência atende: saúde, estúdios e clínicas locais, serviços profissionais regulados, varejo, projetos de alto valor, educação e B2B.

A auditoria é **só de leitura**. A skill não altera campanha, verba, lance, anúncio ou conversão, não envia mensagens e só testa formulário com autorização. Toda mudança vira um item do plano de ação, para uma pessoa aplicar.

## O que ela entrega

- **Saúde e cobertura por bloco**, separadas. A saúde mostra o que está certo entre o que foi verificado; a cobertura mostra quanto foi possível verificar.
- **Nota geral de 0 a 100**, provisória. Ela só aparece quando há evidência suficiente e tem teto quando a mensuração tem falha crítica.
- **Plano de ação pelo objetivo do cliente**: mais volume, mais qualidade ou menor custo, com a troca de cada ação explícita e metas de 30, 60 e 90 dias.
- **Relatório interno completo** e uma **versão de uma página** para o cliente.
- **Dashboard por cliente**, que acumula as auditorias e mostra a evolução de uma para a outra.

## Como a auditoria funciona

| Etapa | O que verifica |
| --- | --- |
| Ficha do cliente | Perfil, objetivo, conversão que importa, custo por lead aceitável, valor de um cliente, região e verba |
| Mensuração (portão) | Se a conta mede a conversão que gera dinheiro, sem duplicidade e sem contar clique como lead |
| Google Ads | Entrega, lances, termos de pesquisa, negativas, estrutura, Índice de Qualidade, anúncios, verba, Performance Max |
| Meta Ads | Objetivo e evento otimizado, fase de aprendizado, fadiga de criativo, públicos, API de conversões, leads de conversão |
| Pós-clique e atendimento | Páginas de destino, WhatsApp, formulários, agendamento e se as conversões batem com os contatos reais |
| Conformidade | Regras de publicidade dos conselhos profissionais e políticas das plataformas |

Se a mensuração reprovar em item crítico, a auditoria continua, mas os blocos seguintes saem marcados como provisórios.

## Princípios

- **Nada de número inventado.** O que não foi visto nos dados aparece como FALTANDO.
- **Nenhum limite universal.** Um CPA ou CTR é bom ou ruim em relação à meta do cliente e ao histórico da própria conta, não a uma média de mercado.
- **Pouco dado não prova desperdício.** A skill calcula quantos cliques sem conversão são necessários antes de chamar um termo de desperdício.
- **Recurso novo não é critério de saúde.** A conta só reprova pelo que comprovadamente atrapalha o resultado ou a medição.
- **Dados pessoais protegidos.** Nada de nome, telefone ou conversa de paciente ou cliente final no relatório.

## Conselhos profissionais cobertos

Medicina (CFM), psicologia (CFP), odontologia (CFO), fisioterapia e terapia ocupacional (COFFITO), nutrição (CFN), biomedicina (CFBM), enfermagem (COFEN), farmácia (CFF), medicina veterinária (CFMV), educação física (CONFEF), advocacia (OAB), contabilidade (CFC) e corretagem de imóveis (COFECI).

Arquitetura, fonoaudiologia, engenharia e mercado financeiro ainda não foram verificados. Para essas profissões, a skill aplica as regras gerais (CDC, LGPD e políticas das plataformas) e marca a regra do conselho como FALTANDO.

## Fontes

As regras de plataforma vêm da documentação oficial do Google Ads e do Meta, e as regras de conselho vêm do texto oficial de cada norma. A lista completa, com a data da conferência, está no fim do `SKILL.md`. Normas e políticas mudam: reconfira a fonte quando a auditoria for feita muito depois dessa data.

## Como usar

1. Instale a skill a partir do arquivo `SKILL.md` deste repositório, no assistente que você usa.
2. Conecte as contas que serão auditadas. A skill foi escrita para um conector de Google Ads, o conector de Meta Ads e, opcionalmente, um CRM ou caixa de WhatsApp para comparar conversões com contatos reais. Com outras ferramentas, adapte os nomes das consultas.
3. Peça a auditoria indicando o cliente, a plataforma e o período. Exemplo:

   > Faça uma auditoria só de leitura do Google Ads do cliente X, de 06/10 a 04/11, comparando com os 30 dias anteriores.

## Limitações

- Os pesos da nota são a versão 0 e serão calibrados depois de mais auditorias reais.
- A auditoria depende do que os conectores deixam ler. O que não estiver acessível vira FALTANDO, não estimativa.
- A conformidade aponta o que a norma diz; ela não substitui orientação jurídica em caso de dúvida sobre como interpretar uma regra.
