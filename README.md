# 서울 사고누적지점 분석

[서울 사고 유형 지도 열기](https://agliotomato.github.io/BigData_Project/)

2023~2025년 서울 327개 사고누적지점의 사망·중상사고 4,564건을 사고 유형별로 살펴볼 수 있습니다.

## 팀원 실행 방법

저장소 전체를 내려받고 프로젝트 루트에서 다음 명령을 실행한다.

```shell
python -m pip install jupyterlab ipykernel
python -m jupyterlab
```

Python 3 커널에서 아래 순서로 각 노트북의 **Run All**을 실행한다.

1. [사고 데이터 전처리](notebooks/사고_데이터_전처리.ipynb)는 `data/raw/tmacs/2025/`의 사고상세·지점목록 CSV를 검증하고 `data/processed/사고_분석용.csv`를 생성하거나 확인한다.
2. [데이터 시각화](notebooks/데이터%20시각화.ipynb)는 분석용 CSV와 지점목록으로 `outputs/서울_사고유형_지도.html`을 생성한다. 지도 배경과 Leaflet을 불러올 때 인터넷 연결이 필요하다.
