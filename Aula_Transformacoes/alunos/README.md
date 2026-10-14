# 1. Mini Sistema Solar

**Disciplina:** Computação Gráfica  
**Atividade:** Mini Sistema Solar  
**Integrantes:** Phillipe Almeida Faria; Miguel Felipe Garcez Viana.

## Descrição

Composição de matrizes para animar o Sol, a órbita do planeta (raio 0,6), sua rotação própria e a Lua (raio 0,2). Os ângulos acumulam velocidade × deltaTime. A Lua reutiliza a matriz da órbita do planeta, sem herdar sua escala ou rotação própria.

## Resposta da questão

Em A @ B @ ponto, B é aplicada primeiro. Na órbita R @ T, a translação afasta o planeta da origem e a rotação gira esse deslocamento ao redor do Sol. A rotação própria fica à direita de T para girar a geometria ao redor do centro local antes de posicioná-la na órbita. Assim, a composição é R_orbita @ T_raio @ R_propria @ S. A escala à direita altera somente o tamanho do planeta, preservando o raio da órbita.

## Execução (Windows)

Abra o terminal nesta pasta `alunos` e execute:

```powershell
py -3 -m venv .venv
.venv\Scripts\python.exe -m pip install -r requirements.txt
.venv\Scripts\python.exe atividade_sistema_solar.py
```

**Controles:** ↑/↓: aumentar/diminuir a velocidade orbital; P: salvar captura; Esc: fechar.

A captura é salva em `capturas/resultado.png`. 

**Fonte:** [Enunciado da disciplina](https://github.com/rodrygofesantos/pygame/blob/main/Aula_Transformacoes/alunos/ATIVIDADE.md).
