---
title: List buckets
description: '**plannerbucket** オブジェクトのリストを取得します。'
ms.openlocfilehash: fe5882faac32550a8611fa0a70fa677468ea891e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070720"
---
# <a name="list-buckets"></a><span data-ttu-id="350d2-103">List buckets</span><span class="sxs-lookup"><span data-stu-id="350d2-103">List buckets</span></span>

> <span data-ttu-id="350d2-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="350d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="350d2-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="350d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="350d2-106">**plannerbucket** オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="350d2-106">Retrieve a list of **plannerbucket** objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="350d2-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="350d2-107">Permissions</span></span>
<span data-ttu-id="350d2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="350d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="350d2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="350d2-110">Permission type</span></span>      | <span data-ttu-id="350d2-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="350d2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="350d2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="350d2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="350d2-113">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="350d2-113">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="350d2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="350d2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="350d2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="350d2-115">Not supported.</span></span>    |
|<span data-ttu-id="350d2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="350d2-116">Application</span></span> | <span data-ttu-id="350d2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="350d2-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="350d2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="350d2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /planner/buckets
```
## <a name="optional-query-parameters"></a><span data-ttu-id="350d2-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="350d2-119">Optional query parameters</span></span>
<span data-ttu-id="350d2-120">このメソッドでは planId [フィルター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="350d2-120">This method requires planId [filter](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to be specified.</span></span>

## <a name="request-headers"></a><span data-ttu-id="350d2-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="350d2-121">Request headers</span></span>
| <span data-ttu-id="350d2-122">名前</span><span class="sxs-lookup"><span data-stu-id="350d2-122">Name</span></span>      |<span data-ttu-id="350d2-123">説明</span><span class="sxs-lookup"><span data-stu-id="350d2-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="350d2-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="350d2-124">Authorization</span></span>  | <span data-ttu-id="350d2-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="350d2-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="350d2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="350d2-127">Request body</span></span>
<span data-ttu-id="350d2-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="350d2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="350d2-129">応答</span><span class="sxs-lookup"><span data-stu-id="350d2-129">Response</span></span>

<span data-ttu-id="350d2-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [plannerBucket](../resources/plannerbucket.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="350d2-130">If successful, this method returns a `200 OK` response code and collection of [plannerBucket](../resources/plannerbucket.md) objects in the response body.</span></span>

<span data-ttu-id="350d2-p104">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、403 および 404 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="350d2-p104">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 403 and 404 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>
## <a name="example"></a><span data-ttu-id="350d2-134">例</span><span class="sxs-lookup"><span data-stu-id="350d2-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="350d2-135">要求</span><span class="sxs-lookup"><span data-stu-id="350d2-135">Request</span></span>
<span data-ttu-id="350d2-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="350d2-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_buckets"
}-->
```http
GET https://graph.microsoft.com/beta/planner/buckets
```
##### <a name="response"></a><span data-ttu-id="350d2-137">応答</span><span class="sxs-lookup"><span data-stu-id="350d2-137">Response</span></span>
<span data-ttu-id="350d2-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="350d2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.plannerBucket",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "value": [
    {
      "@odata.etag": "W/\"JzEtQnVja2V0QEBAQEBAQEBAQEBAQEBARCc=\"",
      "name": "To do",
      "planId": "2txjA-BMZEq-bKi6Wfj5aGQAB1OJ",
      "orderHint": "85752723360752+",
      "id": "hsOf2dhOJkqyYYZEtdzDe2QAIUCR"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List buckets",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->