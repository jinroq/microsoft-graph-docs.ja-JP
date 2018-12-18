---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
author: tfitzmac
ms.openlocfilehash: 68fe4e7b5a226422cc0aaf980ac7fb0421a9bfc0
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350373"
---
# <a name="ioshomescreenapp-resource-type"></a>iosHomeScreenApp リソースの種類

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

ホーム画面上のアプリのアイコンを表します

[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|displayName|文字列型 (String)|アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承|
|bundleID|文字列型 (String)|アプリの BundleID|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



