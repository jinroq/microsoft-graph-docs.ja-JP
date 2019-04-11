---
title: iosbookmark リソースの種類
description: iOS URL ブックマーク
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5231ccbae496e310e414c6429190e0b4d53cbaa7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782801"
---
# <a name="iosbookmark-resource-type"></a>iosbookmark リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS URL ブックマーク

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|url|String|アクセスが許可されている URL|
|bookmarkFolder|文字列|ブックマークを Safari で追加するフォルダー|
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





