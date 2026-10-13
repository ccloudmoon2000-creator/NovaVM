# NovaVM — protótipo de emulador web

Interface estática pronta para publicar no GitHub Pages.

## Publicar
1. Cria um repositório no GitHub.
2. Envia `index.html` para a raiz do repositório.
3. Abre **Settings → Pages**.
4. Em **Build and deployment**, escolhe **Deploy from a branch**.
5. Seleciona a branch `main` e a pasta `/ (root)`, depois guarda.

## Estado atual
Este projeto é um protótipo funcional de interface: permite escolher um ficheiro ISO/IMG, ajustar opções de hardware e ver uma consola de demonstração. **Não executa nem arranca o sistema operativo** e os valores de hardware não são recursos reais reservados.

## Para evoluir para emulação real
- Integrar um motor WebAssembly compatível com o sistema pretendido.
- Para x86, investigar o projeto v86 e as suas imagens/firmwares suportados.
- A emulação de Android moderno (frequentemente ARM e dependente de virtualização/aceleração específica) não é equivalente a arrancar uma ISO de PC num navegador.
- GitHub Pages serve ficheiros estáticos; não fornece CPU/RAM/GPU de servidor nem backend. A emulação terá de correr no navegador do visitante, com limites de desempenho e memória.
- Não enviar imagens de sistemas operativos protegidas por direitos de autor para o repositório. O upload atual lê apenas o nome/tamanho localmente; não envia o ficheiro para lado nenhum.

## Ficheiros
- `index.html`: aplicação completa, sem etapa de build.
