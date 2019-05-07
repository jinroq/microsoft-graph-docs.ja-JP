---
title: サブスクリプションを一覧表示する
description: " 詳細については、以下のシナリオを参照してください。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 3728c3fcf2fe3d78b243894632a363804a2f92c8
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638698"
---
# <a name="list-subscriptions"></a>サブスクリプションを一覧表示する

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Webhook サブスクリプションの一覧を取得します。 応答の内容は、アプリが呼び出しているコンテキストによって異なります。詳細については、以下のシナリオを参照してください。

## <a name="permissions"></a>アクセス許可

この API は、次のアクセス許可スコープをサポートしています。アクセス許可の選択方法などに関する詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類  | アクセス許可 (特権の小さいものから大きいものへ)  |
|:---------------- |:-------------------------------------------- |
| [委任](/graph/auth-v2-user)された(職場または学校のアカウント) | サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。 |
| [委任](/graph/auth-v2-user)された(個人 Microsoft アカウント) | サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。 |
| [Application](/graph/auth-v2-service) | [サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 |

応答の結果は、呼び出し元アプリのコンテキストによって異なります。 次に、一般的なシナリオの概要を示します。

### <a name="basic-scenarios"></a>基本シナリオ

ほとんどの場合、アプリケーションは、現在サインインしているユーザーかディレクトリ (職場アカウントや学校アカウント) 内のすべてのユーザーに対してそのアプリケーションが元々作成していたサブスクリプションを取得しようとします。 このようなシナリオでは、アプリがサブスクリプションを作成するために元々使用していたアクセス許可以外には、特別なアクセス許可は必要ありません。

| 呼び出し元アプリのコンテキスト | 応答内容 |
|:-----|:---------------- |
| サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。 <br/>- および -<br/>[サブスクリプションの作成](subscription-post-subscriptions.md)に必要な元のアクセス許可をアプリが持っている。<br/><br/>注: これは、個人用の Microsoft アカウントと職場や学校のアカウントの両方に適用されます。 | **このアプリ**によって作成された、サインイン ユーザーのみのサブスクリプション。 |
| アプリがそのアプリのために呼び出しを実行している (アプリケーションのアクセス許可)。<br/>- および -<br/>[サブスクリプションの作成](subscription-post-subscriptions.md)に必要な元のアクセス許可をアプリが持っている。<br/><br/>注: これは、職場や学校のアカウントにのみ適用されます。| **このアプリ**によって作成された、アプリ自体またはディレクトリ内の任意のユーザーのサブスクリプション。|

### <a name="advanced-scenarios"></a>高度なシナリオ

場合によっては、アプリは、他のアプリによって作成されたサブスクリプションを取得しようとします。 たとえば、ユーザーが、自分に代わって任意のアプリによって作成されたすべてのサブスクリプションを確認しようとすることがあります。 また、管理者が、ディレクトリ内のすべてのアプリによって作成されたすべてのサブスクリプションを確認しようとすることがあります。
このような場合、委任されたアクセス許可の Subscription.Read.All が必要になります。

| 呼び出し元アプリのコンテキスト | 応答内容 |
|:-----|:---------------- |
| サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。 *ユーザーは管理者ではない*。 <br/>- および -<br/>Subscription.Read.All アクセス許可をアプリが持っている<br/><br/>注: これは、個人用の Microsoft アカウントと職場や学校のアカウントの両方に適用されます。 | **任意のアプリ**によって作成された、サインイン ユーザーのみのサブスクリプション。 |
| サインイン ユーザーに代わってアプリが呼び出しを実行している (委任されたアクセス許可)。 *ユーザーは管理者である*。<br/>- および -<br/>Subscription.Read.All アクセス許可をアプリが持っている<br/><br/>注: これは、職場や学校のアカウントにのみ適用されます。 | **任意のアプリ**によって作成された、ディレクトリ内の**任意のユーザー**のサブスクリプション。|

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [subscription](../resources/subscription.md) オブジェクトの一覧を返します。

## <a name="example"></a>例

##### <a name="request"></a>要求

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a>応答

以下は、応答の例です。 注: 簡潔にするために、ここに示す応答は切り捨てられる場合があります。 実際の呼び出しではすべてのプロパティが返されます。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
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
#### <a name="sdk-sample-code"></a>SDK サンプルコード
# <a name="ctabcs"></a>[Visual](#tab/cs)
[!INCLUDE [sample-code](../includes/get_subscriptions-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Java](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_subscriptions-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->

複数ページにわたるデータを要求が返す場合は、結果を管理しやすくするため、応答に `@odata.nextLink` プロパティが含まれます。  詳細については、「[アプリで Microsoft Graph データをページングする](/graph/paging)」を参照してください。
