---
title: managedDeviceReportedApp リソースの種類
description: 報告のためのアプリケーション データ
ms.openlocfilehash: 820269422891e01352a7f605d62147a84facea67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067309"
---
# <a name="manageddevicereportedapp-resource-type"></a>managedDeviceReportedApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

報告のためのアプリケーション データ
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|appId|文字列型 (String)|アプリケーションのアプリケーションまたはバンドルの識別子|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceReportedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceReportedApp",
  "appId": "String"
}
```





