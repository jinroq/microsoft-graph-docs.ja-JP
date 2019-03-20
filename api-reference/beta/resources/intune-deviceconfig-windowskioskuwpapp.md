---
title: windowsKioskUWPApp リソースの種類
description: アプリの種類の基本クラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a247c3f02dc64657ec9cd297d8fff5d8591549cd
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572538"
---
# <a name="windowskioskuwpapp-resource-type"></a>windowsKioskUWPApp リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリの種類の基本クラス


[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承された開始レイアウトのアプリタイルサイズ。 可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。|
|name|String|[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたアプリのフレンドリ名を表します。|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されるアプリの種類。 可能な値は、`unknown`、`store`、`desktop`、`aumId` です。|
|autoLaunch|Boolean|[windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承されたマルチアプリキオスクモードでアプリを自動起動することを許可します。|
|appUserModelId|String|これは、キオスクモードでの使用が可能になる唯一のアプリケーションユーザーモデル ID (AUMID) です。|
|appId|String|これは、キオスクの構成と同じ割り当てに移行する Intune アプリを参照します。|
|containedAppId|String|これは、Intune アプリからの含まれているアプリを参照します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskUWPApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "autoLaunch": true,
  "appUserModelId": "String",
  "appId": "String",
  "containedAppId": "String"
}
```




