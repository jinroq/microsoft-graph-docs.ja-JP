---
title: onPremisesPublishing リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: fd216d52ba212e739f1d7c087a99a4379682010e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568866"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|customdomaincertificate|String|カスタムドメインが使用されているときに、アプリケーションに関連付けられている証明書の詳細。 既定のドメインを使用する場合は Null。|
|externalauthenticationtype|String|詳細アプリケーションの事前認証設定の可能な値は`passthru`、、 `aadPreAuthentication`です。|
|externalUrl|String|アプリケーションの公開された外部 url。 例えばhttps://intranet-contoso.msappproxy.net/  |
|internalUrl|String|アプリケーションの内部 url。 例えばhttps://intranet/ |
|isonprem発行が有効|Boolean|アプリケーションが現在公開されているかどうかを示します。|
|applicationservertimeout|String|この時間が経過すると、コネクタは、接続を閉じる前にバックエンドアプリケーションからの応答を待機します。 可能な値`default`は`long`、です。 サーバー `long`が要求に応答するのに60-75 秒以上かかる場合に使用します。 また、 `long`アプリケーションにアクセスできず、エラー状態が "バックエンドタイムアウト" になっているかどうかを試してみてください。|
|isTranslateHostHeaderEnabled|Boolean|アプリケーションが応答ヘッダー内の url を変換する必要があるかどうかを示します。 これには、cookie の正しいサイトの設定が含まれます。|

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
