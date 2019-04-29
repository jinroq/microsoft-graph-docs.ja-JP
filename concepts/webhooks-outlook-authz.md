---
title: Outlookリソースで、不足状態のサブスクリプションと通知を減らす（プレビュー）
description: ユーザーのパスワードのリセットなどのセキュリティイベントのため、Outlookは変更通知の配信を一時停止することがあります。 通知の中断のない配信を確保するために、特別なライフサイクルイベント - `subscriptionRemoved`および`missed`- を処理する必要があります。 　　
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 1c430743f860536ef20fa2ad9974e580c78a6f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32683981"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a>Outlookリソースで、不足状態のサブスクリプションと通知を減らす（プレビュー） 

Outlookリソースの通知を設定しているアプリが、通知設定を削除され通知を見逃すことがあります。 アプリは、検出し、損失から回復するためのロジックを実装して、継続的な通知のフローを再開する必要があります。

Outlook で特定のイベントでは、サブスクリプションが削除されることがあります。 これらのイベントには次のようなものがあります。

- ユーザーパスワードのリセット
- ユーザーデバイスの要件未準拠
-   ユーザーアカウントの取り消し

そのようなイベントが発生すると、Outlookは特別なライフサイクル通知`subscriptionRemoved`を送信します。

通知をアプリに配信できない場合、Outlookはあらためてもう一度ライフサイクル通知、 `missed`を送信します。

**メッセージ**や**イベント**などのOutlookリソースの通知を設定しているアプリは、`subscriptionRemoved`や `missed` シグナルを監視する必要があります。

- `subscriptionRemoved`通知を受信すると、アプリは継続的な流れを維持するためにサブスクリプションを再作成する必要があります。
- `missed` 通知を受信すると、アプリはMicrosoft Graphを使用してリソースデータを再同期する必要があります。

ライフサイクル通知を受信するには、既存の**notificationUrl**すでにリソース通知を受信しているエンドポイントを使用するか、あるいは別の**lifecycleNotificationUrl** を登録して、 `subscriptionRemoved` と`missed`通知を別のエンドポイントで受信できるようになります。

## <a name="creating-a-subscription"></a>サブスクリプションの作成

サブスクリプションを作成するときに、**lifecycleNotificationUrl**プロパティを使用して個別の通知エンドポイントを指定できます。 エンドポイントを指定すると、現在および将来のすべてのタイプのライフサイクル通知がそこに配信されます。 それ以外の場合、`subscriptionRemoved`と`missed`通知は既存のすべてのサブスクリプションについて既存の**notificationUrl**に配信されます。

> **注意:** 現時点では、 **lifecycleNotificationUrl**プロパティは、Microsoft Graph APIの `beta` バージョンを使用してのみ設定または読み取りができます。　 ただし、`beta`を使用して作成されたサブスクリプションは `v1.0`と同じ運用環境に格納されるため、`v1.0`の通常の他のサブスクリプションとの使用に加えて、ここで説明する新しいOutlookフローを実装できます。

### <a name="subscription-request-example"></a>サブスクリプション要求の例

```http
POST https://graph.microsoft.com/beta/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/api/resourceNotifications",
  "lifecycleNotificationUrl": "https://webhook.azurewebsites.net/api/lifecycleNotifications",
  "resource": "/users/{id}/messages",
  "expirationDateTime": "2019-03-20T11:00:00.0000000Z",
  "clientState": "<secretClientState>"
}
```
 
> **重要:** 両方通知 Url に同じホスト名を使用します。 

> **注意:** [一般的な通知の記事](webhooks.md#managing-subscriptions)で説明されているように、両方の通知エンドポイントを検証する必要があります。　　
両方のエンドポイントに同じURLを使用することを選択した場合は、2つの検証要求を受け取り応答します。

> **注意:** (`PATCH`) 既存のサブスクリプションを**lifecycleNotificationUrl**プロパティを追加するために更新することはできません。  そのような既存のサブスクリプションを削除し、新しいサブスクリプションを作成して**lifecycleNotificationUrl**プロパティを指定する必要があります。 **lifecycleNotificationUrl**プロパティのない既存のサブスクリプションは、**notificationUrl**を介して`subscriptionRemoved`および`missed`通知を受け取ります。 

## <a name="responding-to-subscriptionremoved-notifications"></a>SubscriptionRemoved 通知に応答します。

`subscriptionRemoved`通知によって、サブスクリプションが削除されたため再作成する必要があることが通知されますが、通知を継続して受け取りたい場合。 

長期間のサブスクリプション（3日など）を作成すると、リソースデータの通知が**notificationUrl**に送信され始めます。 しかしながら、リソースデータへのアクセスの条件は時間とともに変化し得るので注意が必要です。 たとえば、Outlookサービスでイベントが発生し、アプリでユーザーの再認証が必要になる場合があります。 そのような場合、フローは次のようになります。

1. Outlookは、サブスクリプションをMicrosoft Graphから削除する必要があることを検出しました。
    1. これらのイベントには決まった頻度があるわけではありません。 いくつかのリソースでは頻繁に発生し、他のリソースではほとんど発生しません。

2. Microsoft Graphは `subscriptionRemoved`通知を **lifecycleNotificationUrl** （指定されている場合）、または**notificationUrl**に送信します。  

3. 同じリソースに対して新しいサブスクリプションを作成することで、この通知に応答することができます。 これを行うには、有効なアクセス トークンを提示する必要があります。 場合によっては、アプリは新しい有効なアクセス トークンを取得するためにユーザーを再認証する必要があります。

4. 新しいサブスクリプションを正常に作成すると、リソースの通知が再開されます。 ただし、作成に失敗した場合（たとえば、アプリが有効なアクセス トークンを取得できなかった場合）、リソース通知は送信されません。

5. 新しいサブスクリプションを作成したら、リソースデータを同期して、不足している変更を特定できます。

### <a name="subscriptionremoved-notification-example"></a>SubscriptionRemoved 通知の例

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "subscriptionRemoved"
    }
  ]
}
```

このタイプの通知について注意することがいくつかあります。
- この`"lifecycleEvent": "subscriptionRemoved"`フィールドは、サブスクリプションの削除に関連するものとしてこの通知を指定します。 他の種類のライフサイクル通知も可能であり、新しいものが将来導入予定です。
- 通知には特定のリソースに関する情報は含まれていません。リソースの変更とは関係がなく、サブスクリプションの状態の変更のみに関するためです。
- リソース通知と同様に、ライフサイクル通知はまとめてバッチ処理することができ(**value** 配列内で)、それぞれが異なる**lifecycleEvent**値を持つことがあります。 それに応じてバッチ内の各通知を処理します。

### <a name="actions-to-take"></a>取るべきアクション

1. `202 - Accepted`でPOST呼び出しに応答して、通知の受信を[確認](webhooks.md#notifications)します。
2. 通知の信頼性を[検証します](webhooks.md#notifications)。
3. 次のステップに進むために、アプリに有効なアクセス トークンがあることを確認してください。 
> **注意:[認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) ** の1つを使用している場合、有効なキャッシュされたトークンを再利用するか、ユーザーに再度ログインするように要求するなど、新しいトークンを取得することでこれを処理します。 アクセスの状況が変化している可能性があり、呼び出し側がリソースデータへのアクセスを許可されなくなっている可能性があるため、新しいトークンの取得が失敗する可能性があることに注意してください。

4. [ここ](webhooks.md#subscription-request-example)に記載されている標準プロセスを使用して、新しいサブスクリプションを作成します。

> **注意:** システムによって実行される承認チェックによって、アプリまたはユーザーによるリソースへのアクセスが拒否される可能性があるため、このアクションは失敗する可能性があります。 サブスクリプションを正常に再認証するには、アプリがユーザーから新しいアクセス トークンを取得する必要がある場合があります。 アクセス条件に変化があった場合など、いつでもこれらのアクションを再試行できます。 ライフサイクル通知が送信されてからアプリがサブスクリプションを正常に再作成するまでの間に発生したリソースの変更はすべて失われます。 アプリは、独自にそれらの変更を取得する必要があります。

5. 新しいサブスクリプションを作成した後、このリソースに関する通知を受け取った最後の既知の時間から不足しているリソースデータを同期します。 例えば：`GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`

## <a name="responding-to-missed-notifications"></a>不在通知に応答します。

これらのシグナルは、いくつかの通知が配信されなかった可能性があることを知らせます。 これらのシグナルを無視するか対処するかをあなたは決めなければなりません。

### <a name="notification-example"></a>通知の例

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2019-03-20T11:00:00.0000000Z",
      "tenantId": "<tenant_guid>",
      "clientState":"<secretClientState>",
      "lifecycleEvent": "missed"
    }
  ]
}
```

このタイプの通知について注意することがいくつかあります。
- この`"lifecycleEvent": "missed"`フィールドは、これを見逃し通知に関するシグナルとして指定します。 他の種類のライフサイクル通知も可能であり、新しいものが将来導入予定です。
- 通知には特定のリソースに関する情報は含まれていません。リソースの変更とは関係がなく、サブスクリプションの状態の変更のみに関するためです
- リソース通知と同様に、ライフサイクル通知はまとめてバッチ処理することができ(**value** 配列内で)、それぞれが異なる**lifecycleEvent**値を持つことがあります。 それに応じてバッチ内の各通知を処理します。

### <a name="actions-to-take"></a>取るべきアクション

1. `202 - Accepted`でPOST呼び出しに応答して、通知の受信を[確認](webhooks.md#notifications)します。
  - 無視するのであれば、他には何もしないでください。 そうでない場合は:
2. 通知の信頼性を[検証します](webhooks.md#notifications)。
3. 通知として配信されなかった変更を識別するために、リソースの完全データ再同期を実行します。 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a>ライフ サイクルの通知を処理するコードを将来的にも有効にする

将来的には、Microsoft Graphはより多くの種類のサブスクリプションライフサイクル通知を追加する予定です。 それらは同じエンドポイント: **lifecycleNotificationUrl**にポストされますが、それらは**lifecycleEvent**下では異なる値を持ち、それらが発行されるシナリオに固有の、わずかに異なるスキーマとプロパティーを含むことがあります。

Microsoft Graphが新しいタイプのライフサイクル通知を導入したときにコードが壊れないよう、将来を見込んだ方法で実装する必要があります。 次のようなアプローチをお勧めします。

1. **lifecycleEvent**プロパティを使用して、サポートするイベントとして各通知を明示的に識別します。 たとえば、特定のイベントを識別するために`"lifecycleEvent": "subscriptionRemoved"` プロパティを探し、それを処理します。

2. 将来、より多くの種類のライフサイクル通知ができる可能性があるので、新しいシナリオの通知の発表に注意してください。いえしょう。

3. アプリでは、アプリが認識しないすべてのライフ サイクル イベントは無視しますが、記録はとって意識していたほうがよいでしょう。

4. あなたの判断で、新しいライフサイクル通知のための関連ドキュメントを調べて、それらのサポートを適切に実装してください。

## <a name="see-also"></a>関連項目

- [Subscription リソースタイプ](/graph/api/resources/subscription?view=graph-rest-1.0)
- [サブスクリプションを取得する](/graph/api/subscription-get?view=graph-rest-1.0)
- [サブスクリプションを作成する](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [サブスクリプションの削除](/graph/api/subscription-delete?view=graph-rest-1.0)
- [サブスクリプションの更新](/graph/api/subscription-update?view=graph-rest-1.0)
