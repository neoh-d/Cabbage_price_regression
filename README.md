# Cabbage Price Regression
배추 가격 예측 프로젝트(2팀) _데이터마이닝_서울과기대

##  Google Colab 실행
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/neoh-d/Cabbage_price_regression/blob/main/notebook/%EB%B0%B0%EC%B6%94%EA%B0%80%EA%B2%A9%EC%98%88%EC%B8%A1.ipynb)


##  프로젝트 개요
기상/기후 데이터를 활용하여 1996–2024년 배추 도매가격을 예측하는 프로젝트입니다.

- 주요 알고리즘: Ridge, Lasso, Random Forest
- 변수 선택: VIF + Stepwise Selection
- 성능 검증: LOOCV, TimeSeriesSplit
- 성능 지표: R2,MSE,MAPE등
- 해석 기법: SHAP 분석

## 📁 폴더 구조
```
cabbage-price-prediction/
├── notebooks/                  #  코드 + 시각화 + 분석 흐름
│   └── 배추가격예측.ipynb
│
├── src/                        #  파이참에서도 실행 가능한 전체 스크립트
│   └── main.py
│
├── data/                       #  프로젝트 입력 데이터
│   ├── final_data2.xlsx
│   ├── weight_final.csv
│   └── ...
│
│
├── README.md                   # 분석 목적/방법/실행법/결과 요약
└── requirements.txt            # 실행을 위한 라이브러리 목록
```


## 모델 성능 요약
| 모델      | R²      | MAPE (%) |
| -------   | ----    | -------- |
| Ridge(CV) | 0.634   |  21.0    |
| RF (CV) | 0.816     |  15.1    |
| RF (TS) | 0.907     |  11.1    |

🧑‍💻 팀원

김대헌/박지홍/이찬우/정지은


