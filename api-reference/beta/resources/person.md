---
title: person リソースの種類
description: メール、連絡先、ソーシャル ネットワークの間でのユーザーに関する情報を集計します。 ユーザーは、個人用の連絡先、ソーシャル ネットワー キングの連絡先、組織のディレクトリ、およびユーザーの最新の通信 (電子メール、Skype など) を使用できます。
author: simonhult
localization_priority: Normal
ms.openlocfilehash: c0318986b01704501a2b7910888d6a5e962a5dca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865381"
---
# <a name="person-resource-type"></a>person リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

メール、連絡先、ソーシャル ネットワークの間でのユーザーに関する情報を集計します。 ユーザーは、個人用の連絡先、ソーシャル ネットワー キングの連絡先、組織のディレクトリ、およびユーザーの最新の通信 (電子メール、Skype など) を使用できます。

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:---------------|:--------|:----------|
|[ユーザーを一覧表示する](../api/user-list-people.md) | **人物** |[ユーザー](../resources/user.md)への関連性によって順序付けられた person オブジェクトの集合を取得します。|

## <a name="properties"></a>プロパティ

| プロパティ | 種類 | 説明 |
|:---------------|:--------|:----------|
|birthday|文字列|人物の誕生日。|
|companyName|文字列|人物の会社名。|
|department|文字列|人物の部署。|
|displayName|string|人物の表示名。|
|emailAddresses|[rankedEmailAddress](rankedemailaddress.md)コレクション|人物の電子メール アドレス。|
|givenName|文字列|人物に指定された名前。|
|ID|文字列|人物の一意の識別子。読み取り専用です。|
|isFavorite|ブール|ユーザーがこの人物をお気に入りとしてフラグを設定した場合は `true`。|
|mailboxType|文字列|相手の電子メール アドレスで表されるメールボックスの種類です。|
|officeLocation|文字列|人物のオフィスの所在地。|
|personNotes|文字列|ユーザーがこの人物について記入した自由形式のメモ。|
|personType|文字列|配布リストなど、ユーザーの種類。|
|phones|[phone](phone.md) コレクション|人物の電話番号。|
|postalAddresses|[location](location.md) コレクション|人物のアドレス。|
|profession|文字列|人物の職業。|
|ソース|[personDataSource](persondatasource.md)コレクション|ソース ユーザー データからのもの、たとえば、ディレクトリ、または Outlook の連絡先です。|
|surname|文字列|人物の姓。|
|タイトル|文字列|人のタイトルです。|
|userPrincipalName|文字列|人物のユーザー プリンシパル名 (UPN)。UPN は、インターネット標準 [RFC 822](https://www.ietf.org/rfc/rfc0822.txt) に基づいた、個人のインターネット スタイルのログイン名です。規則では、これは個人の電子メール名にマップされる必要があります。一般的な書式は alias@domain になります。|
|websites|[website](website.md) コレクション|人物の Web サイト。|
|yomiCompany|文字列|人物の会社の日本名の読み仮名。|

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
<!-- {
  "type": "#page.annotation",
  "description": "person resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
