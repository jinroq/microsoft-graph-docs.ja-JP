---
title: managedDeviceModelsAndManufacturers リソースの種類
description: アカウントの管理対象デバイスのモデルと製造 meatadata
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 99291829bfa672a9ade85a0a015061e4f6ec8e10
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522105"
---
# <a name="manageddevicemodelsandmanufacturers-resource-type"></a>managedDeviceModelsAndManufacturers リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アカウントの管理対象デバイスのモデルと製造 meatadata

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|devicemodels|String collection|アカウント内の管理されたデバイスのモデルの一覧|
|deviceManufacturers|String collection|アカウントで管理されているデバイスの製造元の一覧|

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





