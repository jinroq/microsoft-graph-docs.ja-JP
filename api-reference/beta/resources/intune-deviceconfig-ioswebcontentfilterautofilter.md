---
title: iosWebContentFilterAutoFilter リソースの種類
description: IOS iOS の自動フィルター機能を有効にし、その他の URL のアクセス制御では、Web コンテンツ フィルター設定の種類を表します。 構築すると、プロパティ値を持たない、iOS デバイスは、自動でフィルター処理に関係なく有効になります。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d5be275b74e2675881b9d36b047e2017ef95adb2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401230"
---
# <a name="ioswebcontentfilterautofilter-resource-type"></a>iosWebContentFilterAutoFilter リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

IOS iOS の自動フィルター機能を有効にし、その他の URL のアクセス制御では、Web コンテンツ フィルター設定の種類を表します。 構築すると、プロパティ値を持たない、iOS デバイスは、自動でフィルター処理に関係なく有効になります。


[IosWebContentFilterBase](../resources/intune-deviceconfig-ioswebcontentfilterbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|allowedUrls|String コレクション|追加の Url のアクセス許可|
|blockedUrls|String コレクション|追加の Url アクセスのブロック|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosWebContentFilterAutoFilter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosWebContentFilterAutoFilter",
  "allowedUrls": [
    "String"
  ],
  "blockedUrls": [
    "String"
  ]
}
```




