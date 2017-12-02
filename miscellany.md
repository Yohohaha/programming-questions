- 程序开发过程
  - 程序开发的定义？
    - 程序开发就是根据面对的问题，最终得到一个可以解决问题的程序的工作过程。
  - 工作流程
    - 分析
    - 设计
      - 设计一个计算过程模型
        - 数据
        - 算法
 ```flow
st=>start: 问题
op1=>operation: 分析，严格化
op2=>operation: 设计
op3=>operation: 编码
cond=>condition: 检查，编译
op4=>operation: 测试/调试
e=>end: 完成的程序

st->op1->op2->op3->cond->op4->e
cond(no)->op3
cond(yes)->op4
 ```
- 问题的说明性描述与操作性描述的理解？
  - 说明性描述其实就是提出一个问题
  - 操作性描述就是这个问题的求解方法