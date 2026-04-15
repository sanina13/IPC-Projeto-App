# Princípios de Usabilidade 
## Ecrãs: Dashboard / Adicionar Medicação / Detalhes / Histórico / Popup Confirmação

---

## 1. Observabilidade (Robustez)

**Definição:** O utilizador deve conseguir observar e compreender o estado atual do sistema com base na informação fornecida pela interface.

**Aplicação no protótipo:**

- **Dashboard:** Cada medicamento apresenta um indicador de estado visível — ✔️ verde para tomas já realizadas e ○ (círculo vazio) para tomas pendentes. O utilizador compreende de imediato o estado da sua medicação sem navegar para outro ecrã.
- **Detalhe da Medicação:** O estado da toma é apresentado de forma destacada com "✔️ Tomado" (verde) ou "❌ Não tomado" (vermelho), tornando o estado do sistema inequivocamente visível.
- **Histórico:** Organiza as tomas por data com os mesmos indicadores ✔️ e ❌, permitindo ao utilizador avaliar o histórico de adesão ao tratamento de forma imediata.
- **Detalhe da Medicação:** O botão "Marcar como tomado" aparece acinzentado quando o medicamento já foi registado como tomado, indicando visivelmente que a ação já não está disponível.

---

## 2. Recuperabilidade (Robustez)

**Definição:** O sistema deve permitir ao utilizador efetuar correções em situações de erro, oferecendo mecanismos de prevenção e recuperação.

**Aplicação no protótipo:**

- **Popup de Confirmação:** Antes de registar a toma de um medicamento, a aplicação apresenta um popup "Confirmar toma da medicação?" com as opções "Cancelar" e "Confirmar". Este passo adicional previne registos acidentais — especialmente crítico num contexto de saúde, onde um erro pode ter consequências para o utilizador.
- **Adicionar Medicação:** O ecrã inclui um botão "Cancelar" claramente visível, permitindo ao utilizador abandonar a adição de medicação sem guardar dados incorretos ou incompletos.
- **Detalhe da Medicação:** O botão "Voltar" permite regressar ao Dashboard sem efetuar alterações, oferecendo uma saída segura para o utilizador que acedeu ao ecrã por engano.

---

## 3. Capacidade de Síntese (Aprendizagem)

**Definição:** O sistema deve apoiar o utilizador na avaliação dos efeitos de ações executadas anteriormente, sintetizando o historial de interações.

**Aplicação no protótipo:**

- **Histórico:** Apresenta um registo completo das medicações tomadas e não tomadas ao longo do tempo, organizado por datas. O utilizador pode consultar facilmente o que fez nos dias anteriores sem necessitar de memorizar.
- **Dashboard:** A data atual ("Hoje, 18 Mar") é apresentada de forma proeminente, contextualizando o utilizador sobre o dia em curso e distinguindo-o do histórico passado.
- **Detalhe da Medicação:** Mostra o estado atual da toma do medicamento, sintetizando a informação mais relevante — se já foi tomado ou não — de forma direta e sem ambiguidade.

---

## 4. Conformidade de Funcionalidades (Robustez)

**Definição:** O sistema deve fornecer um conjunto de funcionalidades suficientemente completo para que o utilizador possa realizar as tarefas pretendidas, da forma que pretende.

**Aplicação no protótipo:**

- **Adicionar Medicação:** O formulário permite definir nome, dosagem, hora e frequência (Diário, Semanal, Personalizado) — todos os campos necessários para uma gestão completa da medicação. Os placeholders com exemplos concretos (ex: "Dosagem (ex: 500mg)") guiam o utilizador no preenchimento correto.
- **Dashboard:** O botão "+ Adicionar" está sempre acessível no ecrã principal, permitindo ao utilizador expandir a sua lista de medicamentos sem necessitar de navegar para outra secção.
- O conjunto de ecrãs disponíveis (Dashboard, Adicionar, Detalhe, Histórico) cobre todas as tarefas identificadas nos cenários de utilização — visualizar, registar, adicionar e consultar medicação — garantindo que nenhuma tarefa essencial fica sem suporte.
