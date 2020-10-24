# Introdução à análise geoespacial com R

## Programa de Pós-Graduação em Ecologia, Evolução e Biodiversidade

**Docente responsável** <br>
Prof. Milton Cezar Ribeiro

**Docente convidado** <br>
Prof. Maurício Humberto Vancine

**Período** <br>19/10/2020 - 30/10/2020

**Créditos** <br>
60 horas (4 créditos)

**Vagas** <br>
10 + 5 especiais

**Resumo** <br>A disciplina oferecerá os principais conceitos teórico-práticos introdutórios de análises geoespaciais aplicado à Ecologia. A parte prática será desenvolvida através de ferramentas na linguagem R. Serão abordados os seguintes temas: (1) controle de versão, Git e GitHub, (2) introdução e funcionamento da linguagem R e do software RStudio, (3) estrutura e manejo de dados na linguagem R, (4) funcionamento do tidyverse, (5) estrutura e fonte de dados geoespaciais, (6) manejo dados geoespaciais (vetor), (7) manejo dados geoespaciais (raster) e, (8) produção de mapas. A carga horária total será de 60 horas, onde nos cinco dias iniciais serão ministrados 6 horas teóricas-práticas, num total de 30 horas. As 30 horas restantes serão direcionadas à realização de exercícios práticos, que serão aplicados remotamente como forma de avaliação para compor a nota final da disciplina. Após a realização da disciplina, espera-se que os alunos adquiram conceitos gerais da estrutura e manipulação de dados geoespaciais, assim como domínio das técnicas e métodos para alcançar autonomia e produzir soluções para suas próprias questões relativas ao geoprocessamento utilizando a linguagem R.

---

### Informações aos participantes

**Datas e horários** <br>
Teórico-prático: 19/10 – 23/10 [09 h - 12 h | 14 h - 17 h] (30 horas)

Exercícios-atividades assistidas remotamente: 26/10 – 30/10 (30 horas)

**Plano de ensino** <br> 
[pdf](https://github.com/mauriciovancine/disciplina-analise-geoespacial-r/blob/master/00_plano_ensino/plano_ensino_analise_geoespacial_r.pdf)

**Contato** <br>
Para mais informações ou dúvidas, envie e-mail para Maurício Vancine (mauricio.vancine@gmail.com)

---

### Instruções aos participantes

**Hardware** <br>
Será necessário que todos usem seus notebooks

**Softwares**<br>
R, RStudio e git <br>

1. Instalar a versão mais recente do [R (4.0.x)](https://www.r-project.org) e [RStudio (1.3.x)](https://www.rstudio.com) <br>
   [Vídeo de instalação do R e do RStudio](https://youtu.be/l1bWvZMNMCM) <br>
   [Curso da linguagem R](https://www.youtube.com/playlist?list=PLucm8g_ezqNq0RMHvzZ8M32xhopFhmsr6)

   

2. Instalar o [git (2.28)](https://git-scm.com/downloads)<br>
   [Vídeo de instalação do git](https://youtu.be/QSfHNEiBd2k) <br>

#### Linux (Ubuntu e Linux Mint)

```
# r
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-keys E298A3A825C0D65DFD57CBB651716619E084DAB9
sudo add-apt-repository "deb https://cloud.r-project.org/bin/linux/ubuntu focal-cran40/"
sudo apt update
sudo apt install -y r-base r-base-core r-recommended r-base-dev

# r spatial
sudo add-apt-repository ppa:ubuntugis/ubuntugis-unstable
sudo apt update
sudo apt install -y libudunits2-dev libgdal-dev libgeos-dev libproj-dev

# rstudio
wget -c https://download1.rstudio.org/desktop/bionic/amd64/rstudio-1.3.1093-amd64.deb
sudo dpkg -i rstudio-1.3.1093-amd64.deb
sudo apt install -fy
rm rstudio-1.3.1093-amd64.deb

# git
sudo add-apt-repository ppa:git-core/ppa 
sudo apt update
sudo apt install -y git

```

**Instalar os pacotes no R** <br>
Com o R e o RStudio instalados, baixe esse [script](https://github.com/mauriciovancine/disciplina-analise-geoespacial-r/blob/master/02_scripts/00_script_install_packages.R) (scripts são roteiros que possuem comandos, como um rascunho). <br>
Abra o script (**00_script_install_r_packages.R**) no software RStudio e rode cada linha de comando para instalar os pacotes, necessário estar conectado à internet. <br>
Para rodar as linhas, basta colocar o cursor na linha de código a ser executada e pressionar: `Ctrl + Enter`.


---

## Slides

- [Aula 00](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/00_pres_intro_geocomp_r.html)
- [Aula 01](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/01_pres_intro_geocomp_r.html)
- [Aula 02]([Aula 01](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/02_pres_intro_geocomp_r.html))
- [Aula 03]([Aula 01](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/03_pres_intro_geocomp_r.html))
- [Aula 04]([Aula 01](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/04_pres_intro_geocomp_r.html))
- [Aula 05]([Aula 01](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/05_pres_intro_geocomp_r.html))
- [Aula 06]([Aula 01](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/06_pres_intro_geocomp_r.html))
- [Aula 07]([Aula 01](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/07_pres_intro_geocomp_r.html))
- [Aula 08]([Aula 01](https://mauriciovancine.github.io/disciplina-analise-geoespacial-r/01_aulas/08_pres_intro_geocomp_r.html))

---

## Scripts

- [Instalar pacotes](https://github.com/mauriciovancine/disciplina-analise-geoespacial-r/blob/master/02_scripts/00_script_install_packages.R)
- [Aula 03](https://github.com/mauriciovancine/disciplina-analise-geoespacial-r/blob/master/02_scripts/03_script_intro_geocomp_r.R)
- [Aula 04](https://github.com/mauriciovancine/disciplina-analise-geoespacial-r/blob/master/02_scripts/04_script_intro_geocomp_r.R)
- [Aula 06](https://github.com/mauriciovancine/disciplina-analise-geoespacial-r/blob/master/02_scripts/06_script_intro_geocomp_r.R)
- [Aula 07](https://github.com/mauriciovancine/disciplina-analise-geoespacial-r/blob/master/02_scripts/07_script_intro_geocomp_r.R)
- [Aula 08](https://github.com/mauriciovancine/disciplina-analise-geoespacial-r/blob/master/02_scripts/08_script_intro_geocomp_r.R)