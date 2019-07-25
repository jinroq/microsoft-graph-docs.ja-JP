---
title: TimeOff を取得する
description: ID で timeOff を取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6cc0d75684e040855a85b71e5aa0a4b4ecccb2ca
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35868061"
---
# <a name="get-timeoff"></a><span data-ttu-id="6d984-103">TimeOff を取得する</span><span class="sxs-lookup"><span data-stu-id="6d984-103">Get timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6d984-104">[Timeoff](../resources/timeoff.md)オブジェクトのプロパティと関係を ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="6d984-104">Retrieve the properties and relationships of a [timeOff](../resources/timeoff.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d984-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6d984-105">Permissions</span></span>

<span data-ttu-id="6d984-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d984-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d984-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6d984-108">Permission type</span></span>      | <span data-ttu-id="6d984-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6d984-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d984-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6d984-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6d984-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d984-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d984-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6d984-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d984-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d984-113">Not supported.</span></span>    |
|<span data-ttu-id="6d984-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6d984-114">Application</span></span> | <span data-ttu-id="6d984-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6d984-115">Not supported.</span></span> |

> <span data-ttu-id="6d984-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6d984-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="6d984-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="6d984-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="6d984-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6d984-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="6d984-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d984-119">Request headers</span></span>

| <span data-ttu-id="6d984-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6d984-120">Header</span></span>       | <span data-ttu-id="6d984-121">値</span><span class="sxs-lookup"><span data-stu-id="6d984-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6d984-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d984-122">Authorization</span></span>  | <span data-ttu-id="6d984-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6d984-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6d984-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6d984-125">Content-Type</span></span>  | <span data-ttu-id="6d984-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d984-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6d984-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6d984-127">Request body</span></span>
<span data-ttu-id="6d984-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6d984-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6d984-129">応答</span><span class="sxs-lookup"><span data-stu-id="6d984-129">Response</span></span>

<span data-ttu-id="6d984-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[timeoff](../resources/timeoff.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6d984-130">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d984-131">例</span><span class="sxs-lookup"><span data-stu-id="6d984-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="6d984-132">要求</span><span class="sxs-lookup"><span data-stu-id="6d984-132">Request</span></span>

<span data-ttu-id="6d984-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d984-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6d984-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="6d984-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6d984-135">C#</span><span class="sxs-lookup"><span data-stu-id="6d984-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6d984-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="6d984-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6d984-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="6d984-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6d984-138">Java</span><span class="sxs-lookup"><span data-stu-id="6d984-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/timeoff-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="6d984-139">応答</span><span class="sxs-lookup"><span data-stu-id="6d984-139">Response</span></span>

<span data-ttu-id="6d984-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d984-140">The following is an example of the response.</span></span> 

><span data-ttu-id="6d984-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6d984-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.timeOff"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "createdDateTime": "2019-03-14T05:35:57.755Z",
  "lastModifiedDateTime": "2019-03-14T05:36:08.381Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "white"
  },
  "draftTimeOff": {
    "timeOffReasonId": "TOR_891045ca-b5d2-406b-aa06-a3c8921245d7",
    "startDateTime": "2019-03-11T07:00:00Z",
    "endDateTime": "2019-03-12T07:00:00Z",
    "theme": "pink"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a timeOff by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
