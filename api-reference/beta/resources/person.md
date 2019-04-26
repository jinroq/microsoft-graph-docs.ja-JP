---
title: person リソースの種類
description: メール、連絡先、ソーシャルネットワークにわたる個人に関する情報の集約。 ユーザーは、ローカルの連絡先、ソーシャルネットワーキングからの連絡先、組織のディレクトリ、および最近のコミュニケーション (電子メールや Skype など) の人物であることができます。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 0def5d62dd941122858ffa61bf224a9ef672ad0c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344925"
---
# <a name="person-resource-type"></a>person リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

メール、連絡先、ソーシャルネットワークにわたる個人に関する情報の集約。 ユーザーは、ローカルの連絡先、ソーシャルネットワーキングからの連絡先、組織のディレクトリ、および最近のコミュニケーション (電子メールや Skype など) の人物であることができます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[ユーザーを一覧表示する](../api/user-list-people.md) | **人物** |[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------------|:--------|:----------|
|birthday|string|人物の誕生日。|
|companyName|string|人物の会社名。|
|department|string|人物の部署。|
|displayName|string|人物の表示名。|
|emailAddresses|[rankedemailaddress](rankedemailaddress.md)コレクション|人物の電子メール アドレス。|
|givenName|string|人物に指定された名前。|
|id|string|人物の一意の識別子。読み取り専用です。|
|isFavorite|boolean|ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。|
|mailboxType|string|ユーザーの電子メールアドレスによって表されるメールボックスの種類。|
|officeLocation|string|人物のオフィスの所在地。|
|personNotes|string|ユーザーがこの人物について記入した自由形式のメモ。|
|personType|string|ユーザーの種類 (例: 配布リスト)。|
|phones|[phone](phone.md) コレクション|人物の電話番号。|
|postalAddresses|[location](location.md) コレクション|人物のアドレス。|
|profession|string|人物の職業。|
|sources|[個人データソース](persondatasource.md)コレクション|ユーザーデータの取得元となるソース (ディレクトリまたは Outlook 連絡先など)。|
|surname|string|人物の姓。|
|title|string|個人の役職。|
|userPrincipalName|string|人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。|
|websites|[website](website.md) コレクション|人物の Web サイト。|
|yomiCompany|string|人物の会社の日本名の読み仮名。|

## <a name="relationships"></a>リレーションシップ

なし

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.person"
}-->

```json
{
  "birthday": "string",
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.rankedEmailAddress"}],
  "givenName": "string",
  "id": "string (identifier)",
  "isFavorite": true,
  "mailboxType": "string",
  "officeLocation": "string",
  "personNotes": "string",
  "personType": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.location"}],
  "profession": "string",
  "sources": [{"@odata.type": "microsoft.graph.personDataSource"}],
  "surname": "string",
  "title": "string",
  "userPrincipalName": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "yomiCompany": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
