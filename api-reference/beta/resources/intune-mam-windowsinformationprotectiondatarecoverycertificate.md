---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 74c480b8117f3d8dbf0ad8208bac09b63b113906
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30156190"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a>windowsInformationProtectionDataRecoveryCertificate リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Windows 情報保護の DataRecoveryCertificate

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|subjectName|文字列型 (String)|データ回復証明書のサブジェクト名|
|説明|String|データ回復証明書の説明|
|expirationDateTime|DateTimeOffset|データ回復証明書の有効期限日時|
|certificate|バイナリ型 (Binary)|データ回復証明書|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```




