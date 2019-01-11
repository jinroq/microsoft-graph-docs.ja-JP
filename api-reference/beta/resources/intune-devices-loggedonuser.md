---
title: loggedOnUser リソースの種類
description: ログオン中のユーザー
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e832c6452b73a6fad39723675acb129d79c2b888
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859753"
---
# <a name="loggedonuser-resource-type"></a>loggedOnUser リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ログオン中のユーザー
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|userId|String|ユーザー id|
|lastLogOnDateTime|DateTimeOffset|ユーザーのログオン時の日付します。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```





