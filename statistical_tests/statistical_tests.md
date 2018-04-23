statistical_tests.R
========================================================
author: JEST
date: 25/04/2018
autosize: true

Porque?
=======================================================
![some caption](imagens/chart.png)
http://www.tylervigen.com/spurious-correlations

Tipos de Variaveis 
========================================================


- Quantitativas - representam variaveis que podem ser medidas numa escala quantitativa
  - Discretas - Ex: numero de filhos, idade...
  - Continuas - EX: peso, altura...
- Qualitativas - representam variaveis definidas por varias categorias
  - Nominais - Ex: sexo, cor dos olhos...
  - Ordinais - Ex: escolaridade, mes...
  
Dataset
========================================================


```r
# https://www.kaggle.com/osmi/mental-health-in-tech-survey
dataset <- read.csv2("survey.csv", header = T)
summary(dataset)
```

```
 Timestamp.Age.Gender.Country.state.self_employed.family_history.treatment.work_interfere.no_employees.remote_work.tech_company.benefits.care_options.wellness_program.seek_help.anonymity.leave.mental_health_consequence.phys_health_consequence.coworkers.supervisor.mental_health_interview.phys_health_interview.mental_vs_physical.obs_consequence.comments
 2014-08-27 11:29:31,37,Female,United States,IL,NA,No,Yes,Often,6-25,No,Yes,Yes,Not sure,No,Yes,Yes,Somewhat easy,No,No,Some of them,Yes,No,Maybe,Yes,No,NA                    :   1                                                                                                                                                                             
 2014-08-27 11:29:37,44,M,United States,IN,NA,No,No,Rarely,More than 1000,No,No,Don't know,No,Don't know,Don't know,Don't know,Don't know,Maybe,No,No,No,No,No,Don't know,No,NA:   1                                                                                                                                                                             
 2014-08-27 11:29:44,32,Male,Canada,NA,NA,No,No,Rarely,6-25,No,Yes,No,No,No,No,Don't know,Somewhat difficult,No,No,Yes,Yes,Yes,Yes,No,No,NA                                    :   1                                                                                                                                                                             
 2014-08-27 11:29:46,31,Male,United Kingdom,NA,NA,Yes,Yes,Often,26-100,No,Yes,No,Yes,No,No,No,Somewhat difficult,Yes,Yes,Some of them,No,Maybe,Maybe,No,Yes,NA                 :   1                                                                                                                                                                             
 2014-08-27 11:30:22,31,Male,United States,TX,NA,No,No,Never,100-500,Yes,Yes,Yes,No,Don't know,Don't know,Don't know,Don't know,No,No,Some of them,Yes,Yes,Yes,Don't know,No,NA:   1                                                                                                                                                                             
 2014-08-27 11:31:22,33,Male,United States,TN,NA,Yes,No,Sometimes,6-25,No,Yes,Yes,Not sure,No,Don't know,Don't know,Don't know,No,No,Yes,Yes,No,Maybe,Don't know,No,NA         :   1                                                                                                                                                                             
 (Other)                                                                                                                                                                       :1253                                                                                                                                                                             
```

Tipos de Amostras
========================================================


