# Verificação da entrega

- Sintaxe Python verificada nos 56 arquivos do pacote.
- Arquivos auxiliares comparados com o repositório original: preservados byte a byte. Os READMEs de origem estão em `INSTRUCOES_ORIGINAIS.md`.
- Demonstrações executadas e os três programas iniciados diretamente por seus arquivos `.py`, com término normal.
- Execução gráfica real com Pygame 2.6.1, PyOpenGL 3.1.10 e contexto OpenGL NVIDIA: sem erros OpenGL detectados.
- Sistema solar: raios do planeta (0,6) e da Lua (0,2), avanço dos ângulos, aumento de velocidade e limite mínimo zero verificados.
- Braço: relações pai/filho, posições das articulações e resposta dos seis controles verificados; captura com braço dobrado.
- Cubos: relação pai/filho, distância 1,3, escala 0,4, repeatUV [2,2], movimento orbital, rotação local e alteração da velocidade verificados.
- As três capturas foram geradas pela execução dos programas e inspecionadas visualmente.

Os controles foram exercitados por chamadas automatizadas a `update`, simulando o retorno de `isKeyPressed`. A interação física com o teclado não foi verificada manualmente. As capturas usam `saveScreenshot`, a mesma função chamada pelas teclas P/S.

**Pendências da entrega:** preencher o nome do segundo integrante, publicar no GitHub e entregar os links no Blackboard. Nenhum envio externo foi realizado.
