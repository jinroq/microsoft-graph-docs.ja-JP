---
title: windows10AssociatedApps リソースの種類
description: Windows 10 関連付けられたアプリケーション定義します。
author: tfitzmac
ms.openlocfilehash: a990d3b1f9b2b33a1e98fd30f5dea4da7fbf4ae8
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344829"
---
# <a name="windows10associatedapps-resource-type"></a>windows10AssociatedApps リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 10 関連付けられたアプリケーション定義します。
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|appType|[windows10AppType](../resources/intune-deviceconfig-windows10apptype.md)|アプリケーションの種類。 使用可能な値は、`desktop`、`universal` です。|
|識別子|String|識別子です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```





