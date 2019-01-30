---
title: licenseAssignmentState リソースの種類
description: 'ユーザー エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。 詳細には、ような情報が含まれています。  '
localization_priority: Normal
ms.openlocfilehash: a33dce3550d5a842493b73c83e8222a579348c9a
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641681"
---
# <a name="licenseassignmentstate-resource-type"></a>licenseAssignmentState リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[ユーザー](user.md)エンティティの**licenseAssignmentStates**プロパティは、 **licenseAssignmentState**のコレクションです。 ユーザー ライセンスの割り当てに関する詳細情報を提供します。 詳細には、ような情報が含まれています。  

 - ユーザーに対してどのようなプランが無効になっています。
 - ライセンスをユーザーに直接割り当てられているか、グループから継承されたかどうか
 - 割り当ての現在の状態
 - 代入の状態がエラーの場合は、エラーのエラーの詳細は? 


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assignedByGroup|string|このライセンスを割り当てられるグループの id。 割り当てがダイレクトに割り当てられたライセンスの場合は、このフィールドは Null になります。 読み取り専用です。|
|disabledPlans|Collection(String)|この割り当て内で無効になっているサービス プランです。 読み取り専用です。|
|エラー|String|ライセンスの割り当てエラーです。 ライセンスが正常に割り当てられると、このフィールドが Null になります。 読み取り専用です。 使用可能な値: `CountViolation`、 `MutuallyExclusiveViolation`、 `DependencyViolation`、 `ProhibitedInUsageLocationViolation`、`UniquenessViolation`と`Others`。 エラーを特定し、ライセンスの割り当てを解決する方法の詳細について参照してください[ここで](https://docs.microsoft.com/azure/active-directory/users-groups-roles/licensing-groups-resolve-problems)。|
|skuId|String|SKU の一意識別子。 読み取り専用です。|
|state|String|この割り当ての現在の状態を示します。 読み取り専用です。 使用可能な値: アクティブ、ActiveWithError、無効になり、エラーです。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

```json
{
  "assignedByGroup": "String",
  "disabledPlans": "Collection(String)",
  "error": " String ",  
  "skuId": "String ",
  "state": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/licenseAssignmentState.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
