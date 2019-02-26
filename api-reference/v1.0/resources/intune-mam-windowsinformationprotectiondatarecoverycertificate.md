---
title: windowsInformationProtectionDataRecoveryCertificate リソースの種類
description: Windows 情報保護の DataRecoveryCertificate
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c321ea06e27e7d6fba0a35446e2b916aaf0689de
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30253653"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a>windowsInformationProtectionDataRecoveryCertificate リソースの種類

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



