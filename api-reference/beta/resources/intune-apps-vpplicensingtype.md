---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2f4966b6608bcd96720c4260191388979e811061
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31796466"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|supportuserlicensing|Boolean|プログラムがユーザー ライセンスの種類をサポートするかどうか。|
|supportdevicelicenel|ブール型 (Boolean)|プログラムがデバイス ライセンスの種類をサポートするかどうか。|
|supportsUserLicensing|Boolean|プログラムがユーザー ライセンスの種類をサポートするかどうか。|
|supportsDeviceLicensing|ブール型 (Boolean)|プログラムがデバイス ライセンスの種類をサポートするかどうか。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportUserLicensing": true,
  "supportDeviceLicensing": true,
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```





