import sys

n = int(sys.stdin.readline())

for _ in range(n):
    p_list = list(sys.stdin.readline().rstrip())
    stk = []
    isVPS = True
    for i in p_list:
        if i == "(":
            stk.append(i)
        elif i == ")":
            if stk:
                stk.pop()
            elif not stk:
                isVPS = False
                break
    if not stk and isVPS:
        print("YES")
    elif stk or not isVPS:
        print("NO")
