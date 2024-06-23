# A Jupyter notebook comparing private german pension plans: self-managed vs. insurance-based

## 🇬🇧🇺🇸 In English

In Germany there are two major models to supplement your retirement fund. Either self managed (which is more heavily
taxed during payout) or mediated through a life-insurance agency (which has higher upfront and running cost). When researching
this topic in detail for my family, I found that there is almost no quantitative cost breakdown / framework that allows you to
run the numbers yourself. This notebook is an attempt. Use at your own risk! Since it's a German thing with lots of German
terminology, let's just speak and "ausnahmsweise" also program in German here this time.

## 🇩🇪 Auf Deutsch

Ziel dieser Übung soll es sein, eigen-gemanagte Altersvorsorge über einen ETF vs. über eine Altersvorsorgeversicherung 
möglichst  genau quantitativ zu vergleichen. Im Internet finden sich hier nur qualitative Aussagen. Dieses Python-Notebook ist
der Versuch, Simulationen beider Strategien zu vergleichen. Nutzung ohne Gewähr!

Insbesondere die steuerliche Kalkulation mit Abgeltungspauschalen, daraus resultierenden Steuerguthaben und Steuerfreibeträgen,
macht die Berechnung recht umständlich, weshalb eine Excel-Tabelle hier ungeeignet und stattdessen ein Python Notebook
entworfen wurde, welches die Anspar- und Rentenphase simuliert und die Statistiken über Data-Frames wegschreibt und dann per
Plotly ausgibt.

## 🇩🇪 Video-Durchlauf

Ich habe ein Youtube-Video veröffentlicht, welches den Sachverhalt inkl. des Python-Notebooks erklärt:



## 🇩🇪 Notebook öffnen

**Das Notebook steht exportiert in [Altersvorsorge.html](https://benkku.com/Altersvorsorge/Altersvorsorge.html)**
[(Quelle)](./Altersvorsorge.html) zur Verfügung. Der Quellcode [Altersvorsorge.ipynb](./Altersvorsorge.ipynb) lässt sich wie
folgt bearbeiten:

Ich verwende Python 3.19.9 sowie die Requirements in `requirements.txt`. Mit 
[`pyenv`](https://github.com/pyenv/pyenv?tab=readme-ov-file) lässt sich diese Python-Version als alternative Python-Version
installieren. Nach dem Clonen dieses Repos im Verzeichnis des Codes:

```bash
curl https://pyenv.run | bash # pyenv installieren
# danach diese Instruktionen folgen:
# https://github.com/pyenv/pyenv#set-up-your-shell-environment-for-pyenv

pyenv install 3.19.9
pyenv local 3.19.9
python -m venv .venv
. .venv/bin/activate
pip install -r requirements.txt
jupyter notebook
# Im Jupyter-Notebook "Altersvorsorge.ipynb" öffnen
```
