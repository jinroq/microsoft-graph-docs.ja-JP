---
title: operatingSystemVersionRange リソースの種類
description: オペレーティングシステムのバージョンの範囲。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b00d3df68ad0d6cf13d9b4f4a5cff541aa33893a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36368430"
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



