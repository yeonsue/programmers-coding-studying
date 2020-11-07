# programmers-coding-studying
def solution(numbers):
    answer=[]
    list_answer=[]
    a=len(numbers)
    
    for k in range(1,a):
        for i in range(a-k):
            ans=numbers[i]+numbers[i+k]
            list_answer.append(ans)
    for i in list_answer:
        if i not in answer:
            answer.append(i)
            answer.sort()
    return answer
