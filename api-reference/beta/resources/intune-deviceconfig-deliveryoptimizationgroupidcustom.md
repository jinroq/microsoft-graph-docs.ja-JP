---
title: deliveryOptimizationGroupIdCustom リソースの種類
description: カスタムグループ id の種類
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d4f369c9a3b62480549f19d4a7c1d7b1d0bb196
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556166"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a>deliveryOptimizationGroupIdCustom リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

カスタムグループ id の種類


[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)から継承します。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|groupidcustom|String|デバイスが属する任意のグループ ID を指定します。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```





