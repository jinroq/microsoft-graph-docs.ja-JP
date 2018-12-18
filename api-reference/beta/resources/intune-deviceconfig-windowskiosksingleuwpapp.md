---
title: windowsKioskSingleUWPApp リソースの種類
description: キオスクの構成の UWP のアプリケーション情報を識別するために使用するクラス
author: tfitzmac
ms.openlocfilehash: fd1dffd5a01b89db27132770d4c8ffe0094eed8f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312181"
---
# <a name="windowskiosksingleuwpapp-resource-type"></a>windowsKioskSingleUWPApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

キオスクの構成の UWP のアプリケーション情報を識別するために使用するクラス

[WindowsKioskAppConfiguration](../resources/intune-deviceconfig-windowskioskappconfiguration.md)から継承します。

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|uwpApp|[windowsKioskUWPApp](../resources/intune-deviceconfig-windowskioskuwpapp.md)|これは、専用アプリケーション ユーザー モデル ID (AUMID) を表示するキオスク モードでの使用を開始するのには、します。|

## <a name="relationships"></a>リレーションシップ
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
    "appUserModelId": "String",
    "appId": "String",
    "containedAppId": "String"
  }
}
```





