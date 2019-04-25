---
title: サブスクリプションのリスト作成
description: " 詳細については、以下のシナリオを参照してください。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537091"
---
# <a name="list-subscriptions"></a>サブスクリプションのリスト作成

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

webhook サブスクリプションの一覧を取得します。 応答の内容は、アプリが呼び出しているコンテキストによって異なります。詳細については、以下のシナリオを参照してください。

## <a name="permissions"></a>アクセス許可

この API は、次のアクセス許可のスコープをサポートしています。アクセス許可の選択方法を含む詳細については、「 [permissions](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類  | アクセス許可 (特権の小さいものから大きいものへ)  |
|:---------------- |:-------------------------------------------- |
| [委任](/graph/auth-v2-user)された(職場または学校のアカウント) | サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。 |
| [委任](/graph/auth-v2-user)された(個人 Microsoft アカウント) | サブスクリプションまたはサブスクリプションを[作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 All (下を参照)。 |
| [アプリケーション](/graph/auth-v2-service) | [サブスクリプションを作成](subscription-post-subscriptions.md)するために必要なアクセス許可。 |

応答の結果は、呼び出し元アプリのコンテキストに基づいています。 一般的なシナリオの概要を次に示します。

### <a name="basic-scenarios"></a>基本的なシナリオ

最も一般的には、アプリケーションは、現在サインインしているユーザーまたはディレクトリ内のすべてのユーザーに対して最初に作成されたサブスクリプションを取得したいと考えています (職場または学校のアカウント)。 これらのシナリオでは、最初にサブスクリプションを作成するために使用されたアプリ以外の特別なアクセス許可は必要ありません。

| 呼び出し元アプリのコンテキスト | 応答の内容 |
|:-----|:---------------- |
| アプリは、サインインしているユーザーの代わりに呼び出しを行います (委任されたアクセス許可)。 <br/>/<br/>アプリには、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元のアクセス許可があります。<br/><br/>注: これは、個人用の Microsoft アカウントと職場/学校のアカウントの両方に適用されます。 | サインインしているユーザーに対してのみ、**このアプリ**によって作成されたサブスクリプション。 |
| アプリは自身の代わりに呼び出しをしています (アプリケーションアクセス許可)。<br/>/<br/>アプリには、[サブスクリプションを作成](subscription-post-subscriptions.md)するために必要な元のアクセス許可があります。<br/><br/>注: これは、職場または学校のアカウントにのみ適用されます。| **このアプリ**によって自分用またはディレクトリ内のユーザー用に作成されたサブスクリプション。|

### <a name="advanced-scenarios"></a>高度なシナリオ

場合によっては、他のアプリによって作成されたサブスクリプションをアプリで取得する必要があります。 たとえば、ユーザーは、任意のアプリによって作成されたすべてのサブスクリプションを自分に代わって表示したいと考えています。 または、管理者がディレクトリ内のすべてのアプリからのすべてのサブスクリプションを表示する必要がある場合があります。
このようなシナリオでは、委任されたアクセス許可のサブスクリプションが必要です。

| 呼び出し元アプリのコンテキスト | 応答の内容 |
|:-----|:---------------- |
| アプリは、サインインしているユーザーの代わりに呼び出しを行います (委任されたアクセス許可)。 *ユーザーが管理者ではない*。 <br/>/<br/>アプリには、アクセス許可のサブスクリプションがあります。 All<br/><br/>注: これは、個人用の Microsoft アカウントと職場/学校のアカウントの両方に適用されます。 | サインインしているユーザーに対してのみ、**そのアプリ**によって作成されたサブスクリプション。 |
| アプリは、サインインしているユーザーの代わりに呼び出しを行います (委任されたアクセス許可)。 *ユーザーが管理者*である。<br/>/<br/>アプリには、アクセス許可のサブスクリプションがあります。 All<br/><br/>注: これは、職場または学校のアカウントにのみ適用されます。 | ディレクトリ内の**すべてのユーザー**について、**任意のアプリ**によって作成されたサブスクリプション。|

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a>省略可能なクエリ パラメーター

このメソッドは、応答をカスタマイズするための[OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートしていません。

## <a name="request-headers"></a>要求ヘッダー

| 名前       | 型 | 説明|
|:-----------|:------|:----------|
| Authorization  | string  | ベアラー {トークン}。必須。 |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[subscription](../resources/subscription.md)オブジェクトのリストを返します。

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
  "truncated": false,
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
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

要求が複数のデータページを返す場合、応答には`@odata.nextLink`結果を管理するためのプロパティが含まれています。  詳細については、「[アプリで Microsoft Graph データをページング](/graph/paging)する」を参照してください。
