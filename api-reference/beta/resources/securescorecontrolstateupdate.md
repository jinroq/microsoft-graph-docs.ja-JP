---
title: " secureScoreControlStateUpdate リソースの種類"
description: このリソースには、ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641730"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>secureScoreControlStateUpdate リソースの種類
ユーザーによって更新されたコントロールの状態の履歴が含まれています (コントロールの状態は、既定、無視、サード ・ パーティ、レビュー済み)。

|プロパティ |型 |説明 |
|:--|:--|:--|
|assignedTo | string | 処理はユーザーにコントロールを割り当てる |
|comment | string | コントロールに関するオプションのコメントを提供します。 |
|state | string | 修正プログラムのコマンドを使用してコントロールの状態を変更することができます (Ex: 無視され、サード ・ パーティなど) |
|updatedBy | string |テナントの状態を更新したユーザーの ID |
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
