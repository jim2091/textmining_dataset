# 텍스트 마이닝 실습을 위한 데이터셋

텍스트 마이닝 실습에 이용되는 데이터셋을 핸들링하는 함수 집합입니다.

하위 폴더들은 각 데이터셋의 이름이며 현재 정리된 데이터셋의 이름은 아래와 같습니다. 데이터 별 특징은 각 데이터 폴더 안의 README 에 기록하였습니다.

| Dataset name | Description |
| --- | --- |
| movie_comments | 네이버영화에서 수집한 영화별 사용자 작성 커멘트와 평점 |

폴더는 아래처럼 구성되어 있습니다. 데이터셋 폴더 아래의 data 는 각 데이터셋별 raw data 이며, models 는 raw data 를 이용하여 학습을 한 모델들이 저장된 폴더 입니다. 예를 들어 영화 평점 분류 문제를 위하여 텍스트들로부터 Bag-of-Words Models 를 만들고, 이를 이용하여 학습데이터 (X, Y) 를 미리 만들어 둘 수 있습니다. 이러한 모델들을  models 안에 모아뒀습니다.

각 데이터셋 안에는 init 과 데이터셋 핸들링에 관련된 Python 파일들이 포함되어 있습니다. 사용법은 각 데이터 폴더 안의 README 를 참고하세요.

```
--| movie_comments
    __init__.py
    loader.py
    fetch.py
    README.md
    --| data
    --| models
```
