# Emagrecentro Guaíba — HTML independente

O arquivo `index.html` contém a página, imagens, fonte, estilos e JavaScript. Ele funciona sem Next.js, React, npm ou build. Você pode abri-lo diretamente no navegador.

## Publicar pelo GitHub na Vercel

1. Crie um repositório no GitHub.
2. Envie o CONTEÚDO desta pasta para a raiz do repositório: `index.html`, `vercel.json`, `og.jpg` e `OFL-Manrope.txt`.
3. Na Vercel, importe esse repositório.
4. Use Framework Preset: **Other**, sem comandos de build ou instalação. O `vercel.json` incluído já define esses valores e diretório de saída `.`.
5. Publique. Nenhuma dependência precisa ser instalada.

Não é necessário enviar o projeto Next.js anterior, `node_modules`, `.next` ou `out`.

Se preferir enviar a pasta antiga inteira ao repositório, o `vercel.json` da RAIZ DO PROJETO aponta para `publicacao`. Nesse caso mantenha essa subpasta. Não confunda os dois arquivos vercel.json: o deste pacote publica `.`, enquanto o da raiz antiga publica `publicacao`.

## Editar

Textos e seções estão no HTML. Cores e estilos estão no `<style id="site-styles">`. As quatro fases e interações estão no `<script id="site-interactions">`. Imagens e fonte estão incorporadas como data URLs; podem ser substituídas por arquivos relativos se desejar separar os assets. A privacidade abre em uma janela dentro da página.

O index da raiz do projeto é uma cópia desta versão. Para publicar futuras alterações pelo repositório completo, edite `publicacao/index.html` (ou mantenha as cópias sincronizadas). Não é necessário gerar o build antigo.

## Depois de definir o domínio

O HTML permite indexação. Inclua canonical, og:url e og:image com URLs absolutas do domínio real. Use o arquivo `og.jpg` incluído para a imagem social; data URLs não são recomendadas para previews de compartilhamento. Nenhum domínio foi inventado. Horários, procedimentos, fotos da unidade e depoimentos continuam sujeitos à confirmação da clínica.

Configuração de referência: https://vercel.com/docs/project-configuration/vercel-json
