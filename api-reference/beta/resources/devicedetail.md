---
title: deviceDetail リソースの種類
description: サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが管理される Azure の AD の場合は、デバイスのブラウザーおよび OS の情報などの情報に含まれています。
ms.openlocfilehash: d7c1830ee5c99fc139a937fcee3896e2a9926592
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067473"
---
# <a name="devicedetail-resource-type"></a>deviceDetail リソースの種類
サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが管理される Azure の AD の場合は、デバイスのブラウザーおよび OS の情報などの情報に含まれています。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ブラウザー|String|使用のブラウザー情報の署名に。|
|deviceId|String|署名に使用するデバイスの UniqueID を意味します。|
|displayName|String|署名に使用するデバイスの名前を参照します。|
|isCompliant|ブール値|デバイスが準拠しているかどうかどうかを示します。|
|isManaged|ブール値|か、デバイスが管理されていることを示します。|
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