---
title: operatingSystemVersionRange リソースの種類
description: オペレーティング システムのバージョンの範囲です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 56df6b53dc29247d3f718ad185152069a071a0f7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875804"
---
# <a name="operatingsystemversionrange-resource-type"></a>operatingSystemVersionRange リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

オペレーティング システムのバージョンの範囲です。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|説明|String|この範囲 (有効 1702 のビルドなど) の説明|
|lowestVersion|String|最小包括的なバージョンをこの範囲に含まれています。|
|highestVersion|String|この範囲に含まれている最高の包括的なバージョンです。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operatingSystemVersionRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.operatingSystemVersionRange",
  "description": "String",
  "lowestVersion": "String",
  "highestVersion": "String"
}
```





