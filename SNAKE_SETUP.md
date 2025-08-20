# 🐍 Configuração do GitHub Snake

## O que foi configurado

1. **Workflow do GitHub Actions** (`.github/workflows/snake.yml`)
   - Executa automaticamente a cada 12 horas
   - Pode ser executado manualmente através do GitHub
   - Gera o snake com suas contribuições do GitHub

2. **Arquivo SVG funcional** (`assets/github-contribution-grid-snake.svg`)
   - Snake funcional com contribuições simuladas
   - Será atualizado automaticamente pelo workflow quando você tiver contribuições reais

## Como funciona

O snake é gerado usando a ferramenta [snk](https://github.com/Platane/snk) que:
- Acessa suas contribuições públicas do GitHub
- Cria uma animação SVG baseada no seu histórico de commits
- Atualiza automaticamente o arquivo no repositório

## Próximos passos

1. **Faça commit e push das alterações:**
   ```bash
   git add .
   git commit -m "Adiciona configuração do GitHub Snake"
   git push
   ```

2. **Execute o workflow manualmente:**
   - Vá para a aba "Actions" no seu repositório
   - Clique em "Generate Snake"
   - Clique em "Run workflow"

3. **Aguarde a execução:**
   - O workflow vai gerar o snake com suas contribuições
   - O arquivo SVG será atualizado automaticamente

## Personalização

Você pode personalizar o snake editando o arquivo `.github/workflows/snake.yml`:

- **Tema:** Adicione `theme: [nome-do-tema]` (ex: `radical`, `tokyo-night`, `dracula`)
- **Frequência:** Altere o `cron` para executar em horários diferentes
- **Formato:** O workflow gera SVG por padrão, mas pode gerar GIF também

## Temas disponíveis

- `radical` (padrão)
- `tokyo-night`
- `dracula`
- `gruvbox`
- `github-dark`
- `github-light`
- E muitos outros...

## Solução de problemas

Se o snake não aparecer:
1. Verifique se o workflow foi executado com sucesso
2. Confirme que o arquivo SVG foi atualizado
3. Aguarde alguns minutos para o GitHub processar as mudanças
4. Verifique se você tem contribuições públicas no GitHub
