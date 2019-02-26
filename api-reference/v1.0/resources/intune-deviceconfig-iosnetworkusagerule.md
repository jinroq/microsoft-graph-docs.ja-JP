---
title: iosNetworkUsageRule リソースの種類
description: ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 516e880e4b6230ca165426b849f57609dcc6e6ad
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250104"
---
# <a name="iosnetworkusagerule-resource-type"></a>iosNetworkUsageRule リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|managedApps|[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション|このルールが適用される管理対象アプリに関する情報です。 このコレクションには、最大で 500 個の要素を含めることができます。|
|cellularDataBlockWhenRoaming|Boolean|true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。|
|cellularDataBlocked|Boolean|true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



