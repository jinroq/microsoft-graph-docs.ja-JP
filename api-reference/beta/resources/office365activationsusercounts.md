---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.openlocfilehash: f57393a538631664be8845fdaeda9f35d07c986f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849309"
---
# <a name="office365activationsusercounts-resource-type"></a>office365ActivationsUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                 | 種類   | 説明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日付   | コンテンツの最新の日付。          |
| productType              | String | 「Office 365 用リソース"、「プロジェクト クライアント」などの製品の種類または"Office 365"の Visio Pro です。 |
| 割り当てられています。                 | Int64  | ユーザーの数は、製品のライセンスの割り当てられています。 |
| アクティブ化                | Int64  | 製品をアクティブにしているユーザーの数です。 |
| sharedComputerActivation | Int64  | 共有のコンピューターで製品を使用したユーザーの数です。 |

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.office365ActivationsUserCounts"
} -->

```json
{
  "reportRefreshDate": "Date", 
  "productType": "String", 
  "assigned": 1024, 
  "activated": 1024,
  "sharedComputerActivation": 1024
}
```
