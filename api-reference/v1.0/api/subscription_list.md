# <a name="list-subscriptions"></a>サブスクリプションのリストアップ

アプリ ID、ユーザー、テナントでのユーザーのロールに基づいて、Web フックへのサブスクリプションのプロパティと関係を取得します。

## <a name="permissions"></a>アクセス許可

この API では、次のアクセス許可の範囲をサポートしています。アクセス許可の選択方法などの詳細については、[アクセス許可](../../../concepts/permissions_reference.md) を参照してください。

| アクセス許可の種類  | アクセス許可 (権限が最小のものから最大のものへ)  |
|:---------------- |:-------------------------------------------- |
| [委任](../../../concepts/auth_v2_user.md) (職場または学校のアカウント) |  [サブスクリプションを作成](subscription_get.md) するのに、または Subscriptions.Read.All (下記参照) に必要なロールです。 |
| [委任](../../../concepts/auth_v2_user.md) (個人用 Microsoft アカウント) |  [サブスクリプションを作成](./subscription_get.md) するのに、または Subscriptions.Read.All (下記参照) に必要なロールです。 |
| [アプリケーション](../../../concepts/auth_v2_service.md) |  [サブスクリプションを作成](./subscription_get.md) するために必要なロールです。 |

応答の結果は、呼び出し元のアプリのコンテキストに基づいています。 以下は、一般的なシナリオの概要です。

### <a name="basic-scenarios"></a>基本的なシナリオ

ほとんどの場合、アプリケーションは、サインインしているユーザー向け、またはディレクトリ内のユーザー（仕事/学校のアカウント）向けに最初に作成したサブスクリプションを取得しようとします。 これらのシナリオでは、サブスクリプションを作成するのにアプリが最初に使用したものを越える、特殊なアクセス許可を必要としません。

| 呼び出し元のアプリのコンテキスト | 応答に含まれるもの |
|:-----|:---------------- |
| アプリはサインインしたユーザーの代理として呼び出しています（委任されたアクセス許可）。 <br/>および<br/>アプリには、 [サブスクリプションを作成](subscription_post_subscriptions.md) するために必要なオリジナルのアクセス許可があります。<br/><br/>注意: 個人用の Microsoft アカウントと仕事/学校のアカウントの両方に適用します。 | **このアプリ** が作成したサブスクリプションは、サインインしているユーザーのみに有効です。 |
| アプリは、アプリ自体の代理として呼び出しています（アプリケーション アクセス許可）<br/>および<br/>アプリには、 [サブスクリプションを作成](subscription_post_subscriptions.md) するために必要なオリジナルのアクセス許可があります。<br/><br/>注意: 仕事/学校のアカウントのみに適用します。| **このアプリ** が作成したサブスクリプションは、アプリ自体またはディレクトリ内のユーザーのみに有効です。|

### <a name="advanced-scenarios"></a>高度なシナリオ

場合によっては、アプリケーションは、他のアプリが作成したサブスクリプションを取得しようとします。 たとえば、あるユーザーが、アプリが作成したすべてのサブスクリプションを代理として閲覧しようとすることがあります。 または、管理者がディレクトリ内のすべてのアプリから、すべてのサブスクリプションを閲覧しようとするかもしれません。
このようなシナリオでは、委任されたアクセス許可 Subscription.Read.All が必要です。

| 呼び出し元のアプリのコンテキスト | 応答に含まれるもの |
|:-----|:---------------- |
| アプリはサインインしたユーザーの代理として呼び出しています（委任されたアクセス許可）。 *ユーザーは管理者ではありません*。 <br/>および<br/>アプリには、アクセス許可 Subscription.Read.All があります。<br/><br/>注意: 個人用の Microsoft アカウントと仕事/学校のアカウントの両方に適用します。 | **すべてのアプリ** が作成したサブスクリプションは、サインインしているユーザーのみに有効です。 |
| アプリはサインインしたユーザーの代理として呼び出しています（委任されたアクセス許可）。 *ユーザーは管理者です*。<br/>および<br/>アプリには、アクセス許可 Subscription.Read.All があります。<br/><br/>注意: 仕事/学校のアカウントのみに適用します。 | **すべてのアプリ** が作成したサブスクリプションは、ディレクトリ内の**すべてのユーザー** に対して有効です。|

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters)をサポートしていません。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| 承認  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文の [サブスクリプション](../resources/subscription.md) のリストを返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a>応答

応答の例をご覧ください。  簡潔にするために切り詰められる可能性があることにご注意ください。  要求と呼び出しのコンテキストに適切なサポートされたプロパティはすべて、実際の呼び出しから返されます。

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

要求が複数のページのデータを返す場合は、結果を管理するために応答には `@odata.nextLink` プロパティ含まれます。  詳細については、「[アプリで Microsoft Graph のデータをページングする](../../../concepts/paging.md)」を参照してください。
