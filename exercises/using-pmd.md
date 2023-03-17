# Using PMD

Pick a Java project from Github (see the [instructions](../sujet.md) for suggestions). Run PMD on its source code using any ruleset. Describe below an issue found by PMD that you think should be solved (true positive) and include below the changes you would add to the source code. Describe below an issue found by PMD that is not worth solving (false positive). Explain why you would not solve this issue.

## Answer

la commande ```./run.sh pmd -d ../../../Documents/Cours/VV/commons-lang-master/ -f html -R java-unusedcode > rapportPMD.html``` m'a permis de générer un rapport dans un fichier rapportPMD.html permettant de retrouver tout le code non utilisé dans la librairie commons-lang-master (voir screenshot ci-dessus)