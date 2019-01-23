---
title: win32LobAppProductCodeDetection リソースの種類
description: Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f5af1cfc5fffe5241ef3b7883c3ebe6a2100278
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411205"
---
# <a name="win32lobappproductcodedetection-resource-type"></a>win32LobAppProductCodeDetection リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています


[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|productCode|String|Win32 基幹業務 (LoB) アプリケーションの製品コードです。|
|productVersionOperator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|製品のバージョンを検出する演算子です。 可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。|
|productVersion|String|Win32 基幹業務 (LoB) アプリケーションの製品バージョン。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```




