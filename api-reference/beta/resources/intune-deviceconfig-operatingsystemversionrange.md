---
title: operatingSystemVersionRange リソースの種類
description: オペレーティングシステムのバージョンの範囲。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a123c645262986711dbe28cc170443f948d2f5c
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987902"
---
# <a name="operatingsystemversionrange-resource-type"></a>operatingSystemVersionRange リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

オペレーティングシステムのバージョンの範囲。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|description|String|この範囲の説明 (例: 有効な1702ビルド)|
|lowestVersion|String|この範囲に含まれている最小の包括バージョン。|
|highestVersion|String|この範囲に含まれている最も高い包括バージョン。|

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





