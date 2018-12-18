---
title: unsupportedDeviceConfigurationDetail リソースの種類
description: エンティティがサポートされている理由の説明です。
author: tfitzmac
ms.openlocfilehash: 4cccf49366a803e5f964605a4dc4ba7f56707823
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344052"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a>unsupportedDeviceConfigurationDetail リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

エンティティがサポートされている理由の説明です。
## <a name="properties"></a>Properties
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





