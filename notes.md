# Data Science Notes

## Pandas

|  What  |  How  |
|----|----|
| Import pandas| `import pandas as pd` |
| Read a csv to a dataframe | `df = pd.read_csv("https:\\....")` |
| Head | `df.head()` |
| Delete a column | `x_data=df.drop('price',axis=1)` |

## Seaborn

## Sklearn

### Split data into training and testing data 
```
from sklearn.model_selection import train_test_split
x_train, x_test, y_train, y_test = train_test_split(x_data, y_data, test_size=0.3, random_state=1)
```
### Linear Regression
```
from sklearn.linear_model import LinearRegression
lre=LinearRegression()
lre.fit(x_train, y_train)
print(lre.score(x_test, y_test))
```

## IPython

|  What  |  How  |
|----|----|
| Hide output| `%%capture` |
