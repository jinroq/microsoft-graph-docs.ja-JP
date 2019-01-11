---
title: windowsKioskDesktopApp リソースの種類
description: アプリケーションの型の基本クラス
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 53eb615dcd1ba2b88c6cdd4bb5a1b76b83b67eaf
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830976"
---
# <a name="windowskioskdesktopapp-resource-type"></a>windowsKioskDesktopApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

アプリケーションの型の基本クラス

[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|startLayoutTileSize|[windowsAppStartLayoutTileSize](../resources/intune-deviceconfig-windowsappstartlayouttilesize.md)|[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される開始レイアウトのアプリケーションのタイルのサイズです。 可能な値は、`hidden`、`small`、`medium`、`wide`、`large` です。|
|名前|String|[WindowsKioskAppBase](../resources/intune-deviceconfig-windowskioskappbase.md)から継承される、アプリケーションのフレンドリ名を表す|
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
  "path": "String",
  "desktopApplicationId": "String",
  "desktopApplicationLinkPath": "String"
}
```





