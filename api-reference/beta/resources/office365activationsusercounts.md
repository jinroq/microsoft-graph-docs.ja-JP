---
title: office365ActivationsUserCounts リソースの種類
description: リソースの JSON 表記を次に示します。
localization_priority: Normal
ms.prod: reports
author: pranoychaudhuri
doc_type: resourcePageType
ms.openlocfilehash: 33339578f498460aacd24481f166ab717138f8fa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966567"
---
# <a name="office365activationsusercounts-resource-type"></a>office365ActivationsUserCounts リソースの種類

## <a name="properties"></a>プロパティ

| プロパティ                 | 型   | 説明                              |
| :----------------------- | :----- | ---------------------------------------- |
| reportRefreshDate        | 日付   | コンテンツの最新の日付。          |
| productType              | String | "Office 365 ProPlus"、"Project Client"、または "Visio Pro for Office 365" などの製品の種類。 |
| ら                 | Int64  | 製品ライセンスに割り当てられているユーザーの数。 |
| アクティブ化                | Int64  | 製品をライセンス認証したユーザーの数。 |
| sharedComputerActivation | Int64  | 共有コンピューターで製品を使用したユーザーの数。 |

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
