---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされている理由の説明です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6b82dcf28652cbe54a4932a641579101cb392639
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27949774"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>unsupportedDeviceConfigurationDetail リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

エンティティがサポートされている理由の説明です。
## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
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





