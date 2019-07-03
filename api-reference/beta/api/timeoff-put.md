---
title: TimeOff を置換する
description: 既存の休暇を置換します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 877d08b1c9b50e828cb9695f00a585880eeea694
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35457983"
---
# <a name="replace-timeoff"></a><span data-ttu-id="63848-103">TimeOff を置換する</span><span class="sxs-lookup"><span data-stu-id="63848-103">Replace timeOff</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63848-104">既存の[休暇](../resources/timeoff.md)を置換します。</span><span class="sxs-lookup"><span data-stu-id="63848-104">Replace an existing [timeOff](../resources/timeoff.md).</span></span>

<span data-ttu-id="63848-105">指定した[Timeoff](../resources/timeoff.md)が存在しない場合、 `404 Not found`このメソッドはを返します。</span><span class="sxs-lookup"><span data-stu-id="63848-105">If the specified [timeOff](../resources/timeoff.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="63848-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="63848-106">Permissions</span></span>

<span data-ttu-id="63848-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63848-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63848-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="63848-109">Permission type</span></span>      | <span data-ttu-id="63848-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="63848-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63848-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="63848-111">Delegated (work or school account)</span></span> | <span data-ttu-id="63848-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63848-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="63848-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="63848-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63848-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63848-114">Not supported.</span></span>    |
|<span data-ttu-id="63848-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="63848-115">Application</span></span> | <span data-ttu-id="63848-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63848-116">Not supported.</span></span> |

> <span data-ttu-id="63848-117">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="63848-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="63848-118">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="63848-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="63848-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="63848-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/timesOff/{timeOffId}
```

## <a name="request-headers"></a><span data-ttu-id="63848-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63848-120">Request headers</span></span>

| <span data-ttu-id="63848-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63848-121">Header</span></span>       | <span data-ttu-id="63848-122">値</span><span class="sxs-lookup"><span data-stu-id="63848-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="63848-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="63848-123">Authorization</span></span>  | <span data-ttu-id="63848-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="63848-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="63848-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="63848-126">Content-Type</span></span>  | <span data-ttu-id="63848-127">application/json</span><span class="sxs-lookup"><span data-stu-id="63848-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63848-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="63848-128">Request body</span></span>

<span data-ttu-id="63848-129">要求本文で、 [Timeoff](../resources/timeoff.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="63848-129">In the request body, supply a JSON representation of a [timeOff](../resources/timeoff.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="63848-130">応答</span><span class="sxs-lookup"><span data-stu-id="63848-130">Response</span></span>

<span data-ttu-id="63848-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[timeoff](../resources/timeoff.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="63848-131">If successful, this method returns a `200 OK` response code and a [timeOff](../resources/timeoff.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63848-132">例</span><span class="sxs-lookup"><span data-stu-id="63848-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="63848-133">要求</span><span class="sxs-lookup"><span data-stu-id="63848-133">Request</span></span>

<span data-ttu-id="63848-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="63848-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="63848-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="63848-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "timeoff-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/timesOff/{timeOffId}
Content-type: application/json
Prefer: return=representation

{
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="63848-136">C#</span><span class="sxs-lookup"><span data-stu-id="63848-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/timeoff-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="63848-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="63848-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/timeoff-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="63848-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="63848-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/timeoff-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="63848-139">応答</span><span class="sxs-lookup"><span data-stu-id="63848-139">Response</span></span>

<span data-ttu-id="63848-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="63848-140">The following is an example of the response.</span></span> 

><span data-ttu-id="63848-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="63848-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "@odata.type":"microsoft.graph.identitySet",
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
  "description": "Replace an existing timeOff",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
