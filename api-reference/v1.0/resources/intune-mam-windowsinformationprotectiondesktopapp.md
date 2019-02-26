---
title: windowsInformationProtectionDesktopApp リソースの種類
description: Windows 情報保護用デスクトップ アプリ
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e83ad9e3e500ab5276e4643055f602e763de34fd
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259984"
---
# <a name="windowsinformationprotectiondesktopapp-resource-type"></a>windowsInformationProtectionDesktopApp リソースの種類

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 情報保護用デスクトップ アプリ


[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|文字列|アプリの表示名。 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承|
|説明|文字列|アプリの説明。 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承|
|publisherName|String|[windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) から継承される発行元名|
|productName|String|製品名。 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承|
|denied|ブール型 (Boolean)|true の場合、アプリは拒否された保護または除外です。 [windowsInformationProtectionApp](../resources/intune-mam-windowsinformationprotectionapp.md) からの継承|
|binaryName|String|バイナリの名前。|
|binaryVersionLow|String|下位のバイナリ バージョン。|
|binaryVersionHigh|文字列型 (String)|上位のバイナリ バージョン。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDesktopApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDesktopApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true,
  "binaryName": "String",
  "binaryVersionLow": "String",
  "binaryVersionHigh": "String"
}
```



