---
title: windowsKioskMultipleApps リソースの種類
description: キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71b8a57151b08d0297a89dfd815f72d66c2d12a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396029"
---
# <a name="windowskioskmultipleapps-resource-type"></a>windowsKioskMultipleApps リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キオスクの構成のマルチ ・ モード ・ アプリケーションの構成を識別するために使用するクラス


[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|apps|[windowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)コレクション|これらは、[スタート] メニューから起動できる唯一の Windows ストア アプリです。 このコレクションは、最大 128 の要素を含めることができます。|
|showTaskBar|Boolean|この設定では、タスク バーを表示するかどうかを指定するのには管理ができます。|
|disallowDesktopApps|Boolean|この設定は、デスクトップ アプリケーションを許可することを示します。 デフォルトは true になります。|
|startMenuLayoutXml|Binary|開始の既定のレイアウトを変更するのには管理者は、ユーザーが変更できないようにします。レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。 XML は、バイナリ形式である必要があります。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskMultipleApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskMultipleApps",
  "apps": [
    {
      "@odata.type": "microsoft.graph.windowsKioskUWPApp",
      "startLayoutTileSize": "String",
      "name": "String",
      "appType": "String",
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```




