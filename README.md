# 📊 Agendamento de Query SQL e Envio por E-mail (Redshift + Gmail)

Este script Python automatiza o processo de **executar uma query em um banco Redshift**, salvar o resultado em um arquivo Excel e **enviar por e-mail com anexo**, em horários agendados diariamente.

---

## 🔍 O que ele faz

- Conecta-se ao Redshift com `psycopg2`.
- Roda uma query SQL definida no script.
- Exporta os dados para um arquivo `.xlsx`.
- Envia por e-mail com o anexo via `yagmail` (SMTP do Gmail).
- Executa o processo automaticamente nos horários: `11:30`, `14:00` e `16:30`.

---

## ⚙️ Pré-requisitos

- Python 3.8+
- Bibliotecas:
  - `pandas`
  - `psycopg2`
  - `yagmail`
  - `schedule`

Informações do banco de dados (host, porta, usuário, senha).

Credenciais de e-mail (senha de app do Gmail).

Lista de destinatários (EMAIL_TO).

Corpo do e-mail e horários de envio.

Execute o script:

python RodarQueryEEnviar.py
O script ficará rodando em loop e executará os envios automaticamente nos horários definidos.

📈 Exemplo de aplicação
Enviar relatórios diários de uso, performance, churn etc.

Automatizar dashboards de produto.

Base para sistemas de alerta via SQL.

📄 Licença
Código open-source para automação de BI e DataOps. Contribuições são bem-vindas!
