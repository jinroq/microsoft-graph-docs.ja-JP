---
title: windowsKioskAppBase リソースの種類
description: アプリの種類の基本クラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 167244028d1d0773caf1802092d70a1cf3ec7560
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371034"
---
# <a name="windowskioskappbase-resource-type"></a>windowsKioskAppBase リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリの種類の基本クラス

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|開始レイアウトのアプリタイルのサイズ。 可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。|
|name|String|アプリのフレンドリ名を表します。|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|アプリの種類。 使用可能な値は、`unknown`、`store`、`desktop`、`aumId` です。|
|autoLaunch|Boolean|アプリをマルチアプリキオスクモードで自動起動できるようにする|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAppBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAppBase",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true
}
```



