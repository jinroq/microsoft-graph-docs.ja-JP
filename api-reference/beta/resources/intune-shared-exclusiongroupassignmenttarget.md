---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 24e732bc0c48c9c25f35da1afbccef04d17fe0cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919863"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a>exclusionGroupAssignmentTarget リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

割り当てから除外するグループを表します。

[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|groupId|文字列|割り当てのターゲットとなるグループ ID です。 [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```





