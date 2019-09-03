---
title: certificateAuthority リソースの種類
description: 証明機関を表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bf88364ffd8f06783ef98ac32276d948fc6b1791
ms.sourcegitcommit: 23aa2941cfb8bd744d8d59e8bba9d2c5f57f8e29
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/29/2019
ms.locfileid: "36667665"
---
# <a name="certificateauthority-resource-type"></a>certificateAuthority リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

証明機関を表します。

## <a name="properties"></a>プロパティ

| プロパティ     | 型        | 説明 |
|:-------------|:------------|:------------|
|certificate|バイナリ型 (Binary)|必須です。 公開証明書を表す base64 でエンコードされた文字列。|
|certificateRevocationListUrl|String|証明書失効リストの URL。|
|deltaCertificateRevocationListUrl|String|完全な証明書の revocaton リストが前回作成されてからの、失効したすべての証明書の一覧が含まれている URL。|
|isRootAuthority|Boolean|必須です。 信頼された証明書がルート証明機関の場合は**true** 、信頼できる証明書が中間証明機関の場合は**false** 。|
|会社|String|証明書の値から計算された**** 証明書の発行者。 読み取り専用です。 |
|issuerSki|String|証明書の値から計算された、証明**** 書のサブジェクトキー識別子。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.certificateAuthority",
  "baseType": null
}-->

```json
{
  "certificate": "Binary",
  "certificateRevocationListUrl": "String",
  "deltaCertificateRevocationListUrl": "String",
  "isRootAuthority": true,
  "issuer": "String",
  "issuerSki": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "certificateAuthority resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->