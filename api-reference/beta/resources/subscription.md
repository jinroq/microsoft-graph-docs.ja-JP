---
title: Subscription リソースタイプ
description: サブスクリプションは、Microsoft Graph でデータへの変更に関する通知を受信するクライアント アプリケーションを許可します。 現時点では、サブスクリプションが有効になって次のリソース。
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 265ea807330f833edf0d7b1f6a640e0a1f6f4634
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517268"
---
# <a name="subscription-resource-type"></a>Subscription リソースタイプ

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

サブスクリプションは、Microsoft Graph でデータへの変更に関する通知を受信するクライアント アプリケーションを許可します。 現時点では、サブスクリプションが有効になって次のリソース。

- Outlook からのメール、イベント、および連絡先
- Office グループからの会話。
- OneDrive からドライブ ルート項目
- ユーザーと Azure Active Directory のグループ。
- Graph セキュリティ API から通知されます。

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
| changeType | string | 必須。 登録しているリソース内の、通知を上げる変更の種類を示します。 サポートされている値は `created`、`updated`、`deleted` です。 コンマ区切りのリストを使用して複数値を結合できます。 <br><br>メモ: ドライブのルート アイテムの通知だけをサポートして、 `updated` changeType です。 ユーザーとグループの通知をサポートして`updated`と`deleted`changeType です。 |
| notificationUrl | string | 必須。 通知を受信するエンドポイントの URL。 この URL が、HTTPS を使用する必要がありますプロトコルです。 |
| リソース | 文字列 | 必須。 変更の監視対象となるリソースを指定します。 ベース URL が含まれていない (`https://graph.microsoft.com/beta/`)。 |
| expirationDateTime | DateTimeOffset | 必須です。 webhook サブスクリプションの有効期限が切れる日時を指定します。 時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。  サポートされているサブスクリプションの最長時間については、次の表をご覧ください。 |
| clientState | string | 省略可能。 各通知内のサービスによって送信される `clientState` プロパティの値を指定します。 最大の長さは、255 文字です。 クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。 |
| id | string | サブスクリプションの一意の識別子です。読み取り専用です。 |
| applicationId | string | サブスクリプションを作成するために使用するアプリケーションの識別子です。 読み取り専用です。 |
| creatorId | string | ユーザーまたはサブスクリプションを作成するサービス ・ プリンシパルの識別子です。 使用するアプリケーションがサブスクリプションを作成するアクセス許可を委任する場合、このフィールドは、サインイン中のユーザーの代理で、アプリケーションが呼び出されるの id を含みます。 アプリケーションは、アプリケーションのアクセス許可を使用する場合、このフィールドには、アプリケーションに対応するサービス ・ プリンシパルの id が含まれています。 読み取り専用です。 |

## <a name="maximum-length-of-subscription-per-resource-type"></a>リソースの種類別のサブスクリプションの最大の長さ

| リソース            | 最大有効期限  |
|:--------------------|:-------------------------|
| メール                | 4230 分 (3 日間で)    |
| カレンダー            | 4230 分 (3 日間で)    |
| 連絡先            | 4230 分 (3 日間で)    |
| グループ会話 | 4230 分 (3 日間で)    |
| ドライブ ルート項目    | 4230 分 (3 日間で)    |
| セキュリティの警告     | 43200 分 (30 日間で)  |

> **注:** 既存のアプリケーションと新しいアプリケーションは、サポートされている値を超える必要があります。 将来、作成するか、最大値を超えるサブスクリプションを更新するすべての要求は失敗します。

## <a name="relationships"></a>リレーションシップ

なし

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-------|:------------|:------------|
| [Create subscription](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。 |
| [Update subscription](../api/subscription-update.md) | [subscription](subscription.md) | 有効期限を更新することにより、サブスクリプションを更新します。 |
| [リストの購読](../api/subscription-list.md) | [subscription](subscription.md) | アクティブなサブスクリプションの一覧を表示します。 |
| [Get subscription](../api/subscription-get.md) | [subscription](subscription.md) | Subscription オブジェクトのプロパティと関係を参照してください。 |
| [サブスクリプションの削除](../api/subscription-delete.md) | なし | サブスクリプション オブジェクトを削除します。 |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/subscription.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
