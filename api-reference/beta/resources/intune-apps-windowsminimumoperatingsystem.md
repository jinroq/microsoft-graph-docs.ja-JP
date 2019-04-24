---
title: windowsMinimumOperatingSystem リソースの種類
description: Windows モバイル アプリに必要な最小オペレーティング システム。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c20bdf575041e28e348f050f7bad4688f76e1398
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32463888"
---
# <a name="windowsminimumoperatingsystem-resource-type"></a>windowsMinimumOperatingSystem リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

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

## <a name="relationships"></a>リレーションシップ
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





