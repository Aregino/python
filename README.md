## Configuração de Tarefa Agendada para Execução de Script Python

**Introdução**

Este guia detalha como configurar uma tarefa agendada no Windows Task Scheduler para executar um script Python de forma automatizada. Isso é útil para tarefas repetitivas, como geração de relatórios ou atualização de dados.

**Pré-requisitos**

* **Python:** Ter o Python instalado (recomenda-se a versão 3.x).
* **Script Python:** Ter o script Python que você deseja executar pronto.
* **Permissões de Administrador:** Você precisará de permissões de administrador para criar a tarefa agendada.

**Passos**

1. **Abrir o Task Scheduler:**  Abra o aplicativo "Agendador de Tarefas".
  ![image](https://github.com/user-attachments/assets/f284e7d6-e511-480b-83e6-240dabdc2189)


2. **Criar Nova Tarefa:** 🆕 Clique em "Criar Tarefa".

![image](https://github.com/user-attachments/assets/fa1c8da2-8d7b-4a00-8cc3-f197dcf82c07)

4. **Nomear a Tarefa:**  Dê um nome descritivo para a tarefa (ex: "Executar Relatório Diário").

![image](https://github.com/user-attachments/assets/6c4bc6f5-8c2f-4e99-beb4-4b4216ce519e)

5. **Configurar Gatilhos:** ⏰ Na aba "Gatilhos", clique em "Novo" e configure a frequência e o horário de execução.

![image](https://github.com/user-attachments/assets/4defb874-06eb-43cc-98e5-7a24fdece300)

6. **Definir Ação:** ⚙️ Na aba "Ações", clique em "Novo":
   * **Programa/Script:** `C:\ProgramData\Anaconda3\python.exe` (ou o caminho do seu interpretador Python)
   * **Adicionar argumentos:** `meu_script.py` (ou o caminho do seu script)

![image](https://github.com/user-attachments/assets/6c977d2f-5689-44ee-8f87-5fa58402b1fd)

7. **Configurações Adicionais:**
   * **Geral:** Marque a opção "Executar se o usuário estiver logado ou não".

![image](https://github.com/user-attachments/assets/70f59845-2f45-4ad7-90a6-cbe5043b618f)

8. **Conceder Permissões:**  O sistema solicitará a senha da conta que será utilizada para executar a tarefa. _Pode ser que não peça dependendo das configurações do seu user._

![image](https://github.com/user-attachments/assets/1585dadb-fa68-4b34-86d4-c20a3302ff4e)

**Quando criado com sucesso  na lista de jobs basta executar :**

![image](https://github.com/user-attachments/assets/8c010cdf-0a5c-4adf-81bf-b48e83b53a4c)
