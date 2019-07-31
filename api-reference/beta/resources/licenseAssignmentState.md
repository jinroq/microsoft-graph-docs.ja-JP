---
title: License割り当て状態リソースの種類
description: 'User エンティティの**License割り当て状態**プロパティは、 **license割り当て状態**のコレクションです。 ユーザーへのライセンス割り当てに関する詳細を提供します。 詳細には、次のような情報が含まれます。  '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: d85b4e2d45739f0d82e11bf029d00cad91a0e726
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966956"
---
# <a name="licenseassignmentstate-resource-type"></a>License割り当て状態リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[User](user.md)エンティティの**license割り当て状態**プロパティは、 **license割り当て状態**のコレクションです。 ユーザーへのライセンス割り当てに関する詳細を提供します。 詳細には、次のような情報が含まれます。  

- ユーザーに対して無効になるプラン
- ライセンスがユーザーに直接割り当てられたか、グループから継承されたか。
- 割り当ての現在の状態
- 割り当ての状態がエラーの場合は、エラーの詳細がどのようなものですか。 


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedByGroup|string|このライセンスを割り当てるグループの id。 割り当てが直接割り当てられたライセンスの場合、このフィールドは Null になります。 読み取り専用です。|
|disabledPlans|Collection(String)|この割り当てで無効になっているサービスプラン。 読み取り専用です。|
|error|String|ライセンスの割り当てエラーエラー。 ライセンスが正常に割り当てられた場合、このフィールドは Null になります。 読み取り専用です。 可能な値`CountViolation`: `MutuallyExclusiveViolation`、 `DependencyViolation` `ProhibitedInUsageLocationViolation` `UniquenessViolation`、、、、 `Others`。 ライセンス割り当てエラーを特定して解決する方法について[は、こちら](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)を参照してください。|
|skuId|String|SKU の一意識別子。 読み取り専用です。|
|state|String|この割り当ての現在の状態を示します。 読み取り専用です。 使用可能な値: Active、ActiveWithError、Disabled、および Error。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.licenseAssignmentState"
}-->
```json
{
  "assignedByGroup": "String",
  "disabledPlans": ["string"],
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
