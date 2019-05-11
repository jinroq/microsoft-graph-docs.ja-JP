---
title: macOSKernelExtension リソースの種類
description: 特定の macOS カーネル拡張情報を表します。 MacOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b75288befb0f8ba7101d88d5b6f0767174469ac3
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946193"
---
# <a name="macoskernelextension-resource-type"></a>macOSKernelExtension リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定の macOS カーネル拡張情報を表します。 MacOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|teamIdentifier|String|カーネル拡張機能の署名に使用されたチーム識別子。|
|bundleId|String|カーネル拡張機能のバンドル ID。|

## <a name="relationships"></a>関係
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSKernelExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSKernelExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```




