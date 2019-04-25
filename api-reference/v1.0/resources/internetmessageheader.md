---
title: internetMessageHeader リソースの種類
description: 'RFC5322 で定義されているように、インターネットメッセージヘッダーを表すキーと値のペア。 '
localization_priority: Normal
ms.openlocfilehash: 2a8dd616ffe8417a5064c0a98976d512b1279704
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567516"
---
# <a name="internetmessageheader-resource-type"></a>internetMessageHeader リソースの種類


[RFC5322](https://www.ietf.org/rfc/rfc5322.txt) によって定義された、インターネット メッセージ ヘッダーを表すキーと値のペア。メッセージが送信者から受信者に到達するまでに辿ったネットワーク パスの詳細を説明します。 

インターネット メッセージ ヘッダーの例については、「[View e-mail message headers (電子メールのメッセージ ヘッダーを表示する)](https://support.office.com/en-us/article/View-e-mail-message-headers-CD039382-DC6E-4264-AC74-C048563D212C#bm4)」を参照してください。


## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|name|string|キーと値のペアの、キーの部分を表します。|
|value|string|キーと値のペアの、値の部分を表します。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.internetMessageHeader"
}-->

```json
{
  "name": "string",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "internetMessageHeader resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
