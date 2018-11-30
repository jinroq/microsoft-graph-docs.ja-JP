---
title: win32LobAppProductCodeDetection リソースの種類
description: Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています
ms.openlocfilehash: fcb9d5927ce1518a7bba2086a8578867d4fdf01a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074263"
---
# <a name="win32lobappproductcodedetection-resource-type"></a>win32LobAppProductCodeDetection リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Win32 アプリケーションを検出するために製品コードとバージョンのプロパティが含まれています

[Win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|productCode|String|Win32 基幹業務 (LoB) アプリケーションの製品コードです。|
|productVersionOperator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|製品のバージョンを検出する演算子です。 可能な値は、`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual` です。|
|productVersion|String|Win32 基幹業務 (LoB) アプリケーションの製品バージョン。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppProductCodeDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppProductCodeDetection",
  "productCode": "String",
  "productVersionOperator": "String",
  "productVersion": "String"
}
```





