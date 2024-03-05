# lab02-ai900
## Introdução

Resolução do laboratório 03 (<i>Optical Character Recognition</i> (OCR)) da série mslearn-ai-fundamentals, da Microsoft. Para mais informações, acesse o [repositório oficial](https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/tree/main/Instructions/Labs).

A proposta é trazer imagens aleatórias que contenham texto e verificar a precisão da extração feita pelo Vision Studio, outra ferramenta do Microsoft Azure.

## Criação do recurso

No portal do [Azure](https://portal.azure.com/), será preciso criar um novo recurso do Azure AI services. Ele será necessário quando iniciarmos a utilização do Vision.

1. Clique em "Create a resource" e, busque por Azure AI services.
2. Preencha as configurações como necessário e confirme sua criação.

![Visão geral Azure AI Service criado](/assets/images/azure-ai-services-overview.png)

## Conexão do recurso ao Vision Studio

1. Em outra guia do navegador, acesse o [Vision Studio](https://portal.vision.cognitive.azure.com/).
2. Depois de entrar com a sua conta, vá ao ícone de engrenagem e selecione o recurso criado anteriormente como padrão.

![Recurso geral Vision Studio](/assets/images/vision-default-resource.png)

## Utilização da análise de imagens

1. Voltando à página inicial do Vision, acesse o menu "Optical character recognition" e selecione "Extract text from images".
2. Aceite o termo sob a opção "Try it out".

Você poderá utilizar imagens pré estabelecidas pela Microsoft, mas também pode subir imagens do seu dispositivo e até mesmo tirar uma fotografia dentro do próprio site.

Ao selecionar uma imagem de exemplo, você será retornado (direita) com todo o texto que foi detectado na imagem e um texto em JSON.

![Resultado da amostra](/assets/images/image-text-extract.png)

Quando passar o cursor (<i>hover</i>) sobre qualquer palavra, ela será destacada - tanto na origem, quanto no retorno.

![Resultado da amostra](/assets/images/image-text-extract-hover.png)

## Inputs e Outputs

As seguintes imagens foram imputadas para teste e análise do retorno:

### Capa de Livro

![Capa de Livro](/output/capa-livro.png)

### Página de Livro

![Página de Livro](/output/pagina.png)

### Rótulo de lata

![Rótulo de Lata](/output/rotulo-cerveja.png)

## Insights

- É de enorme importância ter uma luz de qualidade nas imagens que serão utilizadas;

- O retorno segue fielmente à imagem. Cada item em sua respectiva linha, independente de uma palavra ser formada ou não;

- Para juntar essas informações e montar um texto completo, na maioria dos casos, precisará haver intervenção humana.
