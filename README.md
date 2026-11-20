# FaultScope Studio

**FaultScope Studio** é uma plataforma web para análise de oscilografias e registros de perturbação no padrão IEEE COMTRADE (1991, 1999 e 2013). Executada diretamente no navegador do cliente, sem necessidade de instalação ou envio de dados para servidores externos.

Acesse online: [https://www.vsmconsult.com.br](https://www.vsmconsult.com.br)

---

## Principais Funcionalidades

### 1. Visualização e Análise de Oscilografias COMTRADE
- Suporte a formatos **ASCII**, **BINARY**, **BINARY32** e **FLOAT32** (.CFG, .DAT e arquivos anexados como .INF / .HDR).
- Arraste e solte múltiplos arquivos simultaneamente.
- Gráficos analógicos e digitais de alta taxa de amostragem utilizando HTML5 Canvas acelerado.
- Cursores sincronizados (Cursor A, Cursor B, Delta de tempo e cálculo instantâneo de frequência fundamental).
- Zoom dinâmico horizontal e vertical, arraste (pan) e encaixe automático de escalas.
- Reordenação e movimentação ágil de curvas entre eixos analógicos via arrastar e soltar (drag-and-drop).
- Modo comparativo lado a lado (*side-by-side*) entre diferentes oscilografias.

### 2. Diagrama Fasorial e Componentes Simétricas
- Visualização polar dinâmica dos fasores de tensão e corrente calculados nos pontos dos cursores.
- Detecção automática de fases e agrupamento de grandezas trifásicas (Fases A, B e C).
- Decomposição em **Componentes Simétricas** (Sequência Zero, Positiva e Negativa).
- Indicadores de desbalanço negativo ($I_2/I_1$ e $V_2/V_1$) e fator homopolar ($I_0/I_1$ e $V_0/V_1$).
- Modo de visualização normalizado (**$|-|$**) para facilitar a inspeção angular relativa.
- Seleção e ocultação individual de fasores calculados diretamente na tabela.

### 3. Localização de Faltas por Onda Viajante (TWFL)
- Módulo dedicado para análise de frentes de onda de alta frequência.
- Suporte a cálculo manual de onda viajante e integração ponto a ponto (*double-ended*).
- Calibração de comprimento de linha e velocidade de propagação.

### 4. Análise de Frequência e Trajetória de Impedância
- Espectro harmônico via transformada rápida de Fourier (FFT) com exibição de THD.
- Diagrama R-X de impedância aparente para coordenação e análise de funções de distância (21).
- Detecção automática de instantes de início do defeito e extinção do arco elétrico.

---

## Arquitetura e Privacidade

- **100% Client-Side:** Todo o processamento de sinais, decodificação binária de COMTRADE e renderização gráfica ocorrem localmente no navegador.
- **Privacidade Total:** Os dados de oscilografia nunca deixam a estação de trabalho do engenheiro.
- **Zero Dependências de Servidor:** Funciona mesmo em ambientes operacionais isolados (air-gapped) ou offline.

---

## Estrutura do Repositório

- `index.html`: Aplicação SPA completa contendo os estilos, estrutura de interface e lógica de processamento em JavaScript modular.
- `CNAME`: Configuração de domínio personalizado para publicação via GitHub Pages.

---

## Licença

Este projeto é disponibilizado sob os termos da licença [MIT](LICENSE).
