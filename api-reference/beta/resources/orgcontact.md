---
title: orgcontact リソースの種類
description: 以下は、リソースの JSON 表記です
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d0b5daa4f674762eb7733086678dd08d1389d2c7
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341830"
---
# <a name="orgcontact-resource-type"></a>orgcontact リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[orgcontact の取得](../api/orgcontact-get.md) | [orgcontact へ](orgcontact.md) |orgcontact オブジェクトのプロパティと関係を読み取ります。|
|[マネージャーを取得する](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| 連絡先の上司を取得します。|
|[List directReports](../api/orgcontact-list-directreports.md) |[directoryObject](directoryobject.md) collection| 連絡先の直属の部下を一覧表示します。|
|[List memberOf](../api/orgcontact-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| memberOf オブジェクトのコレクションを取得します。|
|[削除](../api/orgcontact-delete.md) | なし |orgcontact オブジェクトを削除します。 |
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|String collection| グループのメンバーシップを確認します。 |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|String コレクション| 指定した連絡先がメンバーであるすべてのグループを取得します。 |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|String collection| 連絡先がメンバーである directoryobjects の一覧を返します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| 解決                    | [physicalOfficeAddress](physicalofficeaddress.md)コレクション           | この組織の連絡先の住所。 現時点では、連絡先には1つの物理的な住所しかありません。 |
| companyName                  | String                                                    | この組織の連絡先が所属する会社の名前。                                                                                                                                                                                                                                                                                                                 |
| department                   | String                                                     | 連絡先が機能する部署の名前。                                                                                                                                                                                                                                                                                                                                |
| displayName                  | 文字列                                                     | この組織の連絡先の表示名。                                                                                                                                                                                                                                                                                                                                   |
| givenName                    | String                                                     | この組織の連絡先の最初の名前。                                                                                                                                                                                                                                                                                                                                     |
| id                           | 文字列型 (String)                                                     | この組織の連絡先の一意の識別子。                                                                                                                                                                                                                                                                                                                             |
| jobTitle                     | 文字列                                                     | この組織の連絡先の役職。                                                                                                                                                                                                                                                                                                                                      |
|mail|String| 連絡先の SMTP アドレス (例: "jeff@contoso.onmicrosoft.com")。 |
| mailNickname                 | String                                                     | この組織の連絡先の電子メールエイリアス (電子メールアドレスの保留中の @ 記号の前にある部分)。                                                                                                                                                                                                                                                                                |
| onPremisesLastSyncDateTime   | DateTimeOffset                                             | この組織の連絡先が、オンプレミスの AD から最後に同期された日時。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表します。これは常に UTC 時間です。 たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、'2014-01-01T00:00:00Z'.のようになります。   |
| onPremisesProvisioningErrors |[onPremisesProvisioningError](onpremisesprovisioningerror.md) コレクション       | この組織の連絡先の同期プロビジョニングエラーの一覧。                                                                                                                                                                                                                                                                                                |
|onPremisesSyncEnabled|Boolean|このオブジェクトがオンプレミスのディレクトリから同期されている場合は**true** 。このオブジェクトがオンプレミスのディレクトリから最初に同期されていて、同期されておらず Exchange にある場合は、 **false**になります。このオブジェクトがオンプレミスのディレクトリから同期されたことがない場合は**null** (既定値)。|
| phones                       | [phone](phone.md) コレクション                            | この組織の連絡先の電話のリスト。 電話の種類は、mobile、business、および businessfax にすることができます。 コレクションには、それぞれの種類のうち1つだけ存在できます。                                                                                                                       |
| proxyAddresses               | String collection                                         | 例: "smtp: bob@contoso.com", "smtp: bob@sales.contoso.com"。 複数値プロパティのフィルター式には **any** 演算子が必要です。 フィルター \$をサポートします。                                                                                                                                                                               |
| surname                      | String                                                     | この組織の連絡先の姓。                          |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|directReports|[directoryObject](directoryobject.md) collection| 連絡先の直属の部下。 (上司プロパティがこの連絡先に設定されているユーザーと連絡先) 読み取り専用です。 Null 許容型。|
|manager|[directoryObject](directoryobject.md)| この連絡先の上司であるユーザーまたは連絡先。 読み取り専用です。|
|memberOf|[directoryObject](directoryobject.md) collection| この連絡先がメンバーになっているグループ。 読み取り専用です。 Null 許容型。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "directReports",
    "manager",
    "memberOf"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",  
  "@odata.type": "microsoft.graph.orgcontact"
}-->

```json
{
  "addresses": [{"@odata.type": "microsoft.graph.physicalOfficeAddress"}],
  "companyName": "string",
  "department": "string",
  "displayName": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "jobTitle": "string",
  "mail": "string",
  "mailNickname": "string",
  "onPremisesLastSyncDateTime": "string (timestamp)",
  "onPremisesProvisioningErrors": [{"@odata.type": "microsoft.graph.onPremisesProvisioningError"}],
  "onPremisesSyncEnabled": true,
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "proxyAddresses": ["string"],
  "surname": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "orgContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
