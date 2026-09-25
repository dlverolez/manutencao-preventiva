# PCM Preventiva — Sistema de Planos de Manutenção

Aplicação web estática para cadastro e controle de planos de manutenção preventiva, criada a partir da planilha **Plano preventiva Manutenção industrial**.

## O que já vem pronto

- 332 combinações de plano + TAG importadas da planilha original.
- Dashboard com planos ativos, próximos 30 dias, vencidas e aderência.
- Cadastro, edição, inativação e exclusão de planos.
- Campos: ID, plano, TAG, descrição, setor, periodicidade, responsável, data-base e criticidade.
- Agenda automática baseada na periodicidade em dias.
- Registro de execução / SS com data planejada, número da SS, abertura, baixa, responsável e observações.
- Histórico de execuções.
- Filtros por plano, TAG, setor e status.
- Backup e restauração em JSON.
- Funciona no GitHub Pages sem servidor.

## Publicar no GitHub Pages

1. Crie um repositório no GitHub, por exemplo `pcm-preventiva`.
2. Envie `index.html`, `styles.css`, `app.js`, `seed.js` e este `README.md` para a raiz do repositório.
3. No GitHub, acesse **Settings → Pages**.
4. Em **Build and deployment**, selecione **Deploy from a branch**.
5. Escolha a branch `main` e a pasta `/ (root)`.
6. Salve. O GitHub mostrará o endereço público da aplicação.

## Persistência dos dados

Esta versão usa `localStorage`: os dados ficam gravados no navegador/dispositivo de quem está usando. Use a tela **Backup** para exportar periodicamente um JSON.

Para vários usuários compartilharem a mesma base em tempo real, a evolução recomendada é integrar Supabase, Firebase ou outra API/banco de dados.

## Estrutura

- `index.html` — interface do sistema
- `styles.css` — layout e responsividade
- `app.js` — regras, cadastros, agenda, histórico e backup
- `seed.js` — base inicial importada da planilha

