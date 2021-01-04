# ArgVote Dataset

Dataset from an experiment with our argument-based voting advice application (VAA) ArgVote.
For more information, please have a look at the following publication:
TBA

## Files

### data_project.csv

Data from the questionnaire with personal information removed.
The column codes are explained in `codebook.csv` (original German texts) and `codebook_translation.csv` (English translation).

### profiles.edn

Voter profiles collected within ArgVote.
* `:left-metric`: Matching algorithm used for the result displayed to the user (matches column v_84)
* `:attitudes`: Statements the user (dis)agrees to or is neutral.
* `:agreements`: Agreement with each party (for both matching algorithms; only the results of one algorithm was displayed to the user)
* `:answers`: Answers to questionnaire questions asked directly within ArgVote:
    * `:confused`: Ich bin vom Ergebnis irritiert. (I am confused about the result.)
    * `:happy-pos1`: Ich bin damit zufrieden, welche Partei an Position 1 angezeigt wird. (I am happy with which party is displayed at position 1.)
    * `:understand-pos1`: Ich finde nachvollziehbar, welche Partei an Position 1 angezeigt wird. (I can understand which party is displayed at position 1.)
    * `:understand-percentage-pos1`: Ich finde die angezeigte prozentuale Übereinstimmung mit der Partei an Position 1 nachvollziehbar. (I can understand the displayed percentage of agreement with the party at position 1.)
    * `:understand-order`: Ich finde die Reihenfolge der Parteien insgesamt sinnvoll. (I consider the overall order of the parties as a whole to be reasonable.)
    * `:understand-percentage`: Ich finde die prozentuale Übereinstimmung der Parteien insgesamt sinnvoll. (I consider the percentage of agreement of the parties as a whole to be reasonable.)
    * `:justification`: Wenn Sie mögen, können Sie Ihre Antworten der gerade gestellten Fragen begründen. Warum sind Sie mit dem Ergebnis zufrieden/unzufrieden? (If you like, you can give reasons for your answers to the questions you have just been asked. Why are you satisfied/dissatisfied with the result? – personal data, not included in public dataset)

### arguments.json

Argument corpus in the Argument Interchange Format (AIF), including statement ids.
Note that we do not (yet) publicly provide the complete statement texts for legal reasons.
