# 3. Cubo com Satélite Texturizado

**Disciplina:** Computação Gráfica  
**Atividade:** Cubo com Satélite Texturizado  
**Integrantes:** Phillipe Almeida Faria; Miguel Felipe Garcez Viana.

## Descrição

Cubo principal com mosaico.png e satélite filho com grade_uv.png repetida 2×2. O satélite é posicionado a 1,3 unidades e depois recebe escala 0,4. Herda o movimento do cubo principal e gira em seu eixo X a 2 rad/s.

## Resposta da questão

As coordenadas UV associam pontos da superfície do objeto a posições da imagem: U indica a direção horizontal e V, a vertical. Elas determinam qual região da textura aparece em cada face. repeatUV = [2,2] multiplica as coordenadas por 2 em ambas as direções; com o modo de repetição da textura, a imagem aparece duas vezes na horizontal e duas na vertical, formando quatro repetições em cada face.

## Execução (Windows)

Abra o terminal nesta pasta `alunos` e execute:

```powershell
py -3 -m venv .venv
.venv\Scripts\python.exe -m pip install -r requirements.txt
.venv\Scripts\python.exe atividade_cubo.py
```

**Controles:** ↑/↓: aumentar/diminuir a velocidade do cubo; S: salvar captura; Esc: fechar.

A captura é salva em `capturas/resultado.png`. 

**Fonte:** [Enunciado da disciplina](https://github.com/rodrygofesantos/pygame/blob/main/Aula_Texturas/alunos/ATIVIDADE.md).
