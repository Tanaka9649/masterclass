# Masterclass Black Friday — DM Empresarial

Landing page oficial da Masterclass Black Friday, edição de 4 de novembro de 2026 às 20h (horário de Brasília).

## Estrutura
- `site/index.html` — página principal, destinada a `masterclassdm.com.br`.
- `obrigado/index.html` — página de agradecimento, destinada a `obrigado.masterclassdm.com.br`.
- Os botões da página principal levam ao subdomínio de agradecimento.
- Após **2 segundos**, o visitante é enviado ao grupo oficial do WhatsApp, com opção manual caso o navegador não redirecione.

## Hospedagem
Configurar **dois projetos estáticos** na Vercel, usando este mesmo repositório:
1. `masterclass-dm` com Root Directory `site`.
2. `masterclass-dm-obrigado` com Root Directory `obrigado`.

Associação de domínios:
- `masterclassdm.com.br` → `masterclass-dm`
- `obrigado.masterclassdm.com.br` → `masterclass-dm-obrigado`

No Registro.br, criar somente os registros DNS indicados e validados pela Vercel para estes dois domínios. Não substituir nameservers nem excluir registros existentes sem verificar o impacto. Verificar HTTPS e redirecionamento público após propagação.

## Observações
- HTML estático, sem backend nem formulário de inscrições.
- Fotos e logos estão incorporados no HTML para facilitar o deploy.
- O grupo do WhatsApp está configurado apenas na página de obrigado.
- Para campanhas empresariais, verificar plano e termos de hospedagem antes de publicar.
