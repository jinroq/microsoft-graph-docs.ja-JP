---
title: deviceDetail リソースの種類
description: サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが管理される Azure の AD の場合は、デバイスのブラウザーおよび OS の情報などの情報に含まれています。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 18d55e397cf6c892cd37aea930d446c630017a92
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971362"
---
# <a name="devicedetail-resource-type"></a>deviceDetail リソースの種類
サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが管理される Azure の AD の場合は、デバイスのブラウザーおよび OS の情報などの情報に含まれています。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ブラウザー|String|使用のブラウザー情報の署名に。|
|deviceId|String|署名に使用するデバイスの UniqueID を意味します。|
|displayName|String|署名に使用するデバイスの名前を参照します。|
|isCompliant|Boolean|デバイスが準拠しているかどうかどうかを示します。|
|isManaged|Boolean|か、デバイスが管理されていることを示します。|
|operatingSystem|String|OS の名前と署名に使用されるバージョンを示します。|
|trustType|String|署名付きのデバイスは、ワークプ レースに参加して、AzureAD に参加して、ドメインに参加しているかどうかに関する情報を示します。 |

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.deviceDetail"
}-->

```json
{
  "browser": "String",
  "deviceId": "String",
  "displayName": "String",
  "isCompliant": true,
  "isManaged": true,
  "operatingSystem": "String",
  "trustType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "deviceDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
