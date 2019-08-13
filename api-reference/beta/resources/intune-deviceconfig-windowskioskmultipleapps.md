---
title: Windowskiosk多重アプリリソースの種類
description: キオスク構成でのマルチモードアプリの構成を識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cbe64a4c58d405c0ea43e6201f3207169f3c1268
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36370852"
---
# <a name="windowskioskmultipleapps-resource-type"></a>Windowskiosk多重アプリリソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キオスク構成でのマルチモードアプリの構成を識別するために使用されるクラス


[Windowskioskappconfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|apps|[Windowskioskappbase](../resources/intune-deviceconfig-windowskioskappbase.md)コレクション|[スタート] メニューから起動できる Windows ストアアプリは次のとおりです。 このコレクションには、最大128個の要素を含めることができます。|
|showTaskBar バー|Boolean|この設定では、管理者がタスクバーを表示するかどうかを指定できます。|
|allowAccessToDownloadsFolder|Boolean|この設定では、エクスプローラーの [ダウンロード] フォルダーにアクセスできます。|
|disallowDesktopApps|Boolean|この設定は、デスクトップアプリが許可されていることを示します。 既定値は true です。|
|startMenuLayoutXml|Binary|管理者が既定の開始レイアウトを上書きし、ユーザーがそれを変更できないようにします。レイアウトを変更するには、レイアウト変更スキーマに基づく XML ファイルを指定します。 XML はバイナリ形式である必要があります。|

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
      "autoLaunch": true,
      "appUserModelId": "String",
      "appId": "String",
      "containedAppId": "String"
    }
  ],
  "showTaskBar": true,
  "allowAccessToDownloadsFolder": true,
  "disallowDesktopApps": true,
  "startMenuLayoutXml": "binary"
}
```



