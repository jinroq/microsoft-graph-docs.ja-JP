---
title: ActivityStatistics の取得
description: ユーザーの activityStatistics オブジェクトのプロパティを取得します。
localization_priority: Normal
author: madehmer
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 4ed9cda5da96957d3fbc1a4aa7e7919e78b74321
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36719214"
---
# <a name="get-activitystatistics"></a>ActivityStatistics の取得

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

ユーザーの[Activitystatistics](../resources/activitystatistics.md)オブジェクトのプロパティを取得します。

指定したユーザーと日付の範囲の[Activitystatistics](../resources/activitystatistics.md)の種類のプロパティを取得できます。 クエリ`id`で、[[アクティビティ id] プロパティ](../resources/activitystatistics.md#activity-id-property)のサポートされている形式を使用して、統計の種類と日付の範囲を指定できます。

## <a name="permissions"></a>アクセス許可

この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。

| アクセス許可の種類                        | アクセス許可 (特権の小さいものから大きいものへ) |
|:---------------------------------------|:--------------------------------------------|
| 委任 (職場または学校のアカウント)     | Analytics. 読み取り |
| 委任 (個人用 Microsoft アカウント) | サポートされていません。 |
| アプリケーション                            | サポートされていません。 |

## <a name="http-request"></a>HTTP 要求

<!-- { "blockType": "ignored" }  -->

```http
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/{id}

GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/analytics/activitystatistics/{id}

```

## <a name="optional-query-parameters"></a>オプションのクエリ パラメーター

このメソッドは、応答をカスタマイズするためのオプションのクエリパラメーターをサポートしていません。

## <a name="request-headers"></a>要求ヘッダー

| 名前      |説明|
|:----------|:----------|
| Authorization | ベアラー {トークン} |

## <a name="request-body"></a>要求本文

このメソッドには、要求本文を指定しません。

## <a name="response"></a>応答

成功した場合、このメソッド`200 OK`は応答コードと、要求されたアクティビティ統計の種類 ( [activitystatistics](../resources/activitystatistics.md)から派生した次のリソースのいずれか) を返します。 {[Call](../resources/callactivitystatistics.md)、[チャット](../resources/chatactivitystatistics.md)、[電子メール](../resources/emailactivitystatistics.md)、[フォーカス](../resources/focusactivitystatistics.md)、and [Meeting](../resources/meetingactivitystatistics.md)}。

## <a name="example"></a>例

#### <a name="request"></a>要求

次の例では、サインインしているユーザーの emailActivityStatistics の種類に関する統計情報を要求します。 2019-06-16 ~ 2019-06-17 の日付範囲を指定します。 一般 id プロパティの形式の詳細については、「 [activity id プロパティ](../resources/activitystatistics.md#activity-id-property)」を参照してください。


# <a name="httptabhttp"></a>[プロトコル](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_activitystatistics"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/analytics/activitystatistics/email_2019-06-16_2019-06-17

```
# <a name="ctabcsharp"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-activitystatistics-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-activitystatistics-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[目的-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-activitystatistics-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a>応答

次に示すのは、特定のアクティビティと日についてサインインしているユーザーのアクティビティ統計情報を取得する応答の例です。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityStatistics"
} -->

```http
HTTP/1.1 200 OK

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#activitystatistics/$entity",
    "@odata.type": "#microsoft.graph.emailActivityStatistics",
    "activity": "Email",
    "startDate": "2019-06-16",
    "endDate": "2019-06-17",
    "id": "email_2019-06-16_2019-06-17",
    "timeZoneUsed": "Pacific Standard Time",
    "duration": "PT0S",
    "afterHours": "PT0S",
    "readEmail": "PT0S",
    "sentEmail": "PT0S"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get activityStatistics",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
