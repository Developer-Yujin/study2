# study2

H2 프로그래머스 greedy 문제

```python
def solution(n, lost, reserve):
    borrow = 0
    
    
    for i in lost:
        for j in reserve:
            if(i==j):
                lost.remove(i)
                reserve.remove(j)
                
    already = int(n)-len(lost)
    
    for i in lost:
        for j in reserve:
            if(i+1==j or i==j):
                borrow += 1
                break

        
    
    return borrow+already;
    ```
