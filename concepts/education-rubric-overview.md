---
title: 教育機関ルーブリックの概要
description: ルーブリックは、効果的で広く使用されている課題の評価方法で、Microsoft Graph の教育機関 API によってサポートされています。
author: mmast-msft
localization_priority: Priority
ms.prod: education
ms.openlocfilehash: 56b9bcdf32036361fb92fe372952c94d09d8dc57
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173084"
---
# <a name="education-rubric-overview"></a>教育機関ルーブリックの概要

ルーブリックは、効果的で広く使用されている課題の評価方法で、Microsoft Graph の教育機関 API によってサポートされています。

評価ルーブリックは、次のような*品質*、*レベル*、*基準*のマトリックスです。

| | レベル | レベル |
|:--|:--|:--|
| 品質 | 基準 | 基準 |
| 品質 | 基準 | 基準 |

評価ルーブリックの例は、次のとおりです:

| | 良い | 悪い |
|:--|:--|:--|
| 主張 | エッセイの主張に、説得力があります。 | エッセイの主張に、筋が通っていません。 |
| スペルと文法 | エッセイのスペルと文法は正しく、ほとんどまたは全く誤りがありません。 | エッセイには、多くのスペルや文法の誤りがあります。 |

ルーブリックを使用した評価には、ルーブリックの各*品質*に対して 1 つの*レベル*を選択する必要があります。

ルーブリックには、各レベルに関連付けられたポイントと、各品質に関連付けられた重みが*あります*。  存在する場合、重みは最大で 100 になります。

| | 良い (2 ポイント) | 悪い (1 ポイント) |
|:--|:--|:--|
| 主張 (重み 50) | エッセイの主張に、説得力があります。 | エッセイの主張に、筋が通っていません。 |
| スペルと文法 (重み 50) | エッセイのスペルと文法は正しく、ほとんどまたは全く誤りがありません。 | エッセイには、多くのスペルや文法の誤りがあります。 |

## <a name="api-reference"></a>API リファレンス

ルーブリックの使用を開始するには、[Microsoft Graph ベータ版の educationRubric リソースおよび関連メソッド](/graph/api/resources/educationrubric?view=graph-rest-beta)から始めます。





 

