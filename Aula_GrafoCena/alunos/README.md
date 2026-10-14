# 2. Braço Robótico

**Disciplina:** Computação Gráfica  
**Atividade:** Braço Robótico  
**Integrantes:** Phillipe Almeida Faria; Miguel Felipe Garcez Viana.

## Descrição

Grafo de cena com base, pivô do ombro, braço laranja, pivô do cotovelo, antebraço azul e garra cinza. Os deslocamentos são locais; braço e antebraço são deslocados pela metade da altura para prender a extremidade inferior à articulação.

## Resposta da questão

As caixas são centradas na origem local; girá-las diretamente faria cada segmento girar em torno do próprio centro. Os pivôs Object3D definem os centros de rotação nas articulações. Cada caixa é deslocada pela metade de sua altura em relação ao pivô, prendendo a extremidade inferior a ele. A hierarquia faz com que os movimentos da base e do ombro sejam transmitidos aos segmentos seguintes, enquanto o cotovelo movimenta apenas o antebraço e a garra.

## Execução (Windows)

Abra o terminal nesta pasta `alunos` e execute:

```powershell
py -3 -m venv .venv
.venv\Scripts\python.exe -m pip install -r requirements.txt
.venv\Scripts\python.exe atividade_braco.py
```

**Controles:** A/D: girar base; W/S: mover ombro; I/K: mover cotovelo; P: salvar captura; Esc: fechar.

A captura é salva em `capturas/resultado.png`. Dobre o braço com W/S e I/K antes de capturar.

**Fonte:** [Enunciado da disciplina](https://github.com/rodrygofesantos/pygame/blob/main/Aula_GrafoCena/alunos/ATIVIDADE.md).
