---
title: Outlook リソースのサブスクリプションと通知の喪失を減らす (プレビュー)
description: ユーザーのパスワードのリセットなどのセキュリティ イベントが原因で、Outlook で変更通知の配信が一時的に停止されることがあります。 通知の配信が中断されないよう、特殊なライフサイクル イベントである `subscriptionRemoved` および `missed` を処理する必要があります。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 1c430743f860536ef20fa2ad9974e580c78a6f0d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32683981"
---
# <a name="reduce-missing-subscriptions-and-notifications-for-outlook-resources-preview"></a>Outlook リソースのサブスクリプションと通知の喪失を減らす (プレビュー) 

Outlook リソースの通知の受信登録をしてあるアプリでは、サブスクリプションが削除され、通知が配信されない場合があります。 通知の継続的な配信を再開させるには、そのような消失を検出し、設定を復元するためのロジックをアプリで実装する必要があります。

Outlook で特定のイベントが発生すると、サブスクリプションが削除されることがあります。 これらのイベントには次のようなものがあります。

- ユーザーのパスワードがリセットされた場合
- ユーザーのデバイスが準拠しなくなった場合
-   ユーザーのアカウントが取り消された場合

このようなイベントが発生すると、Outlook は特殊なライフサイクル通知である `subscriptionRemoved` を送信します。

通知をアプリに配信できない場合、Outlook は `missed` という別のライフサイクル通知を送信します。

**メッセージ**や**イベント**などの Outlook リソースの受信登録をしてあるアプリでは、`subscriptionRemoved` と `missed` のシグナルが検出されます。

- `subscriptionRemoved` 通知を受信すると、継続的な受信を維持できるよう、アプリでサブスクリプションが再作成されます。
- `missed` 通知を受信した場合は、アプリでは Microsoft Graphを使用してリソース データが再同期されます。

ライフサイクル通知を受信するには、すでにリソース通知を受信している既存の **notificationUrl** エンドポイントを使用するか、`subscriptionRemoved` と `missed` 通知を異なるエンドポイントで受信できるように別の **lifecycleNotificationUrl** を登録するかのいずれを行います。

## <a name="creating-a-subscription"></a>サブスクリプションの作成

サブスクリプションを作成する際は、**lifecycleNotificationUrl** プロパティを使用して異なる通知エンドポイントを指定できます。 エンドポイントを指定すると、現在および将来のすべてのタイプのライフサイクル通知がそのエンドポイントに配信されます。 指定しない場合、既存のすべてのサブスクリプションに関連する `subscriptionRemoved` と `missed` 通知は既存の **notificationUrl** に配信されます。

> **注:** 現時点では、**lifecycleNotificationUrl** プロパティの設定または読み取りは、Microsoft Graph APIの `beta` バージョンを使用した場合のみ行えます。 ただし、`beta` を使用して作成されたサブスクリプションは `v1.0`と同じ運用環境に格納されるため、`v1.0` の通常の他のサブスクリプションの使用に加えて、ここで説明する新しい Outlook のフローを実装できます。

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
 
> **重要:** 両方の通知 URL で同じホスト名を使用します。 

> **注:** [通知に関する一般的な記事](webhooks.md#managing-subscriptions)で説明されているように、両方の通知エンドポイントを検証する必要があります。　　
両方のエンドポイントに同じ URL を使用することを選択した場合は、検証要求が 2 つ配信されるので、それらに応答します。

> **注:** 既存のサブスクリプションを更新 (`PATCH`) して **lifecycleNotificationUrl** プロパティを追加することはできません。  そのような既存のサブスクリプションは削除し、新しいサブスクリプションを作成して **lifecycleNotificationUrl** プロパティを指定する必要があります。 **lifecycleNotificationUrl** プロパティのない既存のサブスクリプションは、**notificationUrl** 経由で `subscriptionRemoved` と `missed` 通知を受け取ります。 

## <a name="responding-to-subscriptionremoved-notifications"></a>SubscriptionRemoved 通知に応答する

`subscriptionRemoved` 通知は、サブスクリプションが削除され、通知の受信を継続するにはサブスクリプションを再作成する必要があることを通知します。 

有効期限が長いサブスクリプション（例: 3 日）を作成すると、リソース データの通知の **notificationUrl** への送信が開始されます。 ただし、リソース データへのアクセスの条件は時間の経過とともに変化する可能性があるので注意が必要です。 たとえば、アプリでユーザーの再認証が必要になるイベントが Outlook サービスで発生する場合があります。 そのような場合、フローは次のようになります。

1. Outlook で、Microsoft Graph からサブスクリプションを削除する必要があることが検出されます。
    1. これらのイベントは、決まった頻度で発生するわけではありません。 イベントが頻繁に発生するリソースもあれば、ほとんど発生しないリソースもあります。

2. Microsoft Graph が `subscriptionRemoved` 通知を **lifecycleNotificationUrl** (指定されている場合) または **notificationUrl** に送信します。  

3. この通知には、同じリソースに対して新しいサブスクリプションを作成することにより応答できます。 これを行うには、有効なアクセス トークンを提示する必要があります。新しい有効なアクセス トークンを取得するために、アプリでユーザーを再認証する必要がある場合があります。

4. 新しいサブスクリプションを正常に作成すると、リソース通知の配信が再開されます。 作成に失敗した場合 (たとえば、アプリが有効なアクセス トークンを取得できなかった場合)、リソース通知は送信されません。

5. 新しいサブスクリプションを作成したら、喪失した変更を特定するためにリソース データを同期できます。

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

このタイプの通知にはいくつかの注意点があります。
- `"lifecycleEvent": "subscriptionRemoved"` フィールドは、この通知はサブスクリプションの削除に関連したものであることを示します。 他の種類のライフサイクル通知が配信される可能性もあり、今後は新しい通知が導入される予定です。
- 通知には特定のリソースに関する情報は含まれていません。通知はサブスクリプションの状態の変更に関するもので、リソースの変更とは関係がないためです。
- リソース通知と同様に、ライフサイクル通知はバッチ処理でき (**value** 配列内で)、それぞれの通知は異なる **lifecycleEvent** 値を持つことができます。 バッチ内の各通知を適切に処理します。

### <a name="actions-to-take"></a>必要なアクション

1. POST 呼び出しに `202 - Accepted` で応答し、通知の受信を[確認通知](webhooks.md#notifications)します。
2. 通知の信頼性を[検証します](webhooks.md#notifications)。
3. 次のステップに進むために必要な有効なアクセス トークンがアプリにあることを確認します。 
> **注:** いずれかの[認証ライブラリ](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries)を使用している場合、その認証ライブラリは、有効なキャッシュされたトークンを再利用するか、ユーザーに再度ログイン (新しいパスワードなどで) するよう要求するなどして新しいトークンを取得することにより、トークンを処理します。 アクセスの状況の変化などの理由により呼び出し側がリソース データへのアクセス許可を失っている場合があるため、新しいトークンの取得が失敗する可能性があることに注意してください。

4. [こちら](webhooks.md#subscription-request-example)に記載されている標準的な手順に従って、新しいサブスクリプションを作成します。

> **注:** システムが実行する承認チェックによりアプリまたはユーザーのリソースへのアクセスが拒否される可能性があるため、このアクションは失敗する可能性があります。 サブスクリプションを正常に再認証するには、アプリはユーザーから新しいアクセス トークンを取得する必要がある場合があります。 アクセス条件に変更があった場合などは、これらのアクションはいつでも再試行できます。 ライフサイクル通知が送信されてからアプリがサブスクリプションを正常に再作成するまでの間に発生したリソースの変更は、すべて失われます。 アプリは、それらの変更を独自に取得する必要があります。

5. 新しいサブスクリプションを作成した後、このリソースに関する通知を受け取った最後の既知の時間以降の受信できなかったリソース データを同期します。 例: `GET https://graph.microsoft.com/v1.0/users/{id}/messages?$filter=createdDateTime+ge+{LastTimeNotificationWasReceived}`

## <a name="responding-to-missed-notifications"></a>受信できなかった通知への応答

これらのシグナルは、配信されなかった可能性がある通知があることを知らせます。 これらのシグナルを無視するか対処するかを決めます。

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

このタイプの通知にはいくつかの注意点があります。
- この`"lifecycleEvent": "missed"` フィールドは、この通知は "missed" (受信出来なかった) 通知に関するシグナルであることを示します。 他の種類のライフサイクル通知が配信される可能性もあり、今後は新しい通知が導入される予定です。
- 通知には特定のリソースに関する情報は含まれていません。通知はサブスクリプションの状態の変更に関するもので、リソースの変更とは関係がないためです。
- リソース通知と同様に、ライフサイクル通知はバッチ処理でき (**value** 配列内で)、それぞれの通知は異なる **lifecycleEvent** 値を持つことができます。 バッチ内の各通知を適切に処理します。

### <a name="actions-to-take"></a>必要なアクション

1. POST 呼び出しに `202 - Accepted` で応答し、通知の受信を[確認通知](webhooks.md#notifications)します。
  - シグナルを無視する場合は、特に操作は必要ありません。 無視しない場合は:
2. 通知の信頼性を[検証します](webhooks.md#notifications)。
3. 通知として配信されなかった変更を特定するために、すべてのデータを対象にリソースの再同期を実行します。 


## <a name="future-proof-the-code-handling-lifecycle-notifications"></a>コードが今後もライフサイクル通知を処理できるようにする

Microsoft Graph では今後、より多くの種類のサブスクリプション ライフサイクル通知が追加される予定です。 これらの通知はこれまでと同じエンドポイント (**lifecycleNotificationUrl**) にポストされますが、通知の **lifecycleEvent** の値が変更され、通知を発行する目的のシナリオに固有の、これまでとはわずかに異なるスキーマとプロパティが含まれる可能性があります。

Microsoft Graph に新しい種類のライフサイクル通知が導入された場合でもコードが正常に動作するよう、コードは将来を見込んだ方法で実装する必要があります。 次のようなアプローチをお勧めします。

1. **lifecycleEvent** プロパティを使用して、サポートするイベントとして各通知を明示的に識別します。 たとえば、特定のイベントを識別するために `"lifecycleEvent": "subscriptionRemoved"` プロパティを探し、それを処理します。

2. 今後より多くの種類のライフサイクル通知が導入される可能性があるため、新しいシナリオの通知の発表を見まもるようにします。

3. アプリでは、アプリが認識しないすべてのライフサイクル イベントを無視するようにしますが、今後の参考にするために記録を残します。

4. 必要と判断する場合は、新しいライフサイクル通知に関連する資料を確認し、適切なサポートを実装します。

## <a name="see-also"></a>関連項目

- [Subscription リソースタイプ](/graph/api/resources/subscription?view=graph-rest-1.0)
- [サブスクリプションを取得する](/graph/api/subscription-get?view=graph-rest-1.0)
- [サブスクリプションを作成する](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)
- [サブスクリプションの削除](/graph/api/subscription-delete?view=graph-rest-1.0)
- [サブスクリプションの更新](/graph/api/subscription-update?view=graph-rest-1.0)
