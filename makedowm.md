**标题**

# 一级标题

## 二级标题

### 三级标题

**表格**

| 列 1 | 列 2 | 列 3 |
| ---- | ---- | ---- |
| 行 1 | 行 1 | 行 1 |
| 行 2 | 行 2 | 行 2 |

**无序列表**

- 无序列表
- 无序列表
  - 无序列表

**有序列表**

1. 有序列表
2. 有序列表
   1. 有序列表

**TodoList**

- [x] A
- [x] B
- [x] C

      | 左对齐 | 居中对齐 | 右对齐 |
      | :--- | :----: | ----: |
      | a | b | c |

**注释**

> 这里可以加注释

文字形式

这里是*斜体*

这里是**粗体**

这里是**_斜体和粗体_**

这里是`变量名`内容

```HTML


```

> 点灯

    RCC_APB2PeriphClockCmd(RCC_APB2Periph_GPIOA,ENABLE);

    GPIO_InitTypeDef GPIO_InitStructure;
    GPIO_InitStructure.GPIO_Mode=GPIO_Mode_Out_PP;
    GPIO_InitStructure.GPIO_Pin=GPIO_Pin_0;
    GPIO_InitStructure.GPIO_Speed=GPIO_Speed_50MHz;
    GPIO_Init(GPIOA,&GPIO_InitStructure);

GPIO_SetBits(GPIOA,GPIO_Pin_0);

> 电灯
> GPIO_ResetBits(GPIOA,GPIO_Pin_0);
> 灭灯
> GPIO_WriteBit(GPIOA,GPIO_Pin_0,Bit_SET);
> 可点可灭

推挽输出高低电平均有驱动能力
GPIO_InitStructure.GPIO_Mode=GPIO_Mode_Out_PP
开漏输出高电平没有有驱动能力，低电平有
GPIO_InitStructure.GPIO_Mode=GPIO_Mode_Out_OD

### 运用函数

1. 打开库函数 gpio.h
2. 拉到最下面找函数
3. 函数的定义
4.
