# VASAP_CONTEMPO

## Visualizador 3D Interativo de Vasos Vasap

Este projeto é um visualizador web 3D para uma coleção de vasos Vasap, desenvolvido usando [A-Frame](https://aframe.io/). Ele permite que usuários inspecionem modelos 3D dos vasos de forma interativa, com animações suaves, iluminação dinâmica, e suporte a visualização em Realidade Aumentada (AR) em dispositivos iOS.

---

## Funcionalidades

- **Visualização 3D Imersiva:** Seis vasos são exibidos em um layout circular, posicionados sobre um plano claro, prontos para inspeção.
- **Interatividade com o Olhar (Gaze):** Ao focar em qualquer vaso, ele se aproxima do usuário, gira lentamente e se inclina, destacando-se para inspeção detalhada.
- **Iluminação Dinâmica:** Cada vaso recebe uma luz direcional que acompanha a posição da câmera, além de iluminação ambiente personalizável.
- **Animações Suaves:** Transições de posição, rotação e iluminação acontecem de forma fluida para criar uma experiência agradável.
- **Barra de Carregamento:** Uma tela de carregamento com barra de progresso garante que todos os modelos sejam carregados antes da interação.
- **Suporte a AR (Realidade Aumentada) no iOS:** Ao focar em um vaso em um dispositivo Apple, surge um botão "Ver em AR" que permite visualizar o modelo no ambiente real via AR Quick Look.
- **Escala e Centralização Automática:** Todos os modelos são automaticamente centralizados e ajustados para proporções ideais.
- **Acessibilidade:** O projeto foi pensado para funcionar tanto em desktop quanto em dispositivos móveis.

---

## Como Usar

1. **Clone o repositório:**
    ```bash
    git clone https://github.com/phillypmack/VASAP_CONTEMPO.git
    cd VASAP_CONTEMPO
    ```

2. **Adicione seus modelos (caso queira substituir):**
    - Os arquivos `.obj` dos vasos devem ser colocados na raiz do projeto e referenciados no `<a-assets>` do HTML.

3. **Abra o arquivo `index.html` em seu navegador:**
    - Recomendado usar Chrome, Firefox, Safari ou Edge.
    - Para visualização AR, use Safari no iOS.

---

## Estrutura do Projeto

- `index.html` – Página principal com estrutura e scripts.
- `logo.png` – Logo exibida na tela de carregamento.
- `VSPX30 - 01.obj` a `VSPX30 - 06.obj` – Modelos 3D dos vasos.
- (Opcional) Arquivos `.usdz` para AR no iOS.

---

## Principais Componentes Personalizados

- **gaze-and-interact:** Garante a interatividade e animações de aproximação, giro, inclinação e iluminação dos vasos enquanto são inspecionados.
- **secondary-light:** Cria uma fonte de luz dinâmica que acompanha a posição da câmera para cada vaso.
- **autoscale:** Centraliza e ajusta o tamanho de cada modelo 3D automaticamente.
- **face-camera:** (não utilizada nos vasos, mas disponível) faz com que um objeto sempre olhe para a câmera.

---

## Requisitos

- Navegador moderno com suporte a WebGL.
- Para AR: dispositivo iOS com Safari.

---

## Créditos

Desenvolvido por [phillypmack](https://github.com/phillypmack).

---

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.