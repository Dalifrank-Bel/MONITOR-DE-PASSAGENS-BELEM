name: Monitor de Passagens

on:
  schedule:
    # Roda a cada 6 horas automaticamente
    - cron: '0 */6 * * *'
  workflow_dispatch: # Permite que você clique em um botão para testar a qualquer momento

jobs:
  run-monitor:
    runs-on: ubuntu-latest
    steps:
      - name: Baixar código do repositório
        uses: actions/checkout@v4

      - name: Configurar Python
        uses: actions/setup-python@v5
        with:
          python-version: '3.10'

      - name: Executar o monitor
        run: python monitor.py
