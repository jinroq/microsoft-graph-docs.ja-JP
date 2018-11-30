---
title: win32LobAppReturnCode リソースの種類
description: Win32 アプリケーションのプロパティ戻り値のコードにはが含まれています
ms.openlocfilehash: 5f32e7e5953ade1036c49ac2fb45555fd353fa1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068293"
---
# <a name="win32lobappreturncode-resource-type"></a>win32LobAppReturnCode リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Win32 アプリケーションのプロパティ戻り値のコードにはが含まれています
## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|リターン コード|Int32|コードを返します。|
|type|[win32LobAppReturnCodeType](../resources/intune-apps-win32lobappreturncodetype.md)|コードの戻り値の型。 可能な値は、`failed`、`success`、`softReboot`、`hardReboot`、`retry` です。|

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





