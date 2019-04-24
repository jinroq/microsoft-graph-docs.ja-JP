---
title: license割り当て状態リソースの種類
description: user エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**オブジェクトのコレクションです。 ユーザーへのライセンス割り当てに関する詳細を提供します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 0822c975ab81badf5334881bb460532161858010
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585147"
---
# <a name="licenseassignmentstate-resource-type"></a>license割り当て状態リソースの種類


[user](user.md)エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**オブジェクトのコレクションです。 ユーザーへのライセンス割り当てに関する詳細を提供します。 詳細には、次のような情報が含まれます。  

 - ユーザーに対して無効になるプラン
 - ライセンスがユーザーに直接割り当てられたか、グループから継承されたか。
 - 割り当ての現在の状態
 - 割り当ての状態がエラーの場合のエラーの詳細 


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedByGroup|string|このライセンスを割り当てるグループの id。 割り当てが直接割り当てられたライセンスの場合、このフィールドは Null になります。 読み取り専用です。|
|disabledPlans|Collection(String)|この割り当てで無効になっているサービスプラン。 読み取り専用です。|
|error|String|ライセンスの割り当てエラーエラー。 ライセンスが正常に割り当てられた場合、このフィールドは Null になります。 読み取り専用です。 可能な値`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、、、 `Others`。 ライセンス割り当てエラーを特定して解決する方法について[は、こちら](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)を参照してください。|
|skuId|String|SKU の一意識別子。 読み取り専用です。|
|state|String|この割り当ての現在の状態を示します。 読み取り専用です。 使用可能な値: Active、activewitherror、Disabled、および error。|

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
