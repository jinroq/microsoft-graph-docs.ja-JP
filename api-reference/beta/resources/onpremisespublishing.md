---
title: onPremisesPublishing リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508182"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|customDomainCertificate|String|カスタムのドメインが使用しているときに、アプリケーションに関連付けられている証明書の詳細です。 既定のドメインを使用する場合は null にします。|
|externalAuthenticationType|String|アプリケーションの使用可能な値は、事前認証の設定の詳細: `passthru`、 `aadPreAuthentication`。|
|externalUrl|String|アプリケーションの公開済みの外部 url です。 次に例を示します。  |
|internalUrl|String|アプリケーションの内部の url です。 次に例を示します。 |
|isOnPremPublishingEnabled|ブール値|アプリケーションをか現在発行されているかどうかを示します。|
|applicationServerTimeout|String|コネクタが接続を閉じる前に、バックエンド アプリケーションからの応答を待機する期間。 使用可能な値は、`default`、`long` です。 使用`long`場合、サーバーは要求に応答するのには 60 ~ 75 秒以上です。 `long`アプリケーションにアクセスできないし、エラー ・ ステータスは、「バックエンド ・ タイムアウト」です。|
|isTranslateHostHeaderEnabled|ブール値|アプリケーションが応答ヘッダー内の url を変換する必要があるかどうかを示します。 これには、適切なサイトの cookie の設定が含まれます。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesPublishing"
}-->

```json
{
  "customDomainCertificate": "String",
  "externalAuthenticationType": "String",
  "externalUrl": "String",
  "internalUrl": "String",
  "isOnPremPublishingEnabled": true,
  "applicationServerTimeout": "String",
  "isTranslateHostHeaderEnabled": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onpremisespublishing.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
