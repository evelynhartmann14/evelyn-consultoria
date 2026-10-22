# Evelyn Hartmann — Revenda Autorizada Claro

Catálogo de planos Claro para enviar aos clientes pelo WhatsApp.
No ar em: https://evelynhartmann14.github.io/evelyn-consultoria/

## Links diretos para disparo
- Página inicial (análise gratuita + escolha): https://evelynhartmann14.github.io/evelyn-consultoria/
- Portabilidade: https://evelynhartmann14.github.io/evelyn-consultoria/#portabilidade
- Transferência de CPF para CNPJ: https://evelynhartmann14.github.io/evelyn-consultoria/#transferencia
- Linha nova (CNPJ): https://evelynhartmann14.github.io/evelyn-consultoria/#linha-nova
- Internet Wi-Fi: https://evelynhartmann14.github.io/evelyn-consultoria/#internet

## Como alterar
- Todo o site está no `index.html`. Foto da consultora: `retrato.jpg`. Imagem da prévia do link no WhatsApp: `capa.jpg`.
- **WhatsApp:** no final do `index.html`, altere `var WHATSAPP = "..."` (55 + DDD + número, só números).
- **Preços:** procure o plano no bloco `CATÁLOGO 1: PORTABILIDADE`, `CATÁLOGO 2` (CNPJ) ou `CATÁLOGO 3: INTERNET WI-FI`. Mude o valor no plano e também no `data-plano` do botão (é a mensagem enviada no WhatsApp).
- **Cores:** bloco "CORES" no início do arquivo (vermelho Claro).
- **Selo Claro:** `claro-revenda.png` (branco, fundo transparente), recortado da arte oficial de Revenda Autorizada.
- **Logos dos benefícios:** pasta `logos/`, recortados do Book Claro empresas (out/2026).

## Sites de outros consultores
Cada consultor tem uma pasta com o mesmo catálogo (ex.: `everton/` → https://evelynhartmann14.github.io/evelyn-consultoria/everton/).
Essas páginas são **geradas** a partir do `index.html` da Evelyn — não edite `everton/index.html` direto.

- Depois de mudar preços ou textos no `index.html`, rode `python3 gerar_consultores.py` para atualizar todos os consultores.
- Para adicionar um consultor: inclua os dados na lista `CONSULTORES` do `gerar_consultores.py`, coloque a foto em `<pasta>/foto.jpg` e rode o script.
