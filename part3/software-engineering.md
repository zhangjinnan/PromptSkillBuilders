# 产品经理

```
假设你就是一个资深产品经理，有丰富的小团队敏捷开发经验。请根据“用户故事背景”所描述的需求，采用敏捷开发的方法，通过一步步的分析需求和思考，编写一个让研发人员可以清晰了解需求的用户故事。
用户故事背景：
###
现在在一个CRM系统，需要设计普通用户的注册和登录功能。
###
用户故事要求：
##
- 用户故事标题
- 用户角色
- 用户目标
- 描述
- 验收标准
```

# 测试人员

作为一个测试人员，编写测试用例的Prompt，通过用户故事来编写让语言大模型编写测试用例。

```
假设你就是一名资深的测试经理，现在需要根据“用户故事”来设计验证的测试用例，测试用例的模板参考“测试用例要求”所包含的要素进行编写，通过一步步的思考，尽可能全的覆盖用户故事的测试用例。
用户故事：
###
在CRM系统中，我作为一个普通销售角色的用户注册，需要输入用户名、密码、邮箱地址进行注册，注册成功后可以收到注册邮件。
###
测试用例要求：
##
- 测试目标
- 操作步骤
- 测试数据
- 预期结果
- 边界条件
- 清理步骤
```


# 研发人员

作为研发，可以利用大模型提供辅助代码的能力。

```
假设你就是一个资深的python开发人员，现在需要根据“用户故事”一步步来编写代码，编写代码尽量符合“代码规范”要求。
用户故事：
###
在CRM系统中，我作为一个普通销售角色的用户注册，需要输入用户名、密码、邮箱地址进行注册，注册成功后可以收到注册邮件。
###
代码规范：
##
- 先提供代码设计逻辑
- 关键步骤提供详细注释
- 尽可能的考虑代码质量
```


# 研发经理

```
假设你就是一个资深研发经理，有10年的python研发经验。现在需要对开发人员提供的“代码”按照“评审规范”一步步的进行评审并给出意见，如代码有BUG请明确指出BUG的地方并予以修正。
代码：
###
def bubbleSort(arr):
    n = len(arr)

    for i in range(n+1):
 
        # Last i elements are already in place
        for j in range(0, n-i-1):
 
            if arr[j] > arr[j+1] :
                arr[j], arr[j+1] = arr[j+1], arr[j]
 
arr = [64, 34, 25, 12, 22, 11, 90]
 
bubbleSort(arr)
 
print ("排序后的数组:")
for i in range(len(arr)):
    print ("%d" %arr[i]),
###
评审规范：
##
- 代码是否存在BUG
- 关键步骤注释是否缺失
- 代码是否可以更加简洁
```