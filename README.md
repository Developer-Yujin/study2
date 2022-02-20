# study2

체육복

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
    
    조이스틱
    
    ```python
    def solution(name):
    num = 0

    num = num+ ord(name[0])-65
    name = name.replace(name[0],'')
    

    if(name[1]=='A'):
        name = reversed(name)
    
        for i in name:
            num += 1
            num = num+ord(i)-65

    else:
   
        for i in name:
            num +=1
            num = num+ord(i)-65
            
            
            
    return num
    ```
    
    큰 수 만들기
    ```python
    def solution(number, k):
    
    k = int(k)
    for j in range(k):

        min = 10
        for i in number:
           i = int(i)
           if i<min:
           
               min = i
        min = str(min)
        number = list(number)
        number.remove(min)
        number = ''.join(number)
        #number = number.replace(min,'')

    
    return number
    ```
    
    구명보트
    
    ```python
    def solution(people, limit):
    
    num =0
    left = 0
    for i in range(len(people)):
        num = num+1
        left = limit-people[i]
        for j in range(len(people)-1):
            if people[j+1]<=left:
                i = i+1
 ```           
    
   
    
    
    
