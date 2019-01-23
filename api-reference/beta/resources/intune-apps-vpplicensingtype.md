---
title: vppLicensingType リソースの種類
description: iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 42bb678077781309b9e06c339112537bc2e48bde
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399676"
---
# <a name="vpplicensingtype-resource-type"></a>vppLicensingType リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

iOS Volume-Purchase Program (VPP) ライセンスの種類のプロパティが含まれます。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|supportUserLicensing|ブール型 (Boolean)|プログラムがユーザー ライセンスの種類をサポートするかどうか。|
|supportDeviceLicensing|ブール型 (Boolean)|プログラムがデバイス ライセンスの種類をサポートするかどうか。|
|supportsUserLicensing|ブール型 (Boolean)|プログラムがユーザー ライセンスの種類をサポートするかどうか。|
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




