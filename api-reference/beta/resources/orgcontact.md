---
title: orgContact リソースの種類
description: 以下は、リソースの JSON 表記です
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 01f606e8fb1f6ae51608853eed3bc39e0ec124df
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29643532"
---
# <a name="orgcontact-resource-type"></a>orgContact リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="methods"></a>メソッド

| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[OrgContact を取得します。](../api/orgcontact-get.md) | [orgContact](orgcontact.md) |OrgContact オブジェクトのプロパティと関係を参照してください。|
|[マネージャーを取得します。](../api/orgcontact-get-manager.md) |[directoryObject](directoryobject.md)| 連絡先のマネージャーを取得します。|
|[List directReports](../api/orgcontact-list-directreports.md) |[directoryObject](directoryobject.md) collection| 連絡先の直属の部下の一覧を表示します。|
|[memberOf を一覧表示する](../api/orgcontact-list-memberof.md) |[directoryObject](directoryobject.md) コレクション| MemberOf オブジェクトのコレクションを取得します。|
|[削除する](../api/orgcontact-delete.md) | なし |OrgContact オブジェクトを削除します。 |
|[checkMemberGroups](../api/orgcontact-checkmembergroups.md)|String コレクション| グループのメンバーシップを確認します。 |
|[getMemberGroups](../api/orgcontact-getmembergroups.md)|String コレクション| メンバーである、指定した連絡先のすべてのグループを返します。 |
|[getMemberObjects](../api/orgcontact-getmemberobjects.md)|String コレクション| DirectoryObjects のメンバーである連絡先の一覧を返します。 |

## <a name="properties"></a>プロパティ

| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
| アドレス                    | [physicalOfficeAddress](physicalofficeaddress.md)            | この組織の連絡先の郵送先住所です。 ここでは、取引先担当者は、1 つの物理アドレスにだけ配置できます。 |
| companyName                  | String                                                    | この組織の連絡先が所属する会社の名前です。                                                                                                                                                                                                                                                                                                                 |
| department                   | String                                                     | 窓口担当者の部署の名前です。                                                                                                                                                                                                                                                                                                                                |
| displayName                  | String                                                     | この組織の連絡先の名前を表示します。                                                                                                                                                                                                                                                                                                                                   |
| givenName                    | String                                                     | この組織の連絡先の名です。                                                                                                                                                                                                                                                                                                                                     |
| id                           | String                                                     | この組織の連絡先の一意の識別子です。                                                                                                                                                                                                                                                                                                                             |
| imAddresses                  | String コレクション                          | この組織の連絡先の IM アドレス] ボックスの一覧です。 ここでは、取引先担当者はのみ 1 つの SIP アドレスを持つことができます。                                                                                                                                                                                                                        |
| jobTitle                     | String                                                     | この組織の連絡先の役職です。                                                                                                                                                                                                                                                                                                                                      |
|mail|String| "Jeff@contoso.onmicrosoft.com"など、連絡先の SMTP アドレスです。 |
| mailNickname                 | String                                                     | 電子メール エイリアス (電子メール アドレスの前に保留中の部分、@ 記号) この組織の連絡先の。                                                                                                                                                                                                                                                                                |
| onPremisesLastSyncDateTime   | DateTimeOffset                                             | 日付と時刻がこの組織のメンバーが前回との同期、オンプレミス AD。 Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。 たとえば、2014 年 1 月 1 日に UTC 午前 0 時が、これのようになります。: ' 2014-01-01T00:00:00Z' です。   |
| onPremisesProvisioningErrors |[onPremisesProvisioningError](onpremisesprovisioningerror.md) コレクション       | プロビジョニング エラーがこの組織の連絡先の同期の一覧です。                                                                                                                                                                                                                                                                                                |
|onPremisesSyncEnabled|Boolean|**true の**場合は、オンプレミス ディレクトリからは、このオブジェクトを同期してください。**false**場合は、このオブジェクトがもともと設置ディレクトリからの同期が不要になった同期され、Exchange にもう**null**の場合は、オンプレミス ディレクトリ (既定値) からこのオブジェクトが同期されていません。|
| phones                       | [phone](phone.md) コレクション                            | この組織の連絡先の電話のリストです。 電話の種類は、モバイル、ビジネス、および businessFax にあります。 各タイプの 1 つだけというものは、コレクション内に存在します。                                                                                                                       |
| proxyAddresses               | String コレクション                                         | たとえば: ["SMTP: bob@contoso.com"、"smtp: bob@sales.contoso.com"]。 複数値プロパティのフィルター式には **any** 演算子が必要です。 サポートしています\$フィルターです。                                                                                                                                                                               |
| surname                      | String                                                     | この組織の連絡先の姓を入力します。                          |

## <a name="relationships"></a>リレーションシップ

| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|directReports|[directoryObject](directoryobject.md) collection| 連絡先の直属の部下。 (、ユーザーおよび連絡先のマネージャー プロパティが設定された連絡先にします。) 読み取り専用です。 Null 許容型。|
|manager|[directoryObject](directoryobject.md)| ユーザーまたは連絡先は、この連絡先のマネージャーです。 読み取り専用です。|
|memberOf|[directoryObject](directoryobject.md) コレクション| メンバーである連絡先のグループです。 読み取り専用です。 Null 許容型。|

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
  "suppressions": [
    "Error: /api-reference/beta/resources/orgcontact.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
