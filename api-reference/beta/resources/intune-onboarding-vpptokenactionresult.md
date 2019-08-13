---
title: vppTokenActionResult リソースの種類
description: Apple Volume Purchase Program トークンを使用して実行されたアクションの状態。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b840d37963d8d8b56b0fe2ecd461b32f12368ae5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373575"
---
# <a name="vpptokenactionresult-resource-type"></a>vppTokenActionResult リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Apple Volume Purchase Program トークンを使用して実行されたアクションの状態。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|actionName|文字列型 (String)|アクション名|
|actionState|[actionState](../resources/intune-shared-actionstate.md)|アクションの状態。 可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。|
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



