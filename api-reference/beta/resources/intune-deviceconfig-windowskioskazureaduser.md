---
title: windowsKioskAzureADUser リソースの種類
description: キオスクの構成の AzureAD ユーザー アカウントの識別に使用するクラス
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 57b48bcdbac3f95da37704222cded29ba61cd32d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845886"
---
# <a name="windowskioskazureaduser-resource-type"></a>windowsKioskAzureADUser リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

キオスクの構成の AzureAD ユーザー アカウントの識別に使用するクラス

[WindowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)から継承します。

## <a name="properties"></a>プロパティ
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





