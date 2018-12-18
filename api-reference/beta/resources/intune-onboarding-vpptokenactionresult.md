---
title: vppTokenActionResult リソースの種類
description: アクションのステータスは、Apple ボリューム購入プログラム トークンで実行されます。
author: tfitzmac
ms.openlocfilehash: 0b8b074e879321d0aed361373c49e6ed1fd16e62
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27341679"
---
# <a name="vpptokenactionresult-resource-type"></a>vppTokenActionResult リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アクションのステータスは、Apple ボリューム購入プログラム トークンで実行されます。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|actionName|文字列型 (String)|アクション名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|アクションの状態です。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
|startDateTime|DateTimeOffset|アクションが開始された時刻|
|lastUpdatedDateTime|DateTimeOffset|アクション状態の最終更新時刻|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppTokenActionResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppTokenActionResult",
  "actionName": "String",
  "actionState": "String",
  "startDateTime": "String (timestamp)",
  "lastUpdatedDateTime": "String (timestamp)"
}
```





