---
title: deviceDetail リソースの種類
description: サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが Azure AD で管理されている場合、デバイスブラウザーや OS 情報などの情報が含まれます。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f3a0d7f141723beb5194860b025fe6fa349eb95a
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657701"
---
# <a name="devicedetail-resource-type"></a>deviceDetail リソースの種類
サインインに使用するデバイスに関連付けられているデバイスの詳細を示します。 デバイスが Azure AD で管理されている場合、デバイスブラウザーや OS 情報などの情報が含まれます。



## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|ブラウザー|String|サインインに使用するのブラウザー情報を示します。|
|deviceId|String|サインインに使用されているデバイスの UniqueID を参照します。|
|displayName|String|サインインに使用されているデバイスの名前を表します。|
|isCompliant|Boolean|デバイスが準拠しているかどうかを示します。|
|isManaged|ブール値|デバイスが管理されているかどうかを示します。|
|operatingSystem|String|サインインに使用される OS の名前とバージョンを示します。|
|trustType|文字列|サインインしているデバイスが Workplace Join、AzureAD Join、ドメイン参加しているかどうかについての情報を示します。 |

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
