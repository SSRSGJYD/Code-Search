## Requirements of Coding in Python and JavaScript

#### Requirement 1

| Need        | 用户希望可以自动为我写的代码生成测试代码                     |
| ----------- | ------------------------------------------------------------ |
| Approach    | 构建一个模型，以被测试的代码为输入，测试代码为输出，在已有的代码库的基础上进行学习，从而可以生成测试代码。 |
| Benefit     | 节省了大量重复性的劳动，降低软件开发成本。                   |
| Competitors | To my best knowledge, 暂时没有这样的工具。                   |
| Delivery    | 通过编辑器插件的形式进行推广。                               |

#### Requirement 2

| Need        | 用户希望可以在开源代码和各种教程、文档上根据需要搜索对应的API用法 |
| ----------- | ------------------------------------------------------------ |
| Approach    | 构建一个模型，输入用户的需求描述，输出最可能有帮助的API。训练模型后，爬取开源代码以及较为权威可靠的教程、文档的内容构建搜索库。 |
| Benefit     | 方便程序员查询需要的API，提高编码效率。                      |
| Competitors | 有一些关于此任务的研究，但是缺少落地产品。                   |
| Delivery    | 通过编辑器插件的形式进行推广，或者采用网站搜索的方式。       |

#### Requirement 3

| Need        | 用户希望可以根据代码上下文自动生成后面的代码                 |
| ----------- | ------------------------------------------------------------ |
| Approach    | 构建一个模型，以当前的代码为输入，要补充的代码为输出         |
| Benefit     | 节省了大量重复性的劳动，提高编码效率。                       |
| Competitors | 目前有关于根据功能搜索代码的研究，但是无法自动根据上下文直接生成代码，只能提供API或参考代码 |
| Delivery    | 通过编辑器插件的形式进行推广。                               |

