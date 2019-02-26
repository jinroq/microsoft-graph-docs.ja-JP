---
title: win32LobAppReturnCode リソースの種類
description: Win32 アプリのリターンコードプロパティを格納します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4402464bd4618f1e33b9b766be529cbe592165c0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174588"
---
# <a name="win32lobappreturncode-resource-type"></a>win32LobAppReturnCode リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Win32 アプリのリターンコードプロパティを格納します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|returnCode|Int32|コードを返します。|
|type|[win32LobAppReturnCodeType](../resources/intune-apps-win32lobappreturncodetype.md)|戻り値のコードの種類を示します。 可能な値は、`failed`、`success`、`softReboot`、`hardReboot`、`retry` です。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppReturnCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppReturnCode",
  "returnCode": 1024,
  "type": "String"
}
```




