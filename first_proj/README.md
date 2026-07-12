🏆 Scouting the Academy's Next Star (NumPy)
Project Overview

This mini-project uses NumPy to evaluate and rank 12 academy players for a regional tournament. Each player is assessed using four physical performance metrics. The coaching staff provides fixed metric weights and a roster constraint requiring that the final six-player squad include at least one goalkeeper. The objective is to apply these rules consistently, produce a ranked list of players, and justify the final selection.

Methodology
The raw performance metrics are cleaned and combined into a weighted talent score using NumPy broadcasting.
Players, positions, and scores are stored in a structured NumPy array for convenient sorting and filtering.
The array is sorted in descending order of talent score to obtain the preliminary ranking.
The six highest-scoring players form the initial squad.
Because the tournament rules require at least one goalkeeper, the initial selection is checked for positional balance. If no goalkeeper is present, the lowest-scoring outfield player in the provisional squad is replaced by the highest-scoring goalkeeper.
Results

The preliminary top six players by weighted score are:

Adam
Yara
Nada
Omar
Hana
Mostafa

Sprint Speed and Agility receive the largest weights, reflecting the fast pace of the competition. After applying the goalkeeper requirement, Mostafa is replaced by Ziad, who is the highest-rated goalkeeper.

Final Squad: Adam, Yara, Nada, Omar, Hana, and Ziad.

Conclusion

The final roster satisfies all selection criteria established by the coaching staff. The replacement of Mostafa with Ziad slightly reduces the aggregate talent score but ensures the squad includes a specialist goalkeeper, preserving tactical completeness and compliance with the tournament rules.