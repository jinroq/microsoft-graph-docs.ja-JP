---
title: macOSKernelExtension リソースの種類
description: 特定の macOS カーネル拡張情報を表します。 macOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 04320f92045ae128ca1bf128484d2aa55f03d706
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31808954"
---
# <a name="macoskernelextension-resource-type"></a>macOSKernelExtension リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

特定の macOS カーネル拡張情報を表します。 macOS カーネル拡張機能は、そのチーム識別子とそのバンドル識別子によって記述できます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|teamidentifier|文字列|カーネル拡張機能の署名に使用されたチーム識別子。|
|bundleId|String|カーネル拡張機能のバンドル ID。|

## <a name="relationships"></a>リレーションシップ
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





