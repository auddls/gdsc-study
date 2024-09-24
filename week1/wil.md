
(퀴즈1/다음 중 학습방법에 대한 설명으로 가장 적절하지 않은 것은): 3
(퀴즈2/퍼셉트론의 한계 (주관식)): 한개의 선으로 나눌 때 데이터를 0과 1로 제대로 나눌 수 없기 때문이다
(코딩3/퍼셉트론 구현 : ans1과 ans2를 숫자로 변경하시오
import numpy as np

def Perceptron(x, w, b):
    y = np.sum(w * x) + b
    if y <= 0:
        ans1 = "빈칸 1" # 숫자(int)로 변경하시오
        return ans1
    else:
        ans2 = "빈칸 2" # 숫자(int)로 변경하시오
        return ans2 

# NAND 게이트
def NAND(x1, x2):
    return Perceptron(np.array([x1, x2]), np.array([-0.5, -0.5]), 0.7)
 
# OR 게이트
def OR(x1, x2):
    return Perceptron(np.array([x1, x2]), np.array([0.5, 0.5]), -0.2)
 
# AND 게이트
def AND(x1, x2):
    return Perceptron(np.array([x1, x2]), np.array([0.5, 0.5]), -0.7)

# 테스트
print("NAND 게이트:")
print(NAND(0, 0), NAND(0, 1), NAND(1, 0), NAND(1, 1))

print("OR 게이트:")
print(OR(0, 0), OR(0, 1), OR(1, 0), OR(1, 1))

print("AND 게이트:")
print(AND(0, 0), AND(0, 1), AND(1, 0), AND(1, 1))
): ans1 = 0 , ans2 = 1
(설문): 3
