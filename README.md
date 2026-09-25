# PCM Industrial — V4

Versão focada em planos mestres, TAGs e cronograma real de 52 semanas.

## Principais melhorias

- 26 planos mestres identificados na base original.
- 331 vínculos de plano/TAG carregados a partir da aba Gantt_52_Semanas.
- Tela **Planos** agrupada por nome do plano, mostrando a quantidade de TAGs e permitindo expandir a lista.
- Cronograma de **52 semanas com datas reais**.
- Cada TAG usa a última execução encontrada na planilha como referência; a próxima data é calculada por `última execução + periodicidade`.
- Quando não existe execução anterior, o sistema preserva a primeira data planejada encontrada na planilha como início do ciclo.
- Vencidas ficam no backlog, atividades dos próximos 14 dias aparecem como **A vencer**, SS abertas aparecem como **Programado**, e as demais como **Planejado**.
- Ao dar baixa, a data executada vira a nova referência e recalcula automaticamente todo o ciclo futuro.

## Login inicial

- Usuário: `admin`
- Senha: `admin123`

## GitHub Pages

Substitua os arquivos do repositório atual por estes arquivos e faça o commit. O GitHub Pages será atualizado automaticamente.

> Observação: esta versão continua usando armazenamento local do navegador. Para vários usuários compartilharem os mesmos dados em tempo real, é necessário conectar um banco de dados online.
