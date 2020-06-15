# Ingegneria del Software --Modulo-SW-Testing-
Repository di consegna della relazione finale del modulo di Software Testing per il corso di Ingegneria del Sofwtare 2

# Posizione dei Test
A causa della natura _package protected_ di alcuni oggetti o metodi e l'utilizzo di classi di instanziazione dell'ambeinte di test si è reso necessario posizione i test in specifiche cartelle così come da link di seguito

##BookKeeper
https://github.com/Esposito-Matteo/bookkeeper/tree/master/bookkeeper-server/src/test

##Tajo
https://github.com/Esposito-Matteo/tajo/tree/master/tajo-cluster-tests/src/test

#Profili
Per eseguire jacoco, è sufficiente copiare il comando nella sezione script di dei rispettivi file .travis.yml
Per eseguire ba-dua il comando è: mvn test -PbaduaProfile [+ eventuali flag presi dal file .travis.ylm]
( se dovesse mancare la libreria, il pom cerca lo jar partendo dalla root del progetto nella cartella ba-dua-lib/ba-dua-agent-rt-0.4.1-SNAPSHOT-all.jar
Per eseguire pit il comando è: mvn org.pitest:pitest-maven:mutationCoverage surefire:test -PpitProfile [+ eventuali flag presi dal file .travis.ylm]

