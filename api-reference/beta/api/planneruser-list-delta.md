---
title: 'プランナー: デルタ'
description: ユーザーが購読しているオブジェクトへの変更を取得します。
ms.openlocfilehash: 7c866946f0c9a873b99ee4efd6d9e2c7ce646be3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071826"
---
# <a name="planner-delta"></a><span data-ttu-id="b59f7-103">プランナー: デルタ</span><span class="sxs-lookup"><span data-stu-id="b59f7-103">Planner: delta</span></span>

> <span data-ttu-id="b59f7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b59f7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b59f7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b59f7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b59f7-106">ユーザーは、[購読して](../resources/planner-overview.md#track-changes-using-delta-query)いるオブジェクトへの変更を取得します。</span><span class="sxs-lookup"><span data-stu-id="b59f7-106">Retrieves changes to objects that the user is [subscribed](../resources/planner-overview.md#track-changes-using-delta-query) to.</span></span>

<span data-ttu-id="b59f7-107">このメソッドは、時間の経過と共に計画内でユーザーをからアクセスできるオブジェクトに対する変更を追跡するアプリケーションを使用します。</span><span class="sxs-lookup"><span data-stu-id="b59f7-107">This method allows your application to track changes to objects that the user can access from within Planner over time.</span></span>

<span data-ttu-id="b59f7-108">このメソッドの戻り値には、プランナーからのオブジェクトの種類を hetergenous が含まれている可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b59f7-108">The return value of this method might contain hetergenous types of objects from Planner.</span></span>

<span data-ttu-id="b59f7-109">グラフ データの変更の追跡の詳細については、[グラフ データの変更を追跡するためにデルタのクエリを使用する](/graph/delta-query-overview)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b59f7-109">For more information about tracking changes in Microsoft Graph data, see [Use delta query to track changes in Microsoft Graph data](/graph/delta-query-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="b59f7-110">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b59f7-110">Permissions</span></span>

<span data-ttu-id="b59f7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b59f7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b59f7-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b59f7-113">Permission type</span></span>      | <span data-ttu-id="b59f7-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b59f7-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b59f7-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b59f7-115">Delegated (work or school account)</span></span> | <span data-ttu-id="b59f7-116">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b59f7-116">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="b59f7-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b59f7-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b59f7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b59f7-118">Not supported.</span></span>    |
|<span data-ttu-id="b59f7-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b59f7-119">Application</span></span> | <span data-ttu-id="b59f7-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b59f7-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b59f7-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b59f7-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/planner/all/delta
GET /users/<id>/planner/all/delta
```

<span data-ttu-id="b59f7-122">追加のクエリ パラメーターが (次のように`$select`、 `$expand`、または`$filter`) デルタ ・ クエリのプランナーの実装では現在サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b59f7-122">No additional query parameters (such as `$select`, `$expand`, or `$filter`) are currently supported on Planner's implementation of delta queries.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b59f7-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b59f7-123">Request headers</span></span>

| <span data-ttu-id="b59f7-124">名前</span><span class="sxs-lookup"><span data-stu-id="b59f7-124">Name</span></span>           |<span data-ttu-id="b59f7-125">説明</span><span class="sxs-lookup"><span data-stu-id="b59f7-125">Description</span></span>                |
|:---------------|:--------------------------|
| <span data-ttu-id="b59f7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="b59f7-126">Authorization</span></span>  | <span data-ttu-id="b59f7-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b59f7-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b59f7-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="b59f7-129">Request body</span></span>

<span data-ttu-id="b59f7-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b59f7-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b59f7-131">応答</span><span class="sxs-lookup"><span data-stu-id="b59f7-131">Response</span></span>

<span data-ttu-id="b59f7-132">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本体と差分同期のリンク先に移動内のオブジェクトに適用される変更の集まりです。</span><span class="sxs-lookup"><span data-stu-id="b59f7-132">If successful, this method returns a `200 OK` response code and a collection of changes to be applied to objects in the response body, and a Delta Sync link to follow.</span></span>

<span data-ttu-id="b59f7-133">場合、`deltaLink`の呼び出し元の使用の形式が正しくありません、このエンドポイントが HTTP 400 を返すことです。</span><span class="sxs-lookup"><span data-stu-id="b59f7-133">If the `deltaLink` that the caller uses is malformed, this endpoint will return HTTP 400.</span></span>

<span data-ttu-id="b59f7-134">場合、`deltaLink`を呼び出し元の使用が古すぎるため、このエンドポイントは、HTTP 410 を返されます。</span><span class="sxs-lookup"><span data-stu-id="b59f7-134">If the `deltaLink` that the caller uses is too old, this endpoint will return HTTP 410.</span></span>

<span data-ttu-id="b59f7-p104">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b59f7-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="b59f7-138">例</span><span class="sxs-lookup"><span data-stu-id="b59f7-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="b59f7-139">要求</span><span class="sxs-lookup"><span data-stu-id="b59f7-139">Request</span></span>

<span data-ttu-id="b59f7-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b59f7-140">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_delta"
}-->

```http
GET https://graph.microsoft.com/beta/me/planner/all/delta
```

##### <a name="response"></a><span data-ttu-id="b59f7-141">応答</span><span class="sxs-lookup"><span data-stu-id="b59f7-141">Response</span></span>
<span data-ttu-id="b59f7-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b59f7-142">Here is an example of the response.</span></span>

><span data-ttu-id="b59f7-143">**注:** 応答オブジェクトが示すようには、読みやすさの短縮される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="b59f7-143">**Note:** The response object shown might be shortened for readability.</span></span> <span data-ttu-id="b59f7-144">変更されたすべてのプロパティは、実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b59f7-144">All the changed properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "List changes",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
