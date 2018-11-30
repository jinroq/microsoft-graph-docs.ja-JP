---
title: orgContact リソースの種類
description: 以下は、リソースの JSON 表記です
ms.openlocfilehash: fb0970b2eb973e516761ba1145d66b3af7fdef5f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071988"
---
# <a name="orgcontact-resource-type"></a>orgContact リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "@odata.type": "microsoft.graph.orgcontact"
}-->

```json
{
  "businessPhones": ["string"],
  "city": "string",
  "companyName": "string",
  "country": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "mobilePhone": "string",
  "officeLocation": "string",
  "onPremisesLastSyncDateTime": "String (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "postalCode": "string",
  "proxyAddresses": ["string"],
  "state": "string",
  "streetAddress": "string",
  "surname": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|city|String| 連絡先が含まれている都市です。 |
|country|String| 連絡先が存在する国/地域。 |
|department|String| 窓口担当者の部署の名前です。 |
|onPremisesSyncEnabled|Boolean|このオブジェクトがオンプレミスのディレクトリから同期される場合は **true**。このオブジェクトが最初にオンプレミスのディレクトリから同期されていて、今後は同期されない場合は **false**。このオブジェクトがオンプレミスのディレクトリから一度も同期されたことがない場合は **null** (既定値)。|
|displayName|String| 連絡先の表示名です。 |
|givenName|String| 連絡先の指定された名前 (名)。 |
|jobTitle|String| 連絡先の役職。 |
|onPremisesLastSyncDateTime|DateTimeOffset|最後にオブジェクトが設置ディレクトリと同期された時刻を示します。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|onPremisesProvisioningErrors|[onPremisesProvisioningError](onpremisesprovisioningerror.md)コレクション| 提供処理中に同期の Microsoft 製品を使用するときのエラーです。 |
|mail|String| "Jeff@contoso.onmicrosoft.com"など、連絡先の SMTP アドレスです。 |
|mailNickname|String| 連絡先の電子メール エイリアス。 |
|mobilePhone|String| 連絡先の主な携帯電話の番号です。 |
|id|String| 連絡先の一意の識別子です。 読み取り専用。|
|officeLocation|String| ビジネスの連絡先の場所のオフィスの場所。 |
|postalCode|String| 連絡先の郵送先住所の郵便番号コード。 郵便番号のコードは、連絡先の国/地域に固有です。 アメリカ合衆国では、この属性には、ZIP コードが含まれています。 |
|proxyAddresses|String コレクション| 例: `["SMTP: bob@contoso.com", "smtp: bob@sales.contoso.com"]` **any**演算子は、複数値を持つプロパティのフィルター式に必要です。 読み取り専用。 null 許容ではありません。 $filter をサポートします。 |
|state|String| 都道府県連絡先のアドレスにします。 |
|streetAddress|String| ビジネスの連絡先の場所の住所。 |
|surname|String| ファミリの名前 (姓) の連絡先の姓。 |
|businessPhones|String| ビジネスの連絡先の場所の主な電話番号。 |

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|directReports|[directoryObject](directoryobject.md) collection| 連絡先の直属の部下。 (、ユーザーおよび連絡先のマネージャー プロパティが設定された連絡先にします。) 読み取り専用です。 Null 許容型。|
|manager|[directoryObject](directoryobject.md)| ユーザーまたは連絡先は、この連絡先のマネージャーです。 読み取り専用。|
|memberOf|[directoryObject](directoryobject.md) コレクション| メンバーである連絡先のグループです。 読み取り専用。 Null 許容型。|

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[OrgContact を取得します。](../api/orgcontact-get.md) | [orgContact](orgcontact.md) |OrgContact オブジェクトのプロパティと関係を参照してください。|
|[マネージャーを取得します。](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| 連絡先のマネージャーを取得します。|
|[List directReports](../api/orgcontact-list-directreports.md) |[directoryObject](directoryobject.md) collection| 連絡先の直属の部下の一覧を表示します。|
|[memberOf を一覧表示する](../api/orgcontact-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| MemberOf オブジェクトのコレクションを取得します。|
|[削除](../api/orgcontact-delete.md) | なし |OrgContact オブジェクトを削除します。 |
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|String コレクション| グループのメンバーシップを確認します。 |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|String コレクション| メンバーである、指定した連絡先のすべてのグループを返します。 |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|String コレクション| DirectoryObjects のメンバーである連絡先の一覧を返します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->