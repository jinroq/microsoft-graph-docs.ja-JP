---
title: 'Planner: delta'
description: ユーザーが購読しているオブジェクトへの変更を取得します。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: fbda4566dba9a8c21c9cc07e21a4b8d9bc96f1f4
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264303"
---
# <a name="planner-delta"></a><span data-ttu-id="0922a-103">Planner: delta</span><span class="sxs-lookup"><span data-stu-id="0922a-103">Planner: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0922a-104">ユーザーが[購読](../resources/planner-overview.md#track-changes-using-delta-query)しているオブジェクトへの変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="0922a-104">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="0922a-105">このメソッドを使用すると、ユーザーが随時プランナー内からアクセスできるオブジェクトへの変更をアプリケーションで追跡できます。</span><span class="sxs-lookup"><span data-stu-id="0922a-105">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="0922a-106">このメソッドの戻り値には、Planner からの異種の種類のオブジェクトが含まれている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0922a-106">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="0922a-107">Microsoft Graph データでの変更履歴の追跡の詳細については、「 [Microsoft graph のデータの変更を追跡するためにデルタクエリを使用する](/graph/delta-query-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0922a-107">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="0922a-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0922a-108">Permissions</span></span>

<span data-ttu-id="0922a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0922a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0922a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0922a-111">Permission type</span></span>      | <span data-ttu-id="0922a-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0922a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0922a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0922a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0922a-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0922a-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="0922a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0922a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0922a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0922a-116">Not supported.</span></span>    |
|<span data-ttu-id="0922a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0922a-117">Application</span></span> | <span data-ttu-id="0922a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0922a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0922a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0922a-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="0922a-120">プランナーのデルタクエリの実装で`$select`は`$expand`、追加`$filter`のクエリパラメーター (、、など) は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0922a-120">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0922a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0922a-121">Request headers</span></span>

| <span data-ttu-id="0922a-122">名前</span><span class="sxs-lookup"><span data-stu-id="0922a-122">Name</span></span>           |<span data-ttu-id="0922a-123">説明</span><span class="sxs-lookup"><span data-stu-id="0922a-123">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="0922a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0922a-124">Authorization</span></span>  | <span data-ttu-id="0922a-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0922a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0922a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0922a-127">Request body</span></span>

<span data-ttu-id="0922a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0922a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0922a-129">応答</span><span class="sxs-lookup"><span data-stu-id="0922a-129">Response</span></span>

<span data-ttu-id="0922a-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文のオブジェクトに適用される変更のコレクションと、それに続くデルタ同期リンクを返します。</span><span class="sxs-lookup"><span data-stu-id="0922a-130">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="0922a-131">発信者`deltaLink`が使用しているの形式が正しくない場合、このエンドポイントは HTTP 400 を返します。</span><span class="sxs-lookup"><span data-stu-id="0922a-131">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="0922a-132">呼び出し元`deltaLink`が使用しているが古すぎる場合、このエンドポイントは HTTP 410 を返します。</span><span class="sxs-lookup"><span data-stu-id="0922a-132">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="0922a-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0922a-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="0922a-136">例</span><span class="sxs-lookup"><span data-stu-id="0922a-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0922a-137">要求</span><span class="sxs-lookup"><span data-stu-id="0922a-137">Request</span></span>

<span data-ttu-id="0922a-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0922a-138">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```

##### <a name="response"></a><span data-ttu-id="0922a-139">応答</span><span class="sxs-lookup"><span data-stu-id="0922a-139">Response</span></span>
<span data-ttu-id="0922a-140">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="0922a-140">Here is an example of the response.</span></span>

><span data-ttu-id="0922a-141">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="0922a-141">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="0922a-142">変更されたすべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0922a-142">All the changed properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_delta",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.entity)",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
content-type: application/json;odata.metadata=minimal;odata.streaming=true;IEEE754Compatible=false;charset=utf-8
cache-control: private
client-request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
request-id: 3acb384b-e2d1-4a46-a347-e03bc6428cac
preference-applied: odata.track-changes, odata.track-changes

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.plannerDelta)",
    "@odata.deltaLink": "https://graph.microsoft.com/beta/me/planner/all/delta?$deltatoken=jVztGMFnm7qLEQ69FaXzWF5sPEJZU2YxZa32QEvnZTZ4q4C10ThM5uL7bEPm9ysqrxOY0QQIb4Uqmc9DH3rn7pczamvtCipDVJ4FivXh398.J9pSVKpytlutvx03-iBmO4ZM_3qPztOq2T9VIjHoRR0",
    "value": [
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBASCc=\"",
            "percentComplete": 100,
            "completedDateTime": "2018-03-13T21:31:25.778Z",
            "completedBy": {
                "user": {
                    "id": "8414b634-316f-41ba-b6a6-646a2949e3a5"
                }
            },
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBATCc=\"",
            "percentComplete": 0,
            "completedDateTime": null,
            "completedBy": null,
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        },
        {
            "@odata.type": "#microsoft.graph.plannerTask",
            "@odata.etag": "W/\"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAUCc=\"",
            "title": "Title change",
            "id": "5pNWKnX2XUalCKa64-oiXJUAPT1v",
            "@odata.context": "https://graph.microsoft.com/beta/$metadata#planner/tasks/$entity"
        }
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0922a-143">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="0922a-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0922a-144">C#</span><span class="sxs-lookup"><span data-stu-id="0922a-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_delta-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0922a-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="0922a-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_delta-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0922a-146">目的-C</span><span class="sxs-lookup"><span data-stu-id="0922a-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_delta-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/planneruser-list-delta.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/planneruser-list-delta.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/planneruser-list-delta.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
