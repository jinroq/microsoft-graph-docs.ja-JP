---
title: iosBookmark リソースの種類
description: iOS URL ブックマーク
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9310ffe3a664b3fc02e9f498a2c5312dc6683b53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36004345"
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





