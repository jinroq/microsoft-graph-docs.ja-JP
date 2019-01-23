---
title: iosBookmark リソースの種類
description: iOS の URL のブックマーク
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e95f3bfd40bdf5ca5782aa9233a020623d32d6a5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395910"
---
# <a name="iosbookmark-resource-type"></a>iosBookmark リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS の URL のブックマーク

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|url|String|URL のアクセスを許可|
|bookmarkFolder|String|フォルダーには、Safari でブックマークを追加します。|
|displayName|String|ブックマークの表示名|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosBookmark"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosBookmark",
  "url": "String",
  "bookmarkFolder": "String",
  "displayName": "String"
}
```




