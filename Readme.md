# ReadMe.md
이전 코드에서 선형 회귀 모델을 k-최근접 이웃 회귀(이 경우 k=3)로 바꾸려면 간단하게 다음 두 라인만 바꾸면 됩니다:

```python
from sklearn.linear_model import LinearRegression

model = LinearRegression()
```

아래와 같이 바꿉니다:

```python
from sklearn.neighbors import KNeighborsRegressor

model = KNeighborsRegressor(n_neighbors=3)
```