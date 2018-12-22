---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/22/2018
ms.locfileid: "27428841"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate リソースの種類
ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。

|プロパティ |型 |説明 |
|:--|:--|:--|
|担当者 | 文字列 | 処理はユーザーにコントロールを割り当てる |
|comment | 文字列 | コントロールに関するオプションのコメントを提供します。 |
|state | 文字列 | 修正プログラムのコマンドを使用してコントロールの状態を変更することができます (Ex: 無視され、サード ・ パーティなど) |
|updatedBy | 文字列 |テナントの状態を更新したユーザーの ID |
|updatedDateTime | DateTimeOffset でしょうか。 |コントロールの状態が更新された時間 |
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
