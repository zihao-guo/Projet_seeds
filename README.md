# Seeds-Random effect logistic regression
:fire:This is a bayes projet of Clement, Diego, Razan, Zihao. [Data is here](https://github.com/zihao-guo/Projet_seeds/tree/main/DATA)



## Problem Description
This example is taken from Table(above) of Crowder (1978), and concerns the proportion of seeds that germinated on each of 21 plates arranged according to a 2 by 2 factorial layout by seed and type of root extract. The data are shown below, where $r_i$ and $n_i$ are the number of germinated and the total number of seeds on the $i$th plate, $i=1,...,N$. These data are also analysed by, for example, Breslow and Clayton (1993).

<div align=center>
<img src="https://github.com/zihao-guo/Projet_seeds/blob/main/Image/data_intro.png">
</div>

## Model Description

The model is essentially a random effects logistic, allowing for over-dispersion. If $p_i$ is the probability of germination on the $i$th plate, we assume:

$$r_i \sim \text{Binomial}(p_i, n_i)$$

$$\text{logit}(p_i) = \alpha_0 + \alpha_1 x_{1i} + \alpha_2 x_{2i} + \alpha_{12} x_{1i}x_{2i} + b_i$$

$$b_i \sim \text{Normal}(0, \tau)$$

where $x_{1i}$ and $x_{2i}$ are the seed type and root extract of the $i$ th plate, and an interaction term $\alpha_{12}x_{1i}x_{2i}$ is included. $\alpha_0$, $\alpha_1$, $\alpha_2$, $\alpha_{12}$, $\tau$ are given independent "noninformative" priors.


## The following is for my partner's use “Temporary”
### !!! Étapes nécessaires à l'utilisation !!! 

1. Cloner
  - [ ] git clone # <**Première fois seulement**>
  ```bash
  $ git clone https://github.com/zihao-guo/Projet_seeds.git
  $ cd Projet_seeds
  ```
  - [ ] Mises à jour # <**À chaque utilisation**>
  ```bash
  $ git pull
  ```
  
2. Soumettre
  - [ ] Soumettre la zone de développement
  ```bash
  $ git add .
  $ git commit -m "AAAA" # AAAA comme note, par exemple la date...
  $ git push -u origin master # <Zone de travail>
  ```

  **Utile**
   ```bash
  $ git branch -a # Voir les branches
  ```
  
  ## Contenu de la note
  1. :racehorse:Supprimer le code
  2. :construction:Modification du code en cours
  3. :tada:Édition terminée
  4. :boom:Changements révolutionnaires


  
  

