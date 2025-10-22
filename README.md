# matplotlib_library_guide
# 📊 Matplotlib 가이드북

Python의 대표적인 시각화 라이브러리 `matplotlib`을 사용하여 데이터를 시각적으로 표현하는 방법을 소개합니다.

---

## 🧩 소개

| 항목 | 설명 |
|------|------|
| 라이브러리 이름 | `matplotlib` |
| 주요 기능 | 선 그래프, 막대 그래프, 산점도, 히스토그램, 이미지, 애니메이션 등 다양한 시각화 지원 |
| 대표 모듈 | `matplotlib.pyplot` |
| 사용 환경 | Jupyter Notebook, Colab, Python Script 등 |

---

## ⚙️ 설치 방법

| 환경 | 명령어 |
|------|--------|
| pip | `pip install matplotlib` |
| conda | `conda install matplotlib` |
| Jupyter / Colab | 보통 기본 포함됨 (필요 시 `!pip install matplotlib`) |

---

## 🏗️ 기본 구조

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4, 5]
y = [10, 20, 25, 30, 40]

plt.plot(x, y)
plt.title("기본 선 그래프")
plt.xlabel("X축")
plt.ylabel("Y축")
plt.grid(True)
plt.show()
```

---

## 🛠️ 주요 함수 기능 정리

| 함수 | 설명 |
|------|------|
| `plot()` | 선 그래프 |
| `bar()` | 막대 그래프 |
| `scatter()` | 산점도 |
| `hist()` | 히스토그램 |
| `pie()` | 파이 차트 |
| `imshow()` | 이미지 표시 |
| `fill()` | 영역 채우기 |
| `subplot()` | 여러 개의 그래프 배치 |

---

## 🎨 스타일 / 옵션 요약

| 항목 | 사용 예시 | 설명 |
|------|-----------|------|
| 제목 | `plt.title("제목")` | 그래프 제목 |
| 축 이름 | `plt.xlabel("X")`, `plt.ylabel("Y")` | 축 이름 지정 |
| 범례 | `plt.legend()` | 범례 표시 |
| 색상 | `color='red'` | 선, 막대 등 색상 |
| 선 종류 | `linestyle='--'` | 선 스타일 (`-`, `--`, `:`, `-.`) |
| 마커 | `marker='o'` | 점 표시 (`o`, `x`, `s`, etc.) |
| 크기 | `figsize=(6,4)` | 그래프 크기 지정 |

---

## 🔍 자주 쓰는 시각화 예제

### ✔️ 선 그래프

```python
plt.plot([1,2,3], [10,20,30], color='blue', linestyle='--', marker='o')
```

### ✔️ 막대 그래프

```python
plt.bar(['A', 'B', 'C'], [10, 20, 15], color='green')
```

### ✔️ 산점도

```python
plt.scatter([1,2,3], [5,15,25], color='red')
```

### ✔️ 히스토그램

```python
import numpy as np
data = np.random.randn(1000)
plt.hist(data, bins=30)
```

---

## 🧠 팁 & 참고

| 팁 | 설명 |
|-----|------|
| `%matplotlib inline` | Jupyter에서 그래프를 셀 아래에 표시 |
| `plt.savefig('파일명.png')` | 그래프를 이미지로 저장 |
| `plt.style.use('ggplot')` | 스타일 적용 (`seaborn`, `bmh`, `dark_background`, ...) |

---

## 📚 참고 자료

- [Matplotlib 공식 문서](https://matplotlib.org/stable/index.html)
- [Python Graph Gallery](https://www.python-graph-gallery.com/)
- [DataCamp 튜토리얼](https://www.datacamp.com/community/tutorials/matplotlib-tutorial-python)

---

🎉 이 가이드는 matplotlib 입문자와 중급 사용자가 빠르게 개념을 익히고 실습할 수 있도록 구성되었습니다.  
필요 시 더 많은 예제를 추가해보세요!
