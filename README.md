# hello-world
just another repository
'''
 * @Author: Mr.T 
 * @Date: 2019-09-05 11:19:36 
 * @Last Modified by: Mr.T
 * @Last Modified time: 2019-09-05 11:20:25
'''
'''打印各种三角形图案

*
**
***
****
*****

    *
   **
  ***
 ****
*****

    *
   ***
  *****
 *******
*********
'''
row = int(input('请输入行数：'))
#打印第一种三角形
for i in range(row):
    for j in range(i + 1):
        print('*',end='')
    print()
#打印第二种三角形
for i in range(row):
    for j in range(row):
        if j < (row-1-i):
            print(' ',end='')
        else:
            print('*',end='')
    print()
#打印第三种三角形
for i in range(row):
    for _ in range(row - i - 1):
        print(' ', end='')
    for _ in range(2 * i + 1):
        print('*', end='')
    print()
