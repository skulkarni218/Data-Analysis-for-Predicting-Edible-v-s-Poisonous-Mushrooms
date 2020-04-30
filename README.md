# Data-Analysis-for-Predicting-Edible-v-s-Poisonous-Mushrooms

This dataset was originally contributed to the UCI Machine Learning repository. Nearly 30 years ago, mushroom hunting (otherwise known as "shrooming") is enjoying new peaks in popularity. The objective of this analysis is to understand the factors which impact whether a mushroom is edible or poisonous and additionally, to predict the same using machine learning algorithms.

This dataset includes descriptions of hypothetical samples corresponding to 23 species of gilled mushrooms in the Agaricus and Lepiota Family Mushroom drawn from The Audubon Society Field Guide to North American Mushrooms (1981). Each species is identified as definitely edible, definitely poisonous, or of unknown edibility and not recommended. This latter class was combined with the poisonous one. The Guide clearly states that there is no simple rule for determining the edibility of a mushroom; no rule like "leaflets three, let it be'' for Poisonous Oak and Ivy.

After analyzing the data, it was concluded that the top factors and features affect the class of a mushroom i.e. edible or poisonous. 
|	Variable	|	Coefficients	|	Feature	|
|	-------------	|	-------------	|	-------------	|
|	spore_print_color_name_Green	|	4.598658381	|	spore_print_color_name	|
|	odor_name_Creosote	|	3.796506288	|	odor_name	|
|	odor_name_Foul	|	3.59952777	|	odor_name	|
|	gill_size_name_Narrow	|	3.249449791	|	gill_size_name	|
|	odor_name_Pungent	|	2.822277752	|	odor_name	|
|	gill_color_name_Buff	|	2.14979729	|	gill_color_name	|
|	stalk_surface_above_ring_name_Silky	|	1.853463494	|	stalk_surface_above_ring_name	|
|	spore_print_color_name_Chocolate	|	1.757414841	|	spore_print_color_name	|
|	population_name_Clustered	|	1.733027345	|	population_name	|
|	spore_print_color_name_Purple	|	-1.528948761	|	spore_print_color_name	|
|	habitat_name_Waste	|	-1.535387122	|	habitat_name	|
|	odor_name_Anise	|	-1.617734329	|	odor_name	|
|	ring_type_name_Flaring	|	-1.761455002	|	ring_type_name	|
|	stalk_root_name_Rooted	|	-1.801610113	|	stalk_root_name	|
|	gill_spacing_name_Crowded	|	-2.222849008	|	gill_spacing_name	|
|	stalk_root_name_Club	|	-2.223849021	|	stalk_root_name	|
|	odor_name_None	|	-3.611217293	|	odor_name	|

From the above graph we can see that the top influencing features are:
* spore_print_color_name
* odor_name
* gill_size_name
* gill_color_name
* stalk_surface_above_ring_name
* population_name
* habitat_name
* ring_type_name
* stalk_root_name
* gill_spacing_name

The results from the Logistic Regression Model were phenomenal. By using Logistic Regression, I have achieved a 100% prediction accuracy when it comes to predicting edible v/s poisonous mushrooms. From the confusion matrix (can be seen in the .ipynb file), we have only 2 instances (i.e. 0.08%) when the prediction has failed. The prediciton has failed when the mushroom was edible but the model predicted it to be poisonous. According to me, that is perfectly all right as it is not putting anybody's life at risk. It would have been a problem if it were the other way round as it would put the consumers' life at risk. Since, 100% accuracy has been obtained, I did not feel the need to use any other advanced ML algorithms.
