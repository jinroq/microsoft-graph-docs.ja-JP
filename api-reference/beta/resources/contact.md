---
title: contact リソース型
description: 連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d2bdc1be9e504bc72ce12ffe924b6da0812b99ce
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535481"
---
# <a name="contact-resource-type"></a>contact リソース型

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

連絡先は、連絡を取り合う人や組織に関する情報を編成および保存できる Outlook のアイテムです。連絡先は連絡先フォルダーに格納されます。

このリソースは以下をサポートしています。

- [拡張機能](/graph/extensibility-overview)として、カスタム プロパティに独自のデータを追加します。
- [変更通知](/graph/webhooks)を受信します。
- [デルタ](../api/contact-delta.md)関数を提供することにより、[デルタ クエリ](/graph/delta-query-overview)を使用して、増分の追加、削除、更新を追跡します。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.typedEmailAddress"}],
  "fileAs": "string",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "gender": "string",
  "generation": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "nickName": "string",
  "officeLocation": "string",
  "parentFolderId": "string",
  "personalNotes": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.physicalAddress"}],
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "weddingAnniversary": "date",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string"
}

```
## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|assistantName|String|連絡先のアシスタントの名前。|
|birthday|DateTimeOffset|連絡先の誕生日です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|categories|String collection|連絡先に関連付けられたカテゴリ。 各カテゴリは、ユーザーに対して定義されている [outlookCategory](outlookcategory.md) の **displayName** プロパティに対応しています。|
|changeKey|String|連絡先のバージョンを識別します。連絡先を変更するたびに ChangeKey も変更されます。これにより、Exchange は正しいバージョンのオブジェクトに変更を適用できます。|
|children|String collection|連絡先の子供の名前。|
|companyName|String|連絡先の会社の名前。|
|createdDateTime|DateTimeOffset|連絡先が作成された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|department|String|連絡先の部署。|
|displayName|文字列型 (String)|連絡先の表示名。 表示名は、[作成](../api/user-post-contacts.md)操作または[更新](../api/contact-update.md)操作で指定できます。 後で他のプロパティを更新すると、自動的に生成された値が、指定した displayName 値に上書きされる可能性があることに注意してください。 既存の値を保持するには、[更新](../api/contact-update.md)操作で常に displayName として含めます。|
|emailAddresses|[typedEmailAddress](typedemailaddress.md)コレクション|連絡先のメール アドレス。|
|fileAs|String|連絡先がファイルされる名前。|
|flag|[followUpFlag](followupflag.md)|連絡先の状態、開始日、期限、または終了日を示すフラグ値。 |
|gender |String |連絡先の性別。 |
|generation|String|連絡先の世代。|
|givenName|String|連絡先の名。|
|id|String|連絡先の一意識別子。読み取り専用。|
|imAddresses|String collection|連絡先のインスタント メッセージング (IM) アドレス。|
|initials|String|連絡先のイニシャル。|
|jobTitle|String|連絡先の役職。|
|lastModifiedDateTime|DateTimeOffset|連絡先が変更された時刻です。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`|
|manager|String|連絡先の上司の名前。
|middleName|String|連絡先のミドル ネーム。|
|nickName|String|連絡先のニックネーム。|
|officeLocation|String|連絡先のオフィスの所在地。|
|parentFolderId|String|連絡先の親フォルダーの ID。|
|personalNotes|String|連絡先に関するユーザーのメモ。|
|phones |[phone](phone.md) コレクション |自宅電話、携帯電話、勤務先電話など、連絡先に関連付けられた電話番号。 |
|postalAddresses |[physicalAddress](physicaladdress.md)コレクション |自宅住所や勤務先住所など、連絡先に関連付けられた住所。 |
|profession|String|連絡先の専門的職業。|
|spouseName|String|連絡先の配偶者/パートナーの名前。|
|surname|String|連絡先の姓。|
|title|String|連絡先の肩書。|
|websites |[website](website.md) コレクション|連絡先に関連付けられた Web サイト。 |
|weddinganniversary 日 |日付 |連絡先の結婚記念日。 |
|yomiCompanyName|String|連絡先の会社名の読み仮名。|
|yomiGivenName|String|連絡先の名 (ファースト ネーム) の読み仮名。|
|yomiSurname|文字列|連絡先の姓 (ラスト ネーム) の読み仮名。|

## <a name="relationships"></a>リレーションシップ
| リレーションシップ | 型   |説明|
|:---------------|:--------|:----------|
|extensions|[extension](extension.md) コレクション|連絡先に対して定義されているオープン拡張機能のコレクション。 Null 許容型。|
|multiValueExtendedProperties|[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) コレクション| 連絡先に定義された、複数値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|
|写真|[photo](profilephoto.md)| 連絡先の写真 (オプション)。連絡先の写真を取得また設定することができます。|
|singleValueExtendedProperties|[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) コレクション| 連絡先に定義された、単一値の拡張プロパティのコレクション。読み取り専用。Null 許容型。|

## <a name="methods"></a>メソッド
| メソッド           | 戻り値の型    |説明|
|:---------------|:--------|:----------|
|[連絡先を取得する](../api/contact-get.md) | [連絡先](contact.md) |連絡先オブジェクトのプロパティとリレーションシップを読み取ります。|
|[作成](../api/user-post-contacts.md) | [連絡先](contact.md) |連絡先をルート連絡先フォルダーまたは別の連絡先フォルダーの連絡先エンドポイントに追加します。|
|[更新する](../api/contact-update.md) | [contact](contact.md) |連絡先オブジェクトを更新します。 |
|[削除](../api/contact-delete.md) | なし |連絡先オブジェクトを削除します。 |
|[delta](../api/contact-delta.md)|[contact](contact.md)コレクション| 指定したフォルダーで追加、削除、更新された連絡先のセットを取得します。|
|**オープン拡張機能**| | |
|[オープン拡張機能を作成する](../api/opentypeextension-post-opentypeextension.md) |[openTypeExtension](opentypeextension.md)| オープン拡張機能を作成し、新規または既存のリソースにカスタム プロパティを追加します。|
|[オープン拡張機能を取得する](../api/opentypeextension-get.md) |[openTypeExtension](opentypeextension.md) コレクション| 拡張機能の名前で識別されるオープン拡張機能を取得します。|
|**スキーマ拡張機能**| | |
|[スキーマ拡張機能の値を追加する](/graph/extensibility-schema-groups) || スキーマ拡張機能の定義を作成し、それを使用してカスタマイズされた種類のデータをリソースに追加します。|
|**拡張プロパティ**| | |
|[単一値の拡張プロパティを作成する](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[連絡先](contact.md)  |新規または既存の連絡先に、1 つ以上の単一値の拡張プロパティを作成します。   |
|[単一値の拡張プロパティを持つ連絡先を取得する](../api/singlevaluelegacyextendedproperty-get.md)  | [連絡先](contact.md) | `$expand` または `$filter` を使用して、単一値の拡張プロパティを含む連絡先を取得します。 |
|[複数値の拡張プロパティを作成する](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [連絡先](contact.md) | 新規または既存の連絡先に、1 つ以上の複数値の拡張プロパティを作成します。  |
|[複数値の拡張プロパティを持つ連絡先を取得する](../api/multivaluelegacyextendedproperty-get.md)  | [contact](contact.md) | `$expand` を使用して、複数値の拡張プロパティを含む連絡先を取得します。 |

## <a name="see-also"></a>関連項目

- [デルタ クエリを使用して、Microsoft Graph データの変更を追跡する](/graph/delta-query-overview)
- [フォルダー内のメッセージへの増分変更を取得する](/graph/delta-query-messages)
- [拡張機能を使用してカスタム データをリソースに追加する](/graph/extensibility-overview)
- [オープン拡張機能を使用してカスタム データをユーザーに追加する](/graph/extensibility-open-users)
- [スキーマ拡張機能を使用したグループへのカスタム データの追加](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contact.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
