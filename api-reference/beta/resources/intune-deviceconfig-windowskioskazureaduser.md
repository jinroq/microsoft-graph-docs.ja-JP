---
title: windowsKioskAzureADUser リソースの種類
description: キオスクの構成の AzureAD ユーザー アカウントの識別に使用するクラス
author: tfitzmac
ms.openlocfilehash: e4048b4cbea592af350af20bf433ca00ac6d4980
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330073"
---
# <a name="windowskioskazureaduser-resource-type"></a>windowsKioskAzureADUser リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

キオスクの構成の AzureAD ユーザー アカウントの識別に使用するクラス

[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。

## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|userId|String|この構成にキオスクがロックアウトされている AzureAD のユーザーの ID|
|userPrincipalName|String|この構成にキオスクがロックアウトされているユーザー アカウント|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADUser",
  "userId": "String",
  "userPrincipalName": "String"
}
```





