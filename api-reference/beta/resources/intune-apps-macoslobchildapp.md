---
title: macOSLobChildApp リソースの種類
description: バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 43f207bb2cebccdd01c791694674c6fbf96b631f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954233"
---
# <a name="macoslobchildapp-resource-type"></a>macOSLobChildApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

バンドル パッケージに MacOS の LOB アプリケーションのプロパティが含まれています
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|bundleId|String|ID 名。|
|buildNumber|String|MacOS の基幹業務 (LoB) アプリケーションのビルド番号です。|
|VersionNumber|String|MacOS の基幹業務 (LoB) アプリケーションのバージョン番号です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





