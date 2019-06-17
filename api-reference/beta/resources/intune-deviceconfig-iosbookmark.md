---
title: iosBookmark リソースの種類
description: iOS URL ブックマーク
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9d2f96b872d09eaf3c954f18a31219d6bfe17ddb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34988364"
---
# <a name="iosbookmark-resource-type"></a>iosBookmark リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS URL ブックマーク

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|url|String|アクセスが許可されている URL|
|bookmarkFolder|String|ブックマークを Safari で追加するフォルダー|
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





