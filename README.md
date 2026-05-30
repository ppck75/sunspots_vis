# 🌞 Sunspot (태양 흑점 분석)

태양 흑점 데이터를 수집 및 분석한 프로젝트입니다. 

## 📋 개요

이 프로젝트는 태양 흑점의 활동 패턴을 분석하고 시각화하는 데 중점을 두고 있습니다. 역사적 태양 흑점 데이터를 활용하여 태양 활동의 주기성과 트렌드를 파악합니다.

## ✨ 주요 기능

- 📊 **데이터 분석**: 태양 흑점 데이터의 통계 분석
- 📈 **시각화**: 다양한 차트를 통한 데이터 시각화
- 🔄 **패턴 인식**: 태양 활동의 주기성 감지
- 💾 **데이터 처리**: 효율적인 데이터 전처리 및 정제


## 📁 프로젝트 구조

```
sunspots/
├── README.md                 # 프로젝트 설명 (이 파일)
├── requirements.txt          # Python 의존성
├── sumspots/                 # 메인 패키지
│   ├── __init__.py
│   ├── analyze.py           # 분석 모듈
│   ├── visualize.py         # 시각화 모듈
│   └── data/                # 데이터 디렉토리
└── tests/                   # 테스트 코드
```

## 📚 사용 예제

### 데이터 로드 및 분석

```python
from sumspots import data_loader, analyzer

# 데이터 로드
sunspot_data = data_loader.load_data()

# 기본 통계
stats = analyzer.get_statistics(sunspot_data)
print(f"평균: {stats['mean']}")
print(f"최대값: {stats['max']}")
```

### 시각화

```python
from sumspots import visualizer

# 시계열 그래프
visualizer.plot_timeseries(sunspot_data)

# 주기성 분석 그래프
visualizer.plot_periodicity(sunspot_data)
```

## 🔗 참고 자료

- [NOAA 태양 흑점 데이터](https://www.solarserver.com)
- [태양 활동 주기](https://solarscience.msfc.nasa.gov)
- [Python 과학 계산 라이브러리](https://scipy.org)


---

