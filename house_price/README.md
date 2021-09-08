# House Prices - Advanced Regression Techniques


## EDA / Data Preprocessing

### Feature classification
- Split 80 features into 6 categories
- Fill in missing-values
<span style="color:yellow">- Consider about Outliers.</span>

#### Numeric datas
- numeric(raw) : real valued data (ex. area, length...)
- discrete : discrete values (ex. number of rooms)

#### Categorical datas
- mapping : data that has some order (ex. Quality)
- one-hot : data that has no order (ex. SaleType)

#### Others
- extra : data that need discussion
- delete : need to delete

### Data Preprocessing
- Handling our datas according to our classification
- numeric(raw) : Normalization
- discrete : 
- mapping : consider that our order is meaningful?
- one-hot : Use one-hot encoding. 


<span style="color:red">Condider about small samples / Outliers</span>

## Modeling

### Model
We will use Scikit-learn (maybe)
- Random Forest
- XGBoost
- LightGBM
- Others?

### Ensemble



## Evaluating
- Evaluation standard : RMSLE
<span stye='color:red'> - Consider our evaluating model.</span>

