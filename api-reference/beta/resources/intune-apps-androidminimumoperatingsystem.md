---
title: androidMinimumOperatingSystem リソースの種類
description: Android モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 96b68aa12a1cbd0abe2b7761b44a0ef9a5863048
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27875867"
---
# <a name="androidminimumoperatingsystem-resource-type"></a>androidMinimumOperatingSystem リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Android モバイル アプリに必要な最小限のオペレーティング システムのプロパティが含まれます。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|v4_0|ブール型 (Boolean)|バージョン 4.0 以降。|
|v4_0_3|ブール型 (Boolean)|バージョン 4.0.3 以降。|
|v4_1|ブール型 (Boolean)|バージョン 4.1 以降。|
|v4_2|ブール型 (Boolean)|バージョン 4.2 以降。|
|v4_3|ブール型 (Boolean)|バージョン 4.3 以降。|
|v4_4|ブール型 (Boolean)|バージョン 4.4 以降。|
|v5_0|ブール型 (Boolean)|バージョン 5.0 以降。|
|v5_1|ブール型 (Boolean)|バージョン 5.1 以降。|
|v6_0|ブール型|6.0 またはそれ以降のバージョンです。|
|v7_0|ブール型|7.0 またはそれ以降のバージョンです。|
|v7_1|ブール型|7.1 以降のバージョンです。|
|v8_0|ブール型 (Boolean)|バージョン 8.0 以降。|
|v8_1|ブール型 (Boolean)|8.1 またはそれ以降のバージョンです。|
|v9_0|ブール型 (Boolean)|バージョン 9.0 以降。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMinimumOperatingSystem",
  "v4_0": true,
  "v4_0_3": true,
  "v4_1": true,
  "v4_2": true,
  "v4_3": true,
  "v4_4": true,
  "v5_0": true,
  "v5_1": true,
  "v6_0": true,
  "v7_0": true,
  "v7_1": true,
  "v8_0": true,
  "v8_1": true,
  "v9_0": true
}
```





