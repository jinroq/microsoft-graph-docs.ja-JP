---
title: 'Planner: delta'
description: ユーザーが購読しているオブジェクトへの変更を取得します。
author: TarkanSevilmis
localization_priority: Normal
ms.prod: planner
ms.openlocfilehash: f5be8eb19d3af787e8a8910f702b51d2fc4095d6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35448348"
---
# <a name="planner-delta"></a><span data-ttu-id="4c4b7-103">Planner: delta</span><span class="sxs-lookup"><span data-stu-id="4c4b7-103">Planner: delta</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4c4b7-104">ユーザーが[購読](../resources/planner-overview.md#track-changes-using-delta-query)しているオブジェクトへの変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-104">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="4c4b7-105">このメソッドを使用すると、ユーザーが随時プランナー内からアクセスできるオブジェクトへの変更をアプリケーションで追跡できます。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-105">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="4c4b7-106">このメソッドの戻り値には、Planner からの異種の種類のオブジェクトが含まれている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-106">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="4c4b7-107">Microsoft Graph データでの変更履歴の追跡の詳細については、「 [Microsoft graph のデータの変更を追跡するためにデルタクエリを使用する](/graph/delta-query-overview)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-107">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="4c4b7-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4c4b7-108">Permissions</span></span>

<span data-ttu-id="4c4b7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c4b7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c4b7-111">Permission type</span></span>      | <span data-ttu-id="4c4b7-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c4b7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c4b7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c4b7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="4c4b7-114">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c4b7-114">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c4b7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c4b7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c4b7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-116">Not supported.</span></span>    |
|<span data-ttu-id="4c4b7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c4b7-117">Application</span></span> | <span data-ttu-id="4c4b7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c4b7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c4b7-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="4c4b7-120">プランナーのデルタクエリの実装で`$select`は`$expand`、追加`$filter`のクエリパラメーター (、、など) は現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-120">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4c4b7-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c4b7-121">Request headers</span></span>

| <span data-ttu-id="4c4b7-122">名前</span><span class="sxs-lookup"><span data-stu-id="4c4b7-122">Name</span></span>           |<span data-ttu-id="4c4b7-123">説明</span><span class="sxs-lookup"><span data-stu-id="4c4b7-123">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="4c4b7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c4b7-124">Authorization</span></span>  | <span data-ttu-id="4c4b7-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4c4b7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c4b7-127">Request body</span></span>

<span data-ttu-id="4c4b7-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4c4b7-129">応答</span><span class="sxs-lookup"><span data-stu-id="4c4b7-129">Response</span></span>

<span data-ttu-id="4c4b7-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文のオブジェクトに適用される変更のコレクションと、それに続くデルタ同期リンクを返します。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-130">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="4c4b7-131">発信者`deltaLink`が使用しているの形式が正しくない場合、このエンドポイントは HTTP 400 を返します。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-131">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="4c4b7-132">呼び出し元`deltaLink`が使用しているが古すぎる場合、このエンドポイントは HTTP 410 を返します。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-132">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="4c4b7-p103">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-p103">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="4c4b7-136">例</span><span class="sxs-lookup"><span data-stu-id="4c4b7-136">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4c4b7-137">要求</span><span class="sxs-lookup"><span data-stu-id="4c4b7-137">Request</span></span>

<span data-ttu-id="4c4b7-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-138">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="4c4b7-139">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4c4b7-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4c4b7-140">C#</span><span class="sxs-lookup"><span data-stu-id="4c4b7-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-delta-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4c4b7-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="4c4b7-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-delta-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4c4b7-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="4c4b7-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-delta-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4c4b7-143">応答</span><span class="sxs-lookup"><span data-stu-id="4c4b7-143">Response</span></span>
<span data-ttu-id="4c4b7-144">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-144">Here is an example of the response.</span></span>

><span data-ttu-id="4c4b7-145">**注:** ここに示す応答オブジェクトは、読みやすさのために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-145">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="4c4b7-146">変更されたすべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c4b7-146">All the changed properties will be returned from an actual call.</span></span>

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
  ]
}
-->
