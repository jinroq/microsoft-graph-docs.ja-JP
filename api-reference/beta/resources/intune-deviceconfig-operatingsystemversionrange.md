---
title: operatingSystemVersionRange リソースの種類
description: オペレーティングシステムのバージョンの範囲。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 521f7d0b0ec4ddab728ed3b95c27acf21695b0d3
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148609"
---
# <a name="operatingsystemversionrange-resource-type"></a>operatingSystemVersionRange リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

オペレーティングシステムのバージョンの範囲。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|説明|String|この範囲の説明 (例: 有効な1702ビルド)|
|lowestversion|String|この範囲に含まれている最小の包括バージョン。|
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




