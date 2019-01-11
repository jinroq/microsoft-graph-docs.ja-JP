---
title: onPremisesPublishing リソースの種類
description: 以下は、リソースの JSON 表記です。
localization_priority: Normal
ms.openlocfilehash: 30ff6908a42a690e07d71b5d0c62fcb22dea3c34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842540"
---
# <a name="onpremisespublishing-resource-type"></a>onPremisesPublishing リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

## <a name="properties"></a>プロパティ
| プロパティ     | 種類   |説明|
|:---------------|:--------|:----------|
|customDomainCertificate|String|カスタムのドメインが使用しているときに、アプリケーションに関連付けられている証明書の詳細です。 既定のドメインを使用する場合は null にします。|
|externalAuthenticationType|String|アプリケーションの使用可能な値は、事前認証の設定の詳細: `passthru`、 `aadPreAuthentication`。|
|externalUrl|String|アプリケーションの公開済みの外部 url です。 例えばhttps://intranet-contoso.msappproxy.net/  |
|internalUrl|String|アプリケーションの内部の url です。 例えばhttps://intranet/ |
|isOnPremPublishingEnabled|ブール型|アプリケーションをか現在発行されているかどうかを示します。|
|applicationServerTimeout|String|コネクタが接続を閉じる前に、バックエンド アプリケーションからの応答を待機する期間。 使用可能な値は、 `default`、 `long`。 使用`long`場合、サーバーは要求に応答するのには 60 ~ 75 秒以上です。 `long`アプリケーションにアクセスできないし、エラー ・ ステータスは、「バックエンド ・ タイムアウト」です。|
|isTranslateHostHeaderEnabled|ブール型|アプリケーションが応答ヘッダー内の url を変換する必要があるかどうかを示します。 これには、適切なサイトの cookie の設定が含まれます。|

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
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesPublishing resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
