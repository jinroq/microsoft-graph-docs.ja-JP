---
title: secureScoreControlStateUpdate リソースの種類
description: このリソースには、ユーザーが更新したコントロールの状態の履歴が含まれています (コントロールの状態には、Default、ThirdParty、、レビュー済み) などがあります。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 9e051f2c4319a2b2ae1e3dbd9ba633785a345c4a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034476"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate リソースの種類

ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、既定では、無視される、ThirdParty、レビューされます)。

## <a name="properties"></a>プロパティ

|プロパティ |型 |説明 |
|:--|:--|:--|
|assignedTo|String|アクションを実行するユーザーにコントロールを割り当てます。 |
|comment|String|コントロールに関するコメント (省略可能) を提供します。 |
|state|String|コントロールの状態。 PATCH コマンドで変更することができます (たとえば、無視、thirdParty)。 |
|updatedBy|String|テナントの状態を更新したユーザーの ID。 |
|updatedDateTime|DateTimeOffset|コントロールの状態が更新された時刻。 |

## <a name="json-representation"></a>JSON 表記
 リソースの JSON 表記を次に示します。
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
    
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "String (timestamp)"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
