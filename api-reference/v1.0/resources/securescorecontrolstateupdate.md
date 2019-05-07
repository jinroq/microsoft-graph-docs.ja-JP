---
title: secureScoreControlStateUpdate リソースの種類
description: このリソースには、ユーザーが更新したコントロールの状態の履歴が含まれています (コントロールの状態には、Default、ThirdParty、、レビュー済み) などがあります。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: ac66fb2085949e375c79b18bfdfd39e84392159d
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629251"
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
