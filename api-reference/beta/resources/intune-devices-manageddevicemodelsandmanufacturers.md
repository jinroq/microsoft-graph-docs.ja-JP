---
title: managedDeviceModelsAndManufacturers リソースの種類
description: モデルと、アカウントで管理されているデバイスのメーカーの meatadata
author: tfitzmac
ms.openlocfilehash: 42611b0c14aa583d2871d97b66ce116a0b835268
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352935"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>managedDeviceModelsAndManufacturers リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

モデルと、アカウントで管理されているデバイスのメーカーの meatadata
## <a name="properties"></a>Properties
|プロパティ|種類|説明|
|:---|:---|:---|
|deviceModels|String コレクション|アカウントで管理されているデバイスのモデルの一覧|
|deviceManufacturers|String コレクション|アカウントで管理されているデバイスの製造元の一覧|

## <a name="relationships"></a>リレーションシップ
なし
## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedDeviceModelsAndManufacturers"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceModelsAndManufacturers",
  "deviceModels": [
    "String"
  ],
  "deviceManufacturers": [
    "String"
  ]
}
```





