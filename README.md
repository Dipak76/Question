# Question 1

st = "student"
str2 = "agroustu"
len_st = len(st)
len_str2 = len(str2)
ans = 0

for i in range(len_st + 1):
    str1 = st[:i]
    if str1 in str2 and len(str1) > ans:
        ans = len(str1)

print(ans)



#question 2
list1 = [1, 2, 3, 4]  # Use a list in Python
target = 4

for i in range(len(list1)):
    for j in range(len(list1)):
        if list1[i] + list1[j] == target:
            print(True)
            exit()  # Immediately exit once a pair is found
