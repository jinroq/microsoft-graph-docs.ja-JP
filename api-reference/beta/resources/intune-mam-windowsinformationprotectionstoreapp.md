---
title: windowsInformationProtectionStoreApp リソースの種類
description: Windows 情報保護のストア アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: fa2059f7e85c180d4ff091a4596267471d772e3d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986615"
---
# <a name="windowsinformationprotectionstoreapp-resource-type"></a>windowsInformationProtectionStoreApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 情報保護のストア アプリ

[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列型 (String)|アプリの表示名。 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承|
|説明|文字列型 (String)|アプリの説明。 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承|
|publisherName|文字列型 (String)|[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名|
|productName|文字列型 (String)|製品名。 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承|
|denied|ブール型 (Boolean)|true の場合、アプリは拒否された保護または除外です。 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionStoreApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionStoreApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```





