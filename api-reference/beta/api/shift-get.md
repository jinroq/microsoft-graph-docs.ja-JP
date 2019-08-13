---
title: Shift を取得する
description: ID でシフトを取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 00745ad903d47b5fafac336e360ae2c9e5cf7668
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36363845"
---
# <a name="get-shift"></a><span data-ttu-id="ffea3-103">Shift を取得する</span><span class="sxs-lookup"><span data-stu-id="ffea3-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffea3-104">[Shift](../resources/shift.md)オブジェクトのプロパティとリレーションシップを ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="ffea3-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffea3-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ffea3-105">Permissions</span></span>

<span data-ttu-id="ffea3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffea3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ffea3-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffea3-108">Permission type</span></span>      | <span data-ttu-id="ffea3-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffea3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ffea3-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffea3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ffea3-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffea3-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ffea3-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ffea3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ffea3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffea3-113">Not supported.</span></span>    |
|<span data-ttu-id="ffea3-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffea3-114">Application</span></span> | <span data-ttu-id="ffea3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffea3-115">Not supported.</span></span> |

> <span data-ttu-id="ffea3-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ffea3-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="ffea3-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="ffea3-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="ffea3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffea3-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="ffea3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffea3-119">Request headers</span></span>

| <span data-ttu-id="ffea3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffea3-120">Header</span></span>       | <span data-ttu-id="ffea3-121">値</span><span class="sxs-lookup"><span data-stu-id="ffea3-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ffea3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffea3-122">Authorization</span></span>  | <span data-ttu-id="ffea3-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ffea3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="ffea3-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="ffea3-125">Content-Type</span></span>  | <span data-ttu-id="ffea3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ffea3-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ffea3-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ffea3-127">Request body</span></span>
<span data-ttu-id="ffea3-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ffea3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffea3-129">応答</span><span class="sxs-lookup"><span data-stu-id="ffea3-129">Response</span></span>

<span data-ttu-id="ffea3-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[shift](../resources/shift.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ffea3-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffea3-131">例</span><span class="sxs-lookup"><span data-stu-id="ffea3-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="ffea3-132">要求</span><span class="sxs-lookup"><span data-stu-id="ffea3-132">Request</span></span>

<span data-ttu-id="ffea3-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ffea3-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ffea3-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="ffea3-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ffea3-135">C#</span><span class="sxs-lookup"><span data-stu-id="ffea3-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-get-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ffea3-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ffea3-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-get-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ffea3-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="ffea3-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-get-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ffea3-138">Java</span><span class="sxs-lookup"><span data-stu-id="ffea3-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/shift-get-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="ffea3-139">応答</span><span class="sxs-lookup"><span data-stu-id="ffea3-139">Response</span></span>

<span data-ttu-id="ffea3-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ffea3-140">The following is an example of the response.</span></span> 

><span data-ttu-id="ffea3-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="ffea3-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 401

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "createdDateTime": "2019-03-14T04:32:51.451Z",
  "lastModifiedDateTime": "2019-03-14T05:32:51.451Z",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "conversation": null,
    "user": {
      "id": "366c0b19-49b1-41b5-a03f-9f3887bd0ed8",
      "displayName": "John Doe"
    }
  },
  "sharedShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:15:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  },
  "draftShift": {
    "displayName": "Day shift",
    "notes": "Please do inventory as part of your shift.",
    "startDateTime": "2019-03-11T15:00:00Z",
    "endDateTime": "2019-03-12T00:00:00Z",
    "theme": "blue",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2019-03-11T15:00:00Z",
        "endDateTime": "2019-03-11T15:30:00Z",
        "code": "",
        "displayName": "Lunch"
      }
    ]
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get a shift by id",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
