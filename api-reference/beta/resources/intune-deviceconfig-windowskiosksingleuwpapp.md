---
title: windowsKioskSingleUWPApp リソースの種類
description: キオスクの構成の UWP アプリ情報を識別するために使用されるクラス
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3bb9c57de0e3e60d1c62adb62c3d1a274c6f853
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32574653"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a>windowsKioskSingleUWPApp リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キオスクの構成の UWP アプリ情報を識別するために使用されるクラス


[windowskioskappconfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|uwpApp|[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)|これは、キオスクモードでの使用が可能になる唯一のアプリケーションユーザーモデル ID (AUMID) です。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskSingleUWPApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskSingleUWPApp",
  "uwpApp": {
    "@odata.type": "microsoft.graph.windowsKioskUWPApp",
    "startLayoutTileSize": "String",
    "name": "String",
    "appType": "String",
    "autoLaunch": true,
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





