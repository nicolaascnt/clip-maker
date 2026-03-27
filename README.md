# ClipMaker | Corte Viral

Projeto front-end simples desenvolvido para gerar um corte viral a partir de um video.

## O que este projeto faz

1. Envia um video para o Cloudinary.
2. Aguarda a transcricao gerada no Cloudinary.
3. Usa Gemini para identificar o melhor trecho (30 a 60 segundos).
4. Monta e reproduz a URL final do corte.

## Requisitos

1. Conta no Cloudinary.
2. Upload Preset configurado no Cloudinary.
3. Chave da API Gemini.
4. Navegador

## Como testar localmente

1. Abra o arquivo index.html no navegador.
2. Troque temporariamente (your user) pelo seu cloud name.
3. Troque temporariamente (your preset) pelo seu upload preset.
4. No campo Gemini API Key da tela, cole sua chave.
5. Clique em Enviar video e gerar corte viral.

Importante: nao publique valores reais de Cloudinary no GitHub.

No arquivo index.html, localize as funcoes abaixo e deixe com placeholders:

    const pickCloudName = () => {
        return "(your user)";
    };

    const pickPreset = () => {
        return "(your preset)";
    };

Assim, qualquer pessoa que clonar o projeto sabera o que trocar localmente, sem usar suas credenciais.


## Observacao

Este projeto e focado em estudo. Em producao, use backend para proteger credenciais e regras de negocio.
