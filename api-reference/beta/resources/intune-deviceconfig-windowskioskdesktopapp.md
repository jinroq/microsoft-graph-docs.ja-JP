---
title: windowsKioskDesktopApp リソースの種類
description: アプリケーションの型の基本クラス
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 831ed86da24791cde549687ecaff42cabc29a99e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415307"
---
# <a name="windowskioskdesktopapp-resource-type"></a>windowsKioskDesktopApp リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アプリケーションの型の基本クラス


[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される開始レイアウトのアプリケーションのタイルのサイズです。 可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。|
|name|String|[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される、アプリケーションのフレンドリ名を表す|
|appType|[windowsKioskAppType](../resources/intune-deviceconfig-windowskioskapptype.md)|[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)からアプリケーション型継承します。 可能な値は、`unknown`、`store`、`desktop`、`aumId` です。|
|path|String|デスクトップ アプリケーションのパスを定義します。|
|desktopApplicationId|String|アプリケーションの DesktopApplicationID を定義します。|
|desktopApplicationLinkPath|String|アプリケーションの DesktopApplicationLinkPath を定義します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskDesktopApp",
  "startLayoutTileSize": "String",
  "name": "String",
  "appType": "String",
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```




