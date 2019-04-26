---
title: サブスクリプション リソースの種類
description: 'サブスクリプションは、Microsoft Graph 上のデータの変更に関する通知の受信をクライアント アプリに許可します。 サブスクリプションは現在、以下のリソースで有効です:'
localization_priority: Priority
author: piotrci
ms.openlocfilehash: db3a536395f327115af69f769f37c823013ec7fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563701"
---
# <a name="subscription-resource-type"></a>サブスクリプション リソースの種類

サブスクリプションは、Microsoft Graph 上のデータの変更に関する通知の受信をクライアント アプリに許可します。 サブスクリプションは現在、以下のリソースで有効です:

- Outlook の[メッセージ][]、[イベント][]、または[連絡先][]
- Office 365 グループの[会話][]
- OneDrive for Business のルート フォルダー [driveItem][] の階層内にあるコンテンツ、またはユーザーの個人用 OneDrive のルート フォルダーまたはサブフォルダー [driveItem][] の階層内にあるコンテンツ
- Azure Active Directory 内の[ユーザー][]または[グループ][]
- Microsoft Graph Security API の[警告][]

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>プロパティ

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
| changeType | string | 必須です。 登録しているリソース内の、通知を上げる変更の種類を示します。 サポートされている値は `created`、`updated`、`deleted` です。 コンマ区切りのリストを使用して複数値を結合できます。<br><br>注: ドライブ ルート項目の通知では `updated` changeType のみがサポートされます。 ユーザーとグループの通知では、`updated` と `deleted` changeType がサポートされます。|
| notificationUrl | string | 必須です。 通知を受け取るエンドポイントの URL です。 この URL は HTTPS プロトコルを利用する必要があります。 |
| リソース | string | 必須です。 変更の監視対象となるリソースを指定します。 ベース URL (`https://graph.microsoft.com/v1.0/`) は含めないでください。 |
| expirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | 必須です。 webhook サブスクリプションの有効期限が切れる日時を指定します。 時刻は UTC 表示で、登録したリソースごとに異なるサブスクリプション作成からの経過時間にもできます。  サポートされているサブスクリプションの最長時間については、次の表をご覧ください。 |
| clientState | string | オプション。 各通知内のサービスによって送信される `clientState` プロパティの値を指定します。 最大の長さは 128 文字です。 クライアントは、サブスクリプションと共に送信された `clientState` プロパティの値と、各通知と共に受信された `clientState` プロパティの値を比較することで、その通知がサービスから来たことを確認できます。 |
| id | string | サブスクリプションの一意の識別子です。読み取り専用。 |
| applicationId | string | サブスクリプションを作成するときに使用するアプリケーションの識別子。 読み取り専用です。 |
| creatorId | string | サブスクリプションを作成したユーザーまたはサービス プリンシパルの識別子。 委任されたアクセス許可をアプリで使用してサブスクリプションを作成した場合、このフィールドには、アプリが代理で呼び出しを行っているサインインしているユーザーの ID が含まれます。 アプリがアプリケーション アクセス許可を使用した場合には、このフィールドには、アプリに対応するサービス プリンシパルの ID が含まれます。 読み取り専用です。 |

## <a name="maximum-length-of-subscription-per-resource-type"></a>リソースの種類別のサブスクリプションの最大の長さ

| リソース            | 最大有効期限  |
|:--------------------|:-------------------------|
| メール                | 4230 分 (3 日以内)    |
| カレンダー            | 4230 分 (3 日以内)    |
| 連絡先            | 4230 分 (3 日以内)    |
| グループ会話 | 4230 分 (3 日以内)    |
| ドライブ ルート項目    | 4230 分 (3 日以内)    |
| セキュリティの警告     | 43200 分 (30 日以内)  |

> **注:** 既存のアプリケーションと新規アプリケーションのどちらもサポートされている値を超えてはなりません。 将来的には、最大値を超えるサブスクリプションを作成または更新する要求はすべて失敗します。

## <a name="relationships"></a>リレーションシップ

なし

## <a name="methods"></a>メソッド

| メソッド | 戻り値の型 | 説明 |
|:-------|:------------|:------------|
| [Create subscription](../api/subscription-post-subscriptions.md) | [subscription](subscription.md) | Microsoft Graph のデータが変更されたときに通知を受信するリスナー アプリケーションに登録します。 |
| [Update subscription](../api/subscription-update.md) | [subscription](subscription.md) | 有効期限を更新することにより、サブスクリプションを更新します。 |
| [サブスクリプションのリスト作成](../api/subscription-list.md) | [サブスクリプション](subscription.md) | アクティブなサブスクリプションのリストを作成します。 |
| [サブスクリプションの取得](../api/subscription-get.md) | [subscription](subscription.md) | サブスクリプション オブジェクトのプロパティと関係を読み取ります。 |
| [サブスクリプションの削除](../api/subscription-delete.md) | なし |サブスクリプション オブジェクトを削除します。 |

[連絡先]: ./contact.md
[会話]: ./conversation.md
[driveItem]: ./driveitem.md
[イベント]: ./event.md
[グループ]: ./group.md
[メッセージ]: ./message.md
[ユーザー]: ./user.md
[警告]: ./alert.md

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
