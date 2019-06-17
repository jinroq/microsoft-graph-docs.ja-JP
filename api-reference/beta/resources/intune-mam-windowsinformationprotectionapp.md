---
title: windowsInformationProtectionApp リソースの種類
description: Windows 情報保護用アプリ
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a4b5858a09a775b28d12c258bcdca82dc302f813
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994539"
---
# <a name="windowsinformationprotectionapp-resource-type"></a>windowsInformationProtectionApp リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 情報保護用アプリ

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列|アプリの表示名。|
|description|String|アプリの説明。|
|publisherName|String|発行元名|
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





