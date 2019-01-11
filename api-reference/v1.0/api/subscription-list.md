---
title: リストの購読
description: プロパティとアプリケーション ID、ユーザー、およびテナントのユーザーのロールに基づいて、webhook サブスクリプションの関係を取得します。
localization_priority: Priority
ms.openlocfilehash: 663586cc769f04be631e1f3c1bdf86bc4f798022
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850415"
---
# <a name="list-subscriptions"></a>リストの購読

プロパティとアプリケーション ID、ユーザー、およびテナントのユーザーのロールに基づいて、webhook サブスクリプションの関係を取得します。

## <a name="permissions"></a>Permissions

この API には、次のアクセス許可のスコープがサポートされています。アクセス許可] を選択する方法などの詳細については、[アクセス許可](/graph/permissions-reference)を参照してください。

| アクセス許可の種類  | アクセス許可 (特権の小さいものから大きいものへ)  |
|:---------------- |:-------------------------------------------- |
| [委任されたアクセス許可](/graph/auth-v2-user)(職場、学校のアカウント) | [サブスクリプションを作成](subscription-post-subscriptions.md)または Subscription.Read.All (下記参照) に必要なロールです。 |
| [委任されたアクセス許可](/graph/auth-v2-user)(個人用の Microsoft アカウント) | [サブスクリプションを作成](subscription-post-subscriptions.md)または Subscription.Read.All (下記参照) に必要なロールです。 |
| [アプリケーションのアクセス許可](/graph/auth-v2-service) | [サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なロールです。 |

応答の結果は、呼び出し元のアプリケーションのコンテキストに基づいています。 以下は、一般的なシナリオの概要です。

### <a name="basic-scenarios"></a>基本的なシナリオ

ほとんどの場合、アプリケーションは、最初に作成された、現在サインインしているユーザーやディレクトリ (仕事/学校のアカウント) のすべてのユーザーのサブスクリプションを取得しようとします。 これらのシナリオは不要のもの以外の特殊なアクセス許可のサブスクリプションを作成する最初に使用するアプリケーションです。

| 呼び出し元のアプリケーションのコンテキスト | 応答が含まれています |
|:-----|:---------------- |
| サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。 <br/>- と -<br/>アプリケーションでは、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元の権限を持っています。<br/><br/>注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。 | サブスクリプションは、サインインしているユーザーに対してのみ、**このアプリケーション**によって作成されました。 |
| 自体 (アプリケーションのアクセス許可) のため、アプリケーションを呼び出しています。<br/>- と -<br/>アプリケーションでは、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元の権限を持っています。<br/><br/>注意: 仕事/学校のアカウントのみに適用します。| 自体やディレクトリ内のすべてのユーザーに、**このアプリケーション**によって作成されたサブスクリプション。|

### <a name="advanced-scenarios"></a>高度なシナリオ

場合によっては、アプリケーションは、他のアプリケーションによって作成されたサブスクリプションを取得しようとします。 たとえば、ユーザーは代わりに他のアプリケーションによって作成されたすべてのサブスクリプションを参照してください希望しています。 または、管理者はそのディレクトリ内のすべてのアプリケーションからのすべてのサブスクリプションを参照してくださいすることがあります。
このような状況では、Subscription.Read.All の委任されたアクセス許可が必要です。

| 呼び出し元のアプリケーションのコンテキスト | 応答が含まれています |
|:-----|:---------------- |
| サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。 *ユーザーは管理者以外*は。 <br/>- と -<br/>アプリには、アクセス許可が Subscription.Read.All<br/><br/>注意: 個人用の Microsoft アカウントとアカウントの仕事/学校の両方に適用します。 | サブスクリプションは、サインインしているユーザーに対してのみ **、アプリケーション**によって作成されました。 |
| サインインしているユーザー (委任されたアクセス許可) のため、アプリケーションを呼び出しています。 *ユーザーは管理者*です。<br/>- と -<br/>アプリには、アクセス許可が Subscription.Read.All<br/><br/>注意: 仕事/学校のアカウントのみに適用します。 | ディレクトリ内の**すべてのユーザー**の**すべてのアプリケーション**によって作成されるサブスクリプションです。|

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするために[OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 種類 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文のオブジェクトの[サブスクリプション](../resources/subscription.md)の一覧です。

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

ここでは、応答の例です。  簡潔にするために切り捨てられます可能性があることに注意してください。  すべての要求の適切なプロパティがサポートされているし、呼び出し元のコンテキストは、実際の呼び出しから返されます。

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

応答が含まれて、要求にデータの複数のページが返されるとき、 `@odata.nextLink` 、結果を管理するためのプロパティです。  詳細については、[アプリケーションでは、Microsoft Graph のページング データ](/graph/paging)を参照してください。
