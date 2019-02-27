---
title: ユーザー データの変更に関する通知の設定
description: Microsoft Graph の API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 48f9d16374219868418107201ef13a1bf14fb7da
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263378"
---
# <a name="set-up-notifications-for-changes-in-user-data"></a>ユーザー データの変更に関する通知の設定

Microsoft Graph の API は、webhook メカニズムを使用して、クライアントに通知を配信します。クライアントは、通知を受信するために自身の URL を構成する Web サービスです。クライアント アプリは通知を使用して、変更時に状態を更新します。

Microsoft Graph はサブスクリプション要求を受け入れると、サブスクリプションで指定された URL に通知をプッシュします。 アプリはその後、そのビジネス ロジックに従ってアクションを実行します。 たとえば、詳細データのフェッチ、そのキャッシュやビューの更新などです。

## <a name="supported-resources"></a>サポートされているリソース

Microsoft Graph の API を使用すると、アプリは次のリソースに変更を登録できます。

- Outlook [メッセージ][]
- Outlook [イベント][]
- Outlook 個人用[連絡先][]
- [ユーザー][]
- [グループ][]
- Office 365 グループ[会話][]
- ユーザーの個人用 OneDrive 上の_任意のフォルダーの_ [driveItem][] 階層内のコンテンツ
- OneDrive for Business 上の_ルート フォルダーの _ [driveItem][] 階層内のコンテンツ
- セキュリティの[警告][]

受信トレイなど特定の Outlook フォルダーに対してサブスクリプションを作成できます: `me/mailFolders('inbox')/messages`

あるいは、最上位レベルのリソース: `me/messages`、`me/contacts`、`me/events`、`users`、または `groups`

あるいは、特定のリソース インスタンス: `users/{id}`、`groups/{id}`、`groups/{id}/conversations`

または、ユーザーの個人用 OneDrive 内の任意のフォルダー: `/drives/{id}/root`
`/drives/{id}/root/subfolder`

あるいは、Sharepoint/OneDrive for Business ドライブのルート フォルダー: `/drive/root`

または、新しい[セキュリティ API](security-concept-overview.md) の警告: `/security/alerts?$filter=status eq ‘New’`、`/security/alerts?$filter=vendorInformation/provider eq ‘ASC’`

### <a name="azure-ad-resource-limitations"></a>Azure AD リソースの制限

Azure AD ベースのリソース (ユーザー、グループ) には一定の制限が適用され、超過するとエラーが発生する可能性があります。

- 最大サブスクリプションのクォータ:

  - アプリあたり: 合計 50,000 サブスクリプション
  - テナントあたり: すべてのアプリで合計 1000 サブスクリプション
  - アプリとテナントの組み合わせ: 合計 100 サブスクリプション

- Azure AD B2C テナントはサポートされていません。

- ユーザー エンティティの通知は、個人用 Microsoft アカウントではサポートされていません。

## <a name="subscription-lifetime"></a>サブスクリプション ライフタイム

サブスクリプションのライフタイムには制限があります。 アプリは、有効期限が切れる前にサブスクリプションを更新する必要があります。 そうしない場合、新しいサブスクリプションを作成する必要があります。 最長有効期限の一覧については、「[リソースの種類別のサブスクリプションの最大の長さ](/graph/api/resources/subscription?view=graph-rest-1.0#maximum-length-of-subscription-per-resource-type)」をご覧ください。

また、アプリはいつでも登録を解除して、通知の受信を停止できます。

## <a name="managing-subscriptions"></a>サブスクリプションの管理

クライアントは、サブスクリプションを作成したり、サブスクリプションを更新したり、サブスクリプションを削除したりできます。

### <a name="creating-a-subscription"></a>サブスクリプションの作成

リソースの通知の受信を開始する最初の手順は、サブスクリプションの作成です。サブスクリプション プロセスは、次のようになります。

1. クライアントは、特定のリソースのサブスクリプション要求 (POST) を送信します。

1. Microsoft Graph が要求を確認します。

    - 要求が有効な場合、Microsoft Graph は検証トークンを通知 URL に送信します。
    - 要求が無効である場合、Microsoft Graph は、エラー コードと詳細の付いたエラー応答を送信します。

1. クライアントは、Microsoft Graph に検証トークンを返送します。

1. Microsoft Graph からクライアントに応答が送信されます。

クライアントは、サブスクリプションに通知を関連付けるために、サブスクリプション ID を格納する必要があります。

#### <a name="subscription-request-example"></a>サブスクリプション要求の例

```http
POST https://graph.microsoft.com/v1.0/subscriptions
Content-Type: application/json
{
  "changeType": "created,updated",
  "notificationUrl": "https://webhook.azurewebsites.net/notificationClient",
  "resource": "/me/mailfolders('inbox')/messages",
  "expirationDateTime": "2016-03-20T11:00:00.0000000Z",
  "clientState": "SecretClientState"
}
```

プロパティの `changeType`、`notificationUrl`、`resource`、および `expirationDateTime` は必須です。 プロパティの定義と値については、「[サブスクリプション リソースの種類](/graph/api/resources/subscription?view=graph-rest-1.0)」をご覧ください。

`resource` プロパティは、変更の監視対象となるリソースを指定します。 たとえば、特定のメール フォルダーへサブスクリプションを作成できます: `me/mailFolders('inbox')/messages`または、管理者の同意を得たユーザーの代わりに作成できます: `users/john.doe@onmicrosoft.com/mailFolders('inbox')/messages`。

`clientState` は必須ではありませんが、推奨される通知の処理プロセスに準拠するには含める必要があります。 このプロパティを設定すると、受け取る通知が Microsoft Graph サービスから来たものであることを確認することができます。 その理由で、このプロパティの値は機密として保たなければならず、使用はアプリケーションと Microsoft Graph サービスのためにのみ限るようにしてください。

処理が正常に終了すると、Microsoft Graph は `201 Created` コードおよび本文内に [サブスクリプション](/graph/api/resources/subscription?view=graph-rest-1.0) オブジェクトを返します。

#### <a name="notification-endpoint-validation"></a>通知エンドポイントの検証

Microsoft Graph により、サブスクリプション作成の前にサブスクリプション要求の `notificationUrl` プロパティの中で提供される通知エンドポイントが検証されます。 検証プロセスは、次のようになります。

1. Microsoft Graph が通知 URL に POST 要求を送信します。

    ``` http
    POST https://{notificationUrl}?validationToken={opaqueTokenCreatedByMicrosoftGraph}
    ```

    > **重要:** `validationToken` はクエリ パラメーターであるため、クライアントが HTTP コーディング プラクティスに従って適切にデコードする必要があります。 クライアントがトークンをデコードせず、代わりに次の手順で示すエンコードされた値 (応答) を使用する場合、検証は失敗します。 また、トークンの形式は将来予告なしに変更される可能性があるため、クライアントはトークン値を曖昧なものとして処理する必要があります。

1. クライアントは 10 秒以内に次の特性を持つ応答を提供する必要があります。

    - 200 (OK) 状態コード。
    - コンテンツ タイプは `text/plain` でなければなりません。
    - 本文には Microsoft Graph が提供した検証トークンを含める必要があります。

クライアントは、応答を提供した後は検証トークンを破棄する必要があります。

### <a name="renewing-a-subscription"></a>サブスクリプションの更新

クライアントは、要求時から最大 3 日間の特定の有効期限日を持つサブスクリプションを更新できます。 `expirationDateTime` プロパティは必須です。

#### <a name="subscription-renewal-example"></a>サブスクリプションの更新の例

```http
PATCH https://graph.microsoft.com/v1.0/subscriptions/{id}
Content-Type: application/json

{
  "expirationDateTime": "2016-03-22T11:00:00.0000000Z"
}
```

処理が正常に終了すると、Microsoft Graph は `200 OK` コードおよび本文内に [サブスクリプション](/graph/api/resources/subscription?view=graph-rest-1.0) オブジェクトを返します。 サブスクリプション オブジェクトには、新しい `expirationDateTime` 値が含まれます。

### <a name="deleting-a-subscription"></a>サブスクリプションの削除

クライアントは、その ID を使用してサブスクリプションを削除することにより、通知の受信を停止できます。

```http
DELETE https://graph.microsoft.com/v1.0/subscriptions/{id}
```

処理が正常に終了すると、Microsoft Graph は `204 No Content` コードを返します。

## <a name="notifications"></a>通知

クライアントはサブスクリプションを作成した後、通知の受信を開始します。 Microsoft Graph は、リソースに変更が発生すると通知 URL に POST 要求を送信します。 通知が送信されるのは、`created` など、サブスクリプションで指定されているタイプの変更についてのみです。

> **注:** 同じリソース タイプを監視し、同じ通知 URL を使用する複数のサブスクリプションを使用している場合、サブスクリプション ID が異なる複数の通知が含まれる POST が送信されることがあります。 その POST に含まれるすべての通知が、単一のサブスクリプションに属しているという保証はありません。

### <a name="notification-properties"></a>通知のプロパティ

通知オブジェクトには、次のプロパティがあります。

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
| subscriptionId | string | 通知を生成したサブスクリプションの ID。 |
| subscriptionExpirationDateTime | [dateTime](https://tools.ietf.org/html/rfc3339) | サブスクリプションの有効期限が切れるとき。 |
| clientState | string | サブスクリプション要求で指定された `clientState` プロパティ (存在する場合)。 |
| changeType | string | 通知の原因となったイベントの種類。 たとえば、メール受信時は `created`、または読んだメッセージをマークした場合は `updated`。 |
| resource | string | `https://graph.microsoft.com` に関連するリソースの URI。 |
| resourceData | object | このプロパティの内容は、サブスクリプションの対象となるリソースの種類に応じて異なります。 |

たとえば、Outlook リソースの場合、`resourceData` には次のフィールドが含まれています:

| プロパティ | 型 | 説明 |
|:---------|:-----|:------------|
| @odata.type | string | 表しているオブジェクトを記述する、Microsoft Graph の OData エンティティ タイプ。 |
| @odata.id | string | オブジェクトの OData 識別子。 |
| @odata.etag | string | オブジェクトのバージョンを表す HTTP エンティティ タグ。 |
| ID | string | オブジェクトの識別子。 |

> **注:** `resourceData` で提供される `id` 値は、通知生成時に有効だったものです。 メッセージを別のフォルダーに移動するなど、アクションによっては、通知処理時に `id` が有効でなくなるという結果になる場合があります。

### <a name="notification-example"></a>通知の例

ユーザーが電子メールを受信すると、Microsoft Graph は次のように通知を送信します。

```json
{
  "value": [
    {
      "subscriptionId":"<subscription_guid>",
      "subscriptionExpirationDateTime":"2016-03-19T22:11:09.952Z",
      "clientState":"secretClientValue",
      "changeType":"created",
      "resource":"users/{user_guid}@<tenant_guid>/messages/{long_id_string}",
      "resourceData":
      {
        "@odata.type":"#Microsoft.Graph.Message",
        "@odata.id":"Users/{user_guid}@<tenant_guid>/Messages/{long_id_string}",
        "@odata.etag":"W/\"CQAAABYAAADkrWGo7bouTKlsgTZMr9KwAAAUWRHf\"",
        "id":"<long_id_string>"
      }
    }
  ]
}
```

`value` フィールドはオブジェクトの配列であることに注意してください。 キューに多数の通知が入っている場合、Microsoft Graph から、単一の要求の中で複数の項目が送信されることがあります。 同じ通知要求の中に、異なる複数のサブスクリプションからの通知が含まれることがあります。

### <a name="processing-the-notification"></a>通知の処理

アプリの受け取る通知を、それぞれ処理する必要があります。 アプリが通知を処理するために必要な最小限のタスクは、次のようになります。

1. `clientState` プロパティを検証します。 これは、サブスクリプション作成要求で当初送られた値に一致していなければなりません。

    > **注:** そうでない場合、これを有効な通知と見なすことはできません。 通知が Microsoft Graph に由来するものでなく、悪意のある者が偽って送った可能性があります。 また、通知の送信元を調査し、適切なアクションを実行する必要があります。

1. ビジネス ロジックに基づいて、アプリケーションを更新します。

1. Microsoft Graph への応答で、`202 - Accepted` ステータス コードを送信します。 Microsoft Graph が 2xx クラス コードを受信しない場合は、通知を何回でも再試行します。

    > **注:** `clientState`プロパティがサブスクリプション要求のものと一致しない場合でも、`202 - Accepted` ステータス コードを送信する必要があります。 これは、偽通知が信頼されていないかもしれないという事実を悪意のある者が検出し、それを利用して `clientState` プロパティの値を類推するのを防ぐことになるため、優れた方法と言えます。

要求内の他の通知について、これらを繰り返します。

## <a name="code-samples"></a>コード サンプル

GitHub では、次のコード サンプルを利用できます。

- [Node.js 用 Microsoft Graph Webhooks のサンプル](https://github.com/OfficeDev/Microsoft-Graph-Nodejs-Webhooks)
- [ASP.NET 用 Microsoft Graph Webhooks のサンプル](https://github.com/OfficeDev/Microsoft-Graph-ASPNET-Webhooks)
- [WebJobs SDK を使用した Microsoft Graph ユーザー Webhook のサンプル](https://github.com/microsoftgraph/webjobs-webhooks-sample)

## <a name="see-also"></a>関連項目

- [Subscription リソースタイプ](/graph/api/resources/subscription?view=graph-rest-1.0)
- [サブスクリプションを取得する](/graph/api/subscription-get?view=graph-rest-1.0)
- [サブスクリプションを作成する](/graph/api/subscription-post-subscriptions?view=graph-rest-1.0)

[連絡先]: /graph/api/resources/contact?view=graph-rest-1.0
[会話]: /graph/api/resources/conversation?view=graph-rest-1.0
[driveItem]: /graph/api/resources/driveitem?view=graph-rest-1.0
[イベント]: /graph/api/resources/event?view=graph-rest-1.0
[グループ]: /graph/api/resources/group?view=graph-rest-1.0
[メッセージ]: /graph/api/resources/message?view=graph-rest-1.0
[ユーザー]: /graph/api/resources/user?view=graph-rest-1.0
[警告]: /graph/api/resources/alert?view=graph-rest-1.0
