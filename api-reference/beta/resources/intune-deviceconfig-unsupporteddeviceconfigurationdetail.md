---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされている理由の説明です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c03bdb20fc4c48fa7820e09b9212bf73250599aa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400390"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>unsupportedDeviceConfigurationDetail リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティがサポートされている理由の説明です。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|message|String|エンティティがサポートされている理由を説明するメッセージ。|
|プロパティ名|String|メッセージが元のエンティティでは、そのプロパティの名前に特定のプロパティに関連しています。|

## <a name="relationships"></a>リレーションシップ
なし

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```




