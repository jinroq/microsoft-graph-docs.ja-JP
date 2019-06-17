---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされていない理由の説明。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce838f73c4ad02ecb29d540a9f0d4af065796993
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978970"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>unsupportedDeviceConfigurationDetail リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティがサポートされていない理由の説明。

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|メッセージ​​|String|エンティティがサポートされていない理由を説明するメッセージ。|
|propertyName|String|メッセージが元のエンティティの特定のプロパティに関連付けられている場合は、そのプロパティの名前。|

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





