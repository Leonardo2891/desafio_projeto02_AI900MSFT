# Aplicação de Detecção de Faces com Azure AI Vision

## Descrição

Esta é uma aplicação que utiliza o **Azure AI Vision Studio** para detectar e analisar faces em imagens. A solução emprega a inteligência artificial da Microsoft para identificar a localização de faces humanas em fotos, juntamente com atributos como pose, máscara facial e marcos faciais.

## Objetivo

O projeto tem como objetivo demonstrar o uso prático da API de Visão Computacional da Azure para fins de análise facial automatizada. Exemplos de casos de uso incluem:

- Detecção de faces em múltiplas imagens
- Análise de atributos faciais (expressão, pose, acessórios)
- Processamento em lote de arquivos de imagem
- Geração de relatórios em formato JSON com os resultados

## Tecnologia Utilizada

- **Azure AI Vision Studio**: Serviço de visão computacional em nuvem
- **Detect Faces API**: API específica para detecção de faces
- **Formato de Saída**: JSON com análise detalhada de atributos

## Estrutura do Projeto

```
desafio_projeto02_AI900MSFT/
├── inputs/              # Pasta contendo as imagens de entrada
│   ├── 20250316.jpg
│   ├── 20250324.jpg
│   └── 20250410.jpg
├── output/              # Pasta contendo os resultados da análise
│   ├── resultado_1.png
│   ├── resultado_2.png
│   └── resultado_3.png
├── README.md            # Este arquivo
└── LICENSE
```

## Funcionalidades Principais

### 1. Detecção de Faces
- Identifica a localização de faces em imagens
- Retorna coordenadas de bounding boxes para cada face detectada

### 2. Análise de Atributos
A API detecta e retorna informações sobre:
- **Pose**: Rotação e inclinação da cabeça
- **Face Mask**: Detecção de máscara facial
- **Facial Landmarks**: Pontos de referência faciais (olhos, nariz, boca, etc.)
- **Expressão Facial**: Análise de emoções e expressões
- **Acessórios**: Óculos, chapéu e outros acessórios

### 3. Saída em JSON
Todos os resultados são fornecidos em formato JSON estruturado, facilitando a integração com outras aplicações e sistemas.

## Como Usar

1. **Preparar as Imagens**
   - Coloque as imagens a serem analisadas na pasta `inputs/`
   - Formatos suportados: JPG, PNG, BMP, GIF, TIFF

2. **Acessar o Azure AI Vision Studio**
   - Acesse [Azure AI Vision Studio](https://portal.vision.cognitive.azure.com/)
   - Faça login com sua conta Azure
   - Navegue até a seção "Detect faces in an image"

3. **Fazer Upload e Processar**
   - Selecione a imagem ou faça upload de um arquivo
   - Clique no botão de processamento
   - Aguarde o resultado ser retornado

4. **Analisar os Resultados**
   - Visualize a imagem com as faces detectadas e destacadas
   - Consulte os dados JSON com os atributos detalhados
   - Salve os resultados na pasta `output/`

## Exemplos de Resultados

A aplicação gera visualizações das faces detectadas com:
- Retângulos delimitadores (bounding boxes) ao redor de cada face
- Informações detalhadas em formato JSON sobre os atributos de cada face
- Análise completa dos pontos de referência faciais

## Requisitos

- Conta do Microsoft Azure ativa
- Acesso ao Azure AI Vision Studio
- Imagens em formatos padrão (JPG, PNG, etc.)

## Recurso Utilizado

- **Resource**: desafio-dio-ai900-02
- **Plataforma**: Cloud (Azure)

## Notas Importantes

- As informações coletadas de fotos neste demo não predizem nem classificam atributos faciais
- Os dados não são usados para criar modelos faciais
- Nenhuma identificação pessoal é realizada

## Referências Úteis

- [Azure AI Vision Documentation](https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/)
- [Detect Faces API Reference](https://learn.microsoft.com/en-us/azure/ai-services/computer-vision/concept-detecting-faces)
- [Azure AI Vision Studio](https://portal.vision.cognitive.azure.com/)

## Licença

Este projeto está sob a licença especificada no arquivo `LICENSE`.

---

**Desenvolvido como parte do desafio do bootcamp DIO - Microsoft AI-900**
