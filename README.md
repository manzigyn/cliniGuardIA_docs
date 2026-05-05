# CliniGuard IA 🏥🤖
### Guia do Usuário — O que é, para que serve e como usar

---

## O que é o CliniGuard IA?

O **CliniGuard IA** é uma plataforma de avaliação, auditoria e governança de sistemas de Inteligência Artificial voltados à área da saúde. Foi desenvolvida como parte de um trabalho científico para avaliar, de forma sistemática, como diferentes sistemas de IA se comportam quando recebem perguntas médicas reguladas pelos **Protocolos Clínicos e Diretrizes Terapêuticas (PCDTs)** do Ministério da Saúde.

Pense nela como um **examinador automático e imparcial**: a plataforma submete perguntas clínicas estruturadas a diferentes sistemas de IA — como GPT-4, Gemini, Claude e outros — e verifica, em cada resposta, três aspectos essenciais:

- Se a resposta está **alinhada com as normas oficiais** do Ministério da Saúde
- Se o sistema **inventou informações** que não existem (alucinação)
- Se a resposta apresenta alguma **tendência injustificada** que possa prejudicar grupos de pacientes (viés)

O processo é organizado em três etapas integradas: **preparação** (configuração dos experimentos), **execução** (envio automático das perguntas aos sistemas de IA) e **avaliação dos resultados** (análise das respostas por outros sistemas de IA configurados como “juízes”, com classificação e pontuação final). Todo o fluxo é controlado, reproduzível e rastreável, permitindo comparar execuções diferentes com confiança.

---

## Por que isso é importante?

Sistemas de IA já estão sendo usados por profissionais de saúde para tirar dúvidas sobre medicamentos, dosagens e condutas clínicas. No entanto, essas ferramentas não foram criadas especificamente para o contexto da saúde brasileira e não seguem, automaticamente, os protocolos oficiais. Isso gera riscos reais:

- **Inventar informações** — citar medicamentos, dosagens ou tratamentos que não existem ou são incorretos
- **Apresentar tendências** — favorecer ou excluir grupos de pacientes sem qualquer base científica
- **Contradizer protocolos oficiais** — recomendar condutas que vão contra as diretrizes do Ministério da Saúde

O CliniGuard IA foi desenvolvido para **detectar, medir e documentar esses problemas** de forma científica e comparativa. Os resultados ajudam pesquisadores, gestores e profissionais da saúde a entender quais sistemas de IA são mais seguros e confiáveis para uso em contextos clínicos regulados.

A avaliação é ancorada nos próprios PCDTs do Ministério da Saúde, que servem como gabarito normativo. Cada resposta gerada por um sistema de IA é comparada automaticamente com esses documentos e avaliada por outros modelos de IA atuando como “juízes” — tanto especialistas (com acesso ao conteúdo do PCDT) quanto generalistas (avaliando com base no conhecimento médico geral). Ao final, cada modelo recebe uma **pontuação de 0 a 100** e é classificado em uma faixa de risco: **Seguro**, **Uso Supervisionado**, **Restrito** ou **Não Recomendado**.

---

## O que você pode fazer na plataforma?

### 📋 Consultar e Configurar
Antes de realizar qualquer avaliação, é possível organizar os ingredientes do teste:

- **Modelos de IA:** são os sistemas que serão avaliados (ex: GPT-4, Gemini, etc.)
- **Conjuntos de perguntas (Datasets):** agrupamentos temáticos de perguntas clínicas, como "Perguntas sobre Hipertensão" ou "Perguntas sobre Diabetes"
- **Perguntas clínicas:** cada pergunta tem uma resposta correta de referência, baseada nos protocolos do Ministério da Saúde
- **Tipos de risco:** as categorias de problemas que a IA pode apresentar (invenção de informação, tendência clínica, etc.)

### 💬 Conversar com a IA (Chat Interativo)
Existe uma área de **conversa direta** com os modelos de IA cadastrados, parecida com o uso do ChatGPT. Ali você pode testar perguntas clínicas livremente e ver a avaliação em tempo real. Essa área é um **espaço de exploração** — as conversas não são salvas automaticamente, mas você pode guardar perguntas interessantes para uso futuro.

### 🔬 Executar uma Avaliação Oficial (Benchmark)
Esta é a função principal da plataforma. Você escolhe:
- Qual conjunto de perguntas usar
- Quais sistemas de IA avaliar
- Quais juizes de IA usar (especialistas e generalistas)
- Quantas vezes cada pergunta será feita
- Qual metodologia de classificação usar 

A plataforma então submete todas as perguntas para todos os modelos automaticamente e, para cada resposta, verifica:
1. Se a resposta está alinhada com os protocolos do Ministério da Saúde, no caso o dataset
2. Se existe alguma invenção de informação
3. Se existe alguma tendência clínica (viéses e alucinações)
4. Qual foi a nota final do modelo naquela pergunta

### 📊 Dashboard de Indicadores (Painel Analítico)
Após a avaliação, um **painel visual** exibe:
- Classificação dos modelos do melhor ao pior
- Gráficos de desempenho por tipo de problema
- Comparação entre diferentes execuções
- Custo estimado de uso de cada sistema de IA

### 📄 Exportar Relatórios
É possível gerar e baixar relatórios completos das avaliações, incluindo análises por pergunta, comparativos entre modelos e seções formatadas para uso acadêmico.

---

## Quem pode usar a plataforma?

Existem dois perfis de acesso:

### 👤 Usuário Administrador
Tem **acesso completo** à plataforma. Pode criar, editar e excluir qualquer informação, além de executar avaliações.

### 👁️ Usuário de Consulta (Somente Leitura)
Criado para **bancas, demonstrações e auditorias externas**. Pode visualizar todos os dados e executar avaliações, mas **não pode alterar nenhuma informação cadastrada**.

| O que pode fazer | Consulta | Administrador |
|-----------------|----------|---------------|
| Ver painel de resultados | ✅ | ✅ |
| Ver modelos, perguntas e datasets | ✅ | ✅ |
| Usar o chat interativo | ❌ | ✅ |
| Executar uma avaliação | ✅ | ✅ |
| Exportar relatórios | ✅ | ✅ |
| Cadastrar / editar modelos de IA | ❌ | ✅ |
| Cadastrar / editar perguntas | ❌ | ✅ |
| Cadastrar / editar datasets | ❌ | ✅ |
| Enviar documentos de referência | ❌ | ✅ |
| Gerenciar outros usuários | ❌ | ✅ |

#### Credenciais do usuário de consulta


| Campo | Valor |
|-------|-------|
| URL | [https://tcc-ia-cliniguard-ia.afgybm.easypanel.host/](https://tcc-ia-cliniguard-ia.afgybm.easypanel.host/) |
| E-mail | `consulta@cliniguardia.com` |
| Senha | `consulta33` |

> Ao entrar com esse perfil, um indicador **"Somente Leitura"** será exibido no canto superior da tela.

---

## Como uma avaliação funciona, na prática?

Imagine que você quer saber se o **Gemini** e o **GPT-4** respondem bem a perguntas sobre Hipertensão Arterial. O fluxo seria:

1. **Acesse "Execuções de Benchmark"** no menu lateral
2. **Clique em "Nova Execução"** e preencha:
   - Nome da execução (ex: "Teste Hipertensão — Maio 2026")
   - Selecione o conjunto de perguntas sobre Hipertensão
   - Selecione os modelos Gemini e GPT-4
   - Defina quantas tentativas por pergunta (ex: 3 runs)
3. **Clique em Iniciar** — a plataforma começa a avaliar automaticamente
4. Acompanhe o andamento em tempo real na tela
5. Ao terminar, acesse o **Painel** ou **Relatório** para ver os resultados

---

## O que são "Alucinação" e "Viés" no contexto clínico?

Esses são os dois principais problemas que a plataforma detecta:

### 🧠 Alucinação
Ocorre quando a IA **inventa** uma informação que não existe ou está errada. Por exemplo:
- Citar um medicamento inexistente
- Indicar uma dosagem incorreta
- Afirmar que um tratamento é aprovado quando não é

### ⚖️ Viés Clínico
Ocorre quando a IA apresenta uma **tendência injustificada** em suas respostas. Por exemplo:
- Recomendar condutas diferentes para o mesmo problema dependendo do perfil do paciente
- Privilegiar ou excluir grupos sem base nos protocolos oficiais

A plataforma classifica cada resposta e gera uma **pontuação de segurança** para cada modelo avaliado.

---

## Documentos de Referência

A plataforma usa como base de verificação os mesmos documentos que norteiam a saúde pública no Brasil:

| Documento | O que é |
|-----------|---------|
| **PCDT — Protocolos Clínicos e Diretrizes Terapêuticas** | Guias do Ministério da Saúde com as melhores condutas para doenças específicas |
| **Notas Técnicas da ANVISA** | Regulamentações da Agência Nacional de Vigilância Sanitária sobre medicamentos e procedimentos |

Todas as respostas das IAs são verificadas contra esses documentos durante a avaliação.

---

## Materiais de Apoio

| Material | Descrição |
|----------|-----------|
| 🎥 [Vídeo de Demonstração](https://www.youtube.com/watch?v=LINK_DO_VIDEO) | Apresentação completa do uso da plataforma |
| 📊 [Planilha de Perguntas Clínicas e Resultados das Avaliações](pesquisas_resultados_cliniguardIA.xlsx) | Pesquisas realizadas e resultados obtidos com a plataforma |

---

## Perguntas Frequentes

**Preciso entender de tecnologia para usar a plataforma?**
Não. A interface foi desenhada para ser intuitiva. Basta navegar pelos menus, selecionar as opções desejadas e seguir os passos indicados na tela.

**As avaliações demoram muito?**
Depende da quantidade de perguntas e de modelos selecionados. Uma execução pequena (10 perguntas, 2 modelos) pode levar alguns minutos. Execuções maiores podem levar mais tempo, mas você não precisa ficar na tela — a plataforma processa em segundo plano.

**Posso ver execuções feitas por outras pessoas?**
Sim. Todas as execuções ficam visíveis para todos os usuários cadastrados na plataforma.

**O que acontece se eu fechar o navegador durante uma avaliação?**
Nada. A avaliação continua acontecendo normalmente no servidor. Você pode voltar mais tarde e ver os resultados.

**Posso cancelar uma avaliação em andamento?**
Sim. Na lista de execuções, existe um botão de cancelamento para avaliações que ainda estão em andamento.

---

## Contato

**Autor:** Flávio Manzi Alves  
**Instituição:** Universidade Federal de Goiás (UFG)  
**Curso:** Sistemas de Informação  

---

> *"A inteligência artificial na saúde precisa ser auditada antes de chegar ao leito do paciente."*
