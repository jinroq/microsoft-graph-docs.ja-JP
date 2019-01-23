---
title: iosHomeScreenApp リソースの種類
description: ホーム画面上のアプリのアイコンを表します
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dcc90e774f8d032d46968fc4f751923bcc52e559
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412325"
---
# <a name="ioshomescreenapp-resource-type"></a>iosHomeScreenApp リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ホーム画面上のアプリのアイコンを表します


[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列型 (String)|アプリの名前。[iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) から継承|
|bundleID|文字列型 (String)|アプリの BundleID|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```




