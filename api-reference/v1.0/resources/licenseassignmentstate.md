---
title: licenseAssignmentState リソースの種類
description: ユーザー エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**オブジェクトのコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29649437"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState リソースの種類


[ユーザー](user.md)エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**オブジェクトのコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。 詳細情報には、次のような情報があります。  

 - ユーザーに対してどのようなプランが無効になっています。
 - ライセンスをユーザーに直接割り当てられているか、グループから継承されたかどうか
 - 割り当ての現在の状態
 - 割り当ての状態がエラーの場合、エラーの詳細 


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedByGroup|string|このライセンスを割り当てられるグループの id。 割り当てがダイレクトに割り当てられたライセンスの場合は、このフィールドは Null になります。 読み取り専用です。|
|disabledPlans|Collection(String)|この割り当て内で無効になっているサービス プランです。 読み取り専用です。|
|エラー|文字列|ライセンスの割り当てエラーです。 ライセンスが正常に割り当てられると、このフィールドが Null になります。 読み取り専用です。 使用可能な値: `CountViolation`、 `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation`、`UniquenessViolation`と`Others`。 エラーを特定し、ライセンスの割り当てを解決する方法の詳細について参照してください[ここで](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|skuId|文字列|SKU の一意識別子。 読み取り専用です。|
|state|文字列|この割り当ての現在の状態を示します。 読み取り専用です。 使用可能な値: アクティブ、ActiveWithError、無効になり、エラーです。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "licenseAssignmentState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.user/licenseAssignmentStates:
      Referenced type microsoft.graph.licenseAssignmentState is not defined in the doc set! Potential suggestion: UNKNOWN"
  ]
}-->
