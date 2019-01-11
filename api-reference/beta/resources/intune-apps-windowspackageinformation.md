---
title: windowsPackageInformation リソースの種類
description: パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0f7f3cd593670e071ae62bdb287bcebeee01d555
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849533"
---
# <a name="windowspackageinformation-resource-type"></a>windowsPackageInformation リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

パッケージについては、ビジネス アプリケーションのウィンドウの行のプロパティが含まれています。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|applicableArchitecture|[windowsArchitecture](../resources/intune-apps-windowsarchitecture.md)|Windows のアーキテクチャでこのアプリケーションが実行できます。 可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。|
|displayName|String|表示名。|
|identityName|String|ID 名。|
|identityPublisher|String|識別情報の発行元です。|
|identityResourceIdentifier|String|ID のリソースの識別子。|
|identityVersion|String|アイデンティティのバージョンです。|
|minimumSupportedOperatingSystem|[windowsMinimumOperatingSystem](../resources/intune-apps-windowsminimumoperatingsystem.md)|該当するオペレーティング システムの最小の値です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsPackageInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsPackageInformation",
  "applicableArchitecture": "String",
  "displayName": "String",
  "identityName": "String",
  "identityPublisher": "String",
  "identityResourceIdentifier": "String",
  "identityVersion": "String",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  }
}
```





