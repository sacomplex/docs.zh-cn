---
title: true 和 false 运算符 - C# 参考
ms.custom: seodec18
ms.date: 12/10/2018
helpviewer_keywords:
- false operator [C#]
- true operator [C#]
ms.assetid: 81a888fd-011e-4589-b242-6c261fea505e
ms.openlocfilehash: ff8b14413d60761cb28fe8e739a8ee75816a71b0
ms.sourcegitcommit: 8699383914c24a0df033393f55db3369db728a7b
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/15/2019
ms.locfileid: "65633753"
---
# <a name="true-and-false-operators-c-reference"></a>true 和 false 运算符（C# 参考）

`true` 运算符返回 [bool](bool.md) 值 `true`，以指明操作数一定为 true。 `false` 运算符返回 `bool` 值 `true`，以指明操作数一定为 false。 无法确保 `true` 和 `false` 运算符互补。 也就是说，`true` 和 `false` 运算符可能同时针对同一个操作数返回 `bool` 值 `false`。 如果某类型定义这两个运算符之一，它还必须定义另一个运算符。

如果包含已定义 `true` 和 `false` 运算符的类型以某种方式[重载](operator.md)[逻辑 OR 运算符](../operators/boolean-logical-operators.md#logical-or-operator-) `|` 或[逻辑 AND 运算符](../operators/boolean-logical-operators.md#logical-and-operator-) `&`，可以对相应类型的操作数分别执行[条件逻辑 OR 运算符](../operators/boolean-logical-operators.md#conditional-logical-or-operator-) `||` 或[条件逻辑 AND 运算符](../operators/boolean-logical-operators.md#conditional-logical-and-operator-) `&&` 运算。 有关详细信息，请参阅 [C# 语言规范](../language-specification/index.md)的[用户定义条件逻辑运算符](~/_csharplang/spec/expressions.md#user-defined-conditional-logical-operators)部分。

包含已定义 `true` 运算符的类型可以是 [if](if-else.md)、[do](do.md)、[while](while.md) 和 [for](for.md) 语句以及[条件运算符 `?:`](../operators/conditional-operator.md) 中控制条件表达式的结果的类型。 有关详细信息，请参阅 [C# 语言规范](../language-specification/index.md)中的 [Boolean 表达式](~/_csharplang/spec/expressions.md#boolean-expressions)部分。

> [!TIP]
> 如需支持三值逻辑（例如，在使用支持三值布尔类型的数据库时），请使用 `bool?` 类型。 C# 提供 `&` 和 `|` 运算符，它们通过 `bool?` 操作数支持三值逻辑。 有关详细信息，请参阅[布尔逻辑运算符](../operators/boolean-logical-operators.md)一文的[可以为 null 的布尔逻辑运算符](../operators/boolean-logical-operators.md#nullable-boolean-logical-operators)部分。

下面的示例展示了定义 `true` 和 `false` 运算符的类型。 此外，它还重载了逻辑 AND 运算符 `&`，因此也可以对相应类型的操作数执行运算符 `&&` 运算。

[!code-csharp-interactive[true and false operators example](~/samples/snippets/csharp/keywords/TrueFalseOperatorsExample.cs)]

请注意 `&&` 运算符的短路行为。 当 `GetFuelLaunchStatus` 方法返回 `LaunchStatus.Red` 时，不会计算 `&&` 运算符的第二个操作数。 这是因为 `LaunchStatus.Red` 一定为 false。 然后，逻辑 AND 运算符的结果不依赖第二个操作数的值。 示例输出如下所示：

```console
Getting fuel launch status...
Wait!
```

## <a name="see-also"></a>请参阅

- [C# 参考](../index.md)
- [C# 编程指南](../../programming-guide/index.md)
- [C# 关键字](index.md)
- [C# 运算符](../operators/index.md)
- [`true` 文本](true-literal.md)
- [`false` 文本](false-literal.md)
