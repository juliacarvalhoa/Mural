# Mural IELBV

Mural de recados da **Igreja Evangélica Livre do Boa Vista** (Curitiba, PR).
Reúne em uma página simples, feita para o celular, os avisos, eventos e encontros dos ministérios da igreja.

## Como funciona

```
Google Forms  →  Google Sheets  →  esta página (GitHub Pages)
 envio pela       revisão e         mural
 liderança        aprovação
```

- Líderes e secretaria enviam os recados por um formulário.
- Cada recado é revisado e aprovado antes de aparecer.
- A página lê só os recados aprovados e só os campos públicos (título, ministério, texto, data, horário, local e link).
- Cada recado tem uma data de validade e sai do mural sozinho quando ela passa.
- Os recados ficam organizados em "Esta semana", "Avisos" e "Mais pra frente", com busca e filtro por ministério.
- Cada recado pode ser encaminhado direto no WhatsApp.
- Tudo usa ferramentas gratuitas, sem servidor e sem custo de manutenção.

## Privacidade

O mural é para recados que podem ser vistos por qualquer pessoa com o link. Pedidos de oração, dados pessoais e assuntos internos da liderança não são publicados aqui. O nome de quem envia um recado não aparece na página.

## Quer fazer um mural igual na sua comunidade?

1. Crie um Google Forms com: título, ministério, recado, data, horário, local, link, "mostrar até" e "é importante?".
2. Vincule a uma planilha e crie uma coluna **Publicar** (`S`/`N`).
3. Crie uma aba **Mural** com uma fórmula `QUERY` que selecione só as linhas aprovadas e só os campos públicos, com estes rótulos de coluna: `titulo`, `area`, `recado`, `data`, `horario`, `local`, `link`, `ate`, `urgente`.
4. Publique **só a aba Mural** como CSV (Arquivo → Compartilhar → Publicar na Web).
5. Faça uma cópia deste `index.html`, preencha `CSV_URL` e `CONTATO` perto do fim do arquivo e ajuste textos, cores e logo para a sua comunidade.
6. Publique no GitHub Pages (Settings → Pages → Branch `main`).

Atenção: tudo o que estiver na aba publicada fica visível para quem tiver o link.
