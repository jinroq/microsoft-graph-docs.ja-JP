---
title: iosMobileAppIdentifier リソースの種類
description: iOS アプリの識別子。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5dd2ee1531c2bfe2399949d2e08a209826079cb8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875839"
---
# <a name="iosmobileappidentifier-resource-type"></a>iosMobileAppIdentifier リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

iOS アプリの識別子。

[mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|bundleId|文字列型 (String)|App Store で指定されている、アプリの識別子。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



