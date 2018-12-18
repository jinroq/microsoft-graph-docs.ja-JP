---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: tfitzmac
ms.openlocfilehash: 6ad47301dc7ec9650026021a2131d34b4d704e70
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334385"
---
# <a name="windowsinformationprotectionapp-resource-type"></a>windowsInformationProtectionApp リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

Windows 情報保護用アプリ
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|displayName|文字列型 (String)|アプリの表示名。|
|説明|文字列型 (String)|アプリの説明。|
|publisherName|文字列型 (String)|発行元名|
|productName|文字列型 (String)|製品名。|
|denied|ブール型 (Boolean)|true の場合、アプリは拒否された保護または除外です。|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```





