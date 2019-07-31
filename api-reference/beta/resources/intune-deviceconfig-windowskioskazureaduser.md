---
title: windowsKioskAzureADUser リソースの種類
description: キオスク構成の AzureAD ユーザーアカウントを識別するために使用されるクラス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3dd72b65c8829f4b085d4bb8ec86c904746bf126
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36000292"
---
# <a name="windowskioskazureaduser-resource-type"></a>windowsKioskAzureADUser リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

キオスク構成の AzureAD ユーザーアカウントを識別するために使用されるクラス


[Windowskioskuser](../resources/intune-deviceconfig-windowskioskuser.md)からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|userId|String|このキオスク構成にロックされる AzureAD ユーザーの ID|
|userPrincipalName|String|このキオスク構成にロックされるユーザーアカウント|

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





