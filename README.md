# 🚀 Case de Product Discovery: Da Hipótese à Evidência — Validando um Produto Digital com IA e Métodos Ágeis no Agronegócio

## 1. Contexto do Desafio
* **Título:** Da Hipótese à Evidência: Validando um Produto Digital com IA e Métodos Ágeis.
* **Contexto:** Uma startup de tecnologia no setor de agronegócio enfrenta o desafio comum de desenvolver soluções sem validação prévia. O objetivo foi atuar como integrante do time de produto para reduzir incertezas utilizando IA, métodos ágeis e experimentação enxuta (*Lean Startup*), focando em descobrir se a ideia merece ser desenvolvida antes de investir em código complexo.

---

## 2. Problema Identificado, Público e Oportunidade
* **Problema:** Agrônomos e operadores de campo enfrentam grande demora na análise de pragas devido à dependência de pareceres de terceiros e fluxos em sistemas legados. A falta de agilidade no diagnóstico atrasa a aplicação de defensivos e impacta a produtividade da lavoura.
* **Público-Alvo:** Agrônomos, técnicos agrícolas e operadores de campo no setor de agronegócio.
* **Oportunidade:** Utilizar Inteligência Artificial e automação leve (chatbot via Telegram) integrada aos dados da fazenda para fornecer diagnósticos rápidos e confiáveis diretamente no campo.

---

## 3. Hipóteses de Problema, Solução e Valor
* **Hipótese de Problema:** Se os profissionais do campo dependem de sistemas lentos e análises externas, o tempo de resposta é alto e o risco de perda na lavoura aumenta.
* **Hipótese de Solução:** Um assistente via Telegram acionado por IA capaz de cruzar imagens de pragas com dados contextuais (clima, região, cultura).
* **Hipótese de Valor:** O usuário economizará tempo precioso e terá suporte técnico imediato, com índice de acurácia superior a 75%.

---

## 4. Solução Inicialmente Proposta e Definição do MVP
* **MVP Desenvolvido:** Um assistente automatizado (*Concierge MVP*) construído no **Make**, integrando o **Telegram** a modelos de **Inteligência Artificial (Gemini)**.
* **Como funciona:** O usuário envia uma foto da praga junto com uma legenda contendo a região, dados climáticos e a cultura. O Make processa o arquivo, faz o upload para a IA e devolve uma resposta estruturada em segundos.

---

## 5. Como a IA e a Automação Foram Utilizadas no Discovery
A IA foi utilizada estritamente como ferramenta de apoio ao *Product Discovery* e automação operacional. O fluxo técnico implementado no Make compreende as etapas de gatilho, download de arquivo, upload e geração de resposta.

* **Link do Cenário Publicado no Make:** [Make Scenario - Pest Diagnosis Bot](https://us2.make.com/public/shared-scenario/kdUxEL4bp4X/pest-diagnosis-bot)

### ⚙️ Prompt Aplicado na IA (Configuração do Make):
> **Função:** Você é um agrônomo especialista em identificação de pragas, doenças agrícolas e receituário agronômico.
> 
> **Entrada:** Você receberá uma imagem de uma folha/planta com suspeita de praga/doença e uma legenda `[{{1.message.caption}}]` com informações adicionais do usuário (como localização/região, cultura agrícola e observações de campo).
> 
> **Instruções de Análise:**
> 1. **Identificação:** Analise a imagem e a legenda para identificar a praga, doença ou deficiência nutricional mais provável.
> 2. **Nível de Confiança e Criticidade:** Indique a porcentagem de confiança do diagnóstico (mínimo esperado para tomada de decisão: 75%). Classifique a criticidade em: Baixa, Média ou Alta (com base no impacto potencial na lavoura).
> 3. **Condições Climáticas:** Considere a região informada na legenda para avaliar se as condições atuais (ex: umidade, temperatura) favorecem a proliferação da praga.
> 4. **Recomendação de Defensivo e Dosagem:** Sugira a classe de defensivo adequada (ex: fungicida, inseticida) e a dosagem padrão recomendada em manuais técnicos.
> 
> **Formato de Saída Obrigatório (máximo de 260 palavras):**
> 
> 🔎 **DIAGNÓSTICO PRELIMINAR**
> - **Praga/Doença identificada:** [Nome da praga]
> - **Grau de Confiança:** [X]%
> - **Nível de Criticidade:** 🚨 [Baixa / Média / Alta]
> 
> 🌤️ **ANÁLISE CLIMÁTICA & RISCO**
> - [Breve resumo sobre como o clima da região afeta a evolução da praga]
> 
> 💊 **RECOMENDAÇÃO TÉCNICA**
> - **Classe/Princípio Ativo:** [Nome do produto ou classe]
> - **Dosagem Recomendada:** [Dosagem por hectare ou litros/ha]
> - **Instruções de Aplicação:** [Cuidados na aplicação, ex: evitar horários de pico de calor]
> 
> ⚠️ *Nota: Esta é uma análise automatizada via IA para apoio à decisão. Valide os dados antes de efetuar a aplicação no campo.*

---

## 6. Experimento, Evidências e Validação com Usuários Reais
* **Testes Realizados:** O MVP foi testado com **5 colegas de trabalho agrônomos** em campo.
* **Evidências Coletadas:** 
  * Nos testes iniciais (apenas com imagens isoladas), a taxa de erro era alta. 
  * Ao exigir obrigatoriamente mais imagens e a legenda contextual (clima, região, cultura e dados de ERP), a acurácia do modelo saltou para **acima de 85%**.
* **Feedback dos Usuários:** Os agrônomos acharam a ferramenta prática, sugerindo que no futuro o sistema se conecte ao **PCP (Planejamento e Controle de Produção) e Ordens de Serviço** do ERP da empresa, gerando um alerta de recomendação de troca, mas **sempre mantendo a aprovação final nas mãos do gestor** (*human-in-the-loop*).

---

## 7. Decisão Final
* **Decisão:** **AJUSTAR**.
* **Justificativa:** Validamos que a IA traz um ganho enorme de tempo e precisão (acurácia > 85%), desde que alimentada com o contexto correto do operador. A próxima fase do produto não será uma automação cega, mas sim a integração oficial com o ERP/PCP da empresa, focando em notificações de recomendação com validação gerencial prévia.

---

## 8. Vídeo Pitch do Projeto
Assista à apresentação executiva do case de validação:
* **Link do Vídeo:** [YouTube - Pitch do Projeto](https://youtu.be/Mx5F0GTJhB4)
