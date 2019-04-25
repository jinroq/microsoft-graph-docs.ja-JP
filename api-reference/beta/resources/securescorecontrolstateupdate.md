---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、Default、ThirdParty、、レビュー済み) があります。
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549140"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate リソースの種類
ユーザーによって更新されたコントロールの状態の履歴が含まれます (コントロールの状態には、既定では、無視される、ThirdParty、レビューされます)。

|プロパティ |型 |説明 |
|:--|:--|:--|
|assignedTo | string | アクションを実行するユーザーにコントロールを割り当てる |
|comment | string | コントロールに関するオプションのコメントを提供します。 |
|state | string | PATCH コマンドを使用してコントロールの状態を変更できます (例: 無視、thirdParty など) |
|updatedby | string |テナント状態を更新したユーザーの ID |
|updatedDateTime | DateTimeOffset? |コントロールの状態が更新された時刻 |
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
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
