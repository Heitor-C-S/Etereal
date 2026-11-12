*Leia em outros idiomas: [English](README.md), [Português](README.pt.md).*

# Etereal

> Transformando movimentos em música através de visão computacional.

**Etereal** é um projeto experimental que utiliza visão computacional para rastrear gestos e movimentos corporais, convertendo-os em parâmetros musicais e sonoros em tempo real. Inspirado no conceito do Theremin, o projeto permite que a música seja tocada literalmente "no ar", sem a necessidade de contato físico.

## 🗺️ Roadmap de Desenvolvimento e Prova de Conceito

O projeto está estruturado em fases para garantir uma síntese de áudio confiável antes de escalar a complexidade da interface:

### Fase 1: MVP - Sintetizador Gestual Linear (Foco Atual)
O "Hello World" desta PoC foca em gerar acordes básicos (ex: tríade de Dó Maior na 3ª oitava: Dó3, Mi3, Sol3) com rastreamento independente das mãos:
* **Mão Principal (Raiz/Grau):** Seleciona o grau da escala (ex: segunda, terça, quarta) com base em uma escala raiz usando zonas espaciais lineares.
* **Mão Secundária (Modificador):** Atua como um modificador da qualidade do acorde, alterando a tríade base para um acorde menor, maior com sétima, menor com sétima, etc., através de gestos específicos.
* **Motor de Áudio:** Síntese de áudio confiável em tempo real (polifonia de 3 vozes para as tríades) sem estouro de buffer.

### Fase 2: Interface Radial Dinâmica
Uma evolução da UI espacial para permitir transições mais limpas e maior expressividade:
* **Interface Radial (Mão Direita):** A tela é dividida em um círculo com 7 fatias (A a G) e uma "deadzone" central.
  * **Seleção de Raiz:** O ângulo da mão em relação ao centro (coordenadas polares) seleciona a nota raiz.
  * **Deadzone:** Retornar a mão ao centro funciona como um ponto de repouso, silenciando o som para permitir transições limpas entre acordes não adjacentes.
  * **Modificadores (Gestos):** Gestos com os dedos da mesma mão (ex: pinças entre o polegar e outros dedos) alteram a qualidade do acorde em tempo real.
* **Expressão Contínua (Mão Esquerda):** Atua no eixo vertical (Y) para controle dinâmico de volume, semelhante a um Theremin clássico.

## 🛠️ Stack Tecnológico

* **Linguagem:** Python (com possível fallback para TypeScript)
* **Visão Computacional:** MediaPipe / OpenCV
* **Geração de Áudio:** Síntese algorítmica em tempo real via código (ex: `pyo`, `numpy` + `sounddevice`)

## ⚙️ Instalação e Uso

*(Instruções de como clonar, instalar dependências e rodar o projeto serão adicionadas conforme o desenvolvimento avançar).*

## 📄 Licença

Este projeto está licenciado sob a [PolyForm Noncommercial License 1.0.0](https://polyformproject.org/licenses/noncommercial/1.0.0/). O uso, modificação e distribuição são permitidos exclusivamente para fins não comerciais.
