---
title: windowsMinimumOperatingSystem リソースの種類
description: Windows モバイル アプリに必要な最小オペレーティング システム。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2620ac5de3f2aa098a2fc6f5e380e74a99ce42b9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949810"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows モバイル アプリに必要な最小オペレーティング システム。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|v8_0|Boolean|Windows バージョン 8.0 以降。|
|v8_1|ブール型 (Boolean)|Windows バージョン 8.1 以降。|
|v10_0|ブール型 (Boolean)|Windows バージョン 10.0 以降。|
|v10_1607|Boolean|Windows 10 1607 以降。|
|v10_1703|Boolean|Windows 10 1703 以降。|
|v10_1709|Boolean|Windows 10 1709 以降。|
|v10_1803|Boolean|Windows 10 1803 以降。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsMinimumOperatingSystem",
  "v8_0": true,
  "v8_1": true,
  "v10_0": true,
  "v10_1607": true,
  "v10_1703": true,
  "v10_1709": true,
  "v10_1803": true
}
```




