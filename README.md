# 동등성 관계 검사

이 모듈은 집합의 주어진 관계가 등가 관계인지 확인합니다. 등가 관계는 재귀적, 대칭적, 전이적이어야 합니다.

## 함수

- `check_reflexive(R, A)`: 관계가 반사인지 확인합니다.
- `check_symmetric(R)`: 관계가 대칭인지 확인합니다.
- `check_transitive(R)`: 관계가 전이인지 확인합니다.
- `check_equivalence(R, A)`: 반사성, 대칭성, 전이성을 검증하여 집합에서 관계식이 등가 관계인지 확인합니다.

## 사용법

1. 리포지토리를 로컬 컴퓨터에 복제합니다.
2. 스크립트를 실행하여 예시 및 관계에 대한 결과를 확인합니다.

### 예시

```python
if __name__ == "__main__":
    A = {1, 2, 3, 4}
    R = {(1, 1), (1, 3), (2, 2), (3, 3), (3, 1), (3, 4), (4, 4), (4, 3)}

    print("Reflexive:", check_reflexive(R, A))
    print("Symmetric:", check_symmetric(R))
    print("Transitive:", check_transitive(R))
    print("Equivalence:", check_equivalence(R, A))
