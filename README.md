

# recommender-systems-project-2

This  project  was going to be a neutral network model based  recommender system  build on hotel data. The goal was to achieve the best HR@10 in the final  evaluation. In order to do so data had to be preprocessed, user and item  features  prepared, neural network model created and the  recommender  had to be tuned and validated  using  multiple  methodes.  

Sadly attempts in creating neutral network model failed but data preprocessing and input features were improved.
  

### Data preprocessing  

Data preparation  contains  of adding, filtering out, aggregating  and bucking  data to get the most important  features and reduce the offer  space  size.  

  

### Preparing  user and item  features  

For user  features the one-hot encoding was used. Every  feature was taken  into  account but only  n values with the largest  number of occurrences  were  encoded  where n was based on the number of values  of  feature.  

  

For item  features one-hot encoding was used for every  feature. Duplicates of  item_id  were  dropped.  

  

 

### Preparing  recommender  

In fit  function  of the recommender  class  negative  interactions  were  generated, user_id and item_id was randomly  created  from defined  range in order for this  user and item to exist, then  it was checked  if the pair  is  in existing interactions, if not then  it was added to the list of negative  ones.   

  

 

### Tuning  

Tuning was not executed since recommender was not working. 

  

  



### Requirements to run the project: 

- install Anaconda, 

- install all used python libraries: 

        - numpy, 

        - pandas, 

        - hyperopt, 

        - matplotlib, 

        - seaborn,
  
	      - livelossplot,
  
	      - torch,

        -scikit learn
