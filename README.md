def solution(string, ending):
    if(len(string) < len(ending)): return False
    for (x, y) in zip(string[::-1], ending[::-1]):
        if(x != y):
            return False
    return True
