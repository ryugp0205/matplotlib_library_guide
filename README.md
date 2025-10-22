# matplotlib_library_guide
##import numpy as np
import matplotlib.pyplot as plt

# t 값 (파라미터)
t = np.linspace(0, 2 * np.pi, 1000)

# 하트 모양을 나타내는 파라메트릭 방정식
x = 16 * np.sin(t)**3
y = 13 * np.cos(t) - 5 * np.cos(2*t) - 2 * np.cos(3*t) - np.cos(4*t)

# 그래프 그리기
plt.figure(figsize=(6,6))
plt.plot(x, y, color='red')
plt.fill(x, y, color='red', alpha=0.5)  # 내부 채우기 (선택 사항)

# 보기 좋게 꾸미기
plt.title('♥ 하트 모양 ♥', fontsize=16)
plt.axis('equal')      # 축 비율 동일하게
plt.axis('off')        # 축 숨기기
plt.show()
