---
title: Shift を置換する
description: 既存の稼働時間帯を置き換えます。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1f600f3b08dd404829a0655cde40cb1a2f9cef48
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36410074"
---
# <a name="replace-shift"></a><span data-ttu-id="3ed72-103">Shift を置換する</span><span class="sxs-lookup"><span data-stu-id="3ed72-103">Replace shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ed72-104">既存の[稼働時間帯](../resources/shift.md)を置き換えます。</span><span class="sxs-lookup"><span data-stu-id="3ed72-104">Replace an existing [shift](../resources/shift.md).</span></span>

<span data-ttu-id="3ed72-105">指定した[シフト](../resources/shift.md)が存在しない場合、 `404 Not found`このメソッドはを返します。</span><span class="sxs-lookup"><span data-stu-id="3ed72-105">If the specified [shift](../resources/shift.md) doesn't exist, this method returns `404 Not found`.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ed72-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3ed72-106">Permissions</span></span>

<span data-ttu-id="3ed72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3ed72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3ed72-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3ed72-109">Permission type</span></span>      | <span data-ttu-id="3ed72-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3ed72-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3ed72-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3ed72-111">Delegated (work or school account)</span></span> | <span data-ttu-id="3ed72-112">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ed72-112">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="3ed72-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3ed72-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ed72-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ed72-114">Not supported.</span></span>    |
|<span data-ttu-id="3ed72-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3ed72-115">Application</span></span> | <span data-ttu-id="3ed72-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3ed72-116">Not supported.</span></span> |

> <span data-ttu-id="3ed72-117">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3ed72-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="3ed72-118">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="3ed72-118">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="3ed72-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3ed72-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PUT /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="3ed72-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ed72-120">Request headers</span></span>

| <span data-ttu-id="3ed72-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3ed72-121">Header</span></span>       | <span data-ttu-id="3ed72-122">値</span><span class="sxs-lookup"><span data-stu-id="3ed72-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="3ed72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ed72-123">Authorization</span></span>  | <span data-ttu-id="3ed72-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3ed72-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3ed72-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3ed72-126">Content-Type</span></span>  | <span data-ttu-id="3ed72-127">application/json</span><span class="sxs-lookup"><span data-stu-id="3ed72-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3ed72-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="3ed72-128">Request body</span></span>

<span data-ttu-id="3ed72-129">要求本文で、 [shift](../resources/shift.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3ed72-129">In the request body, supply a JSON representation of a [shift](../resources/shift.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3ed72-130">応答</span><span class="sxs-lookup"><span data-stu-id="3ed72-130">Response</span></span>

<span data-ttu-id="3ed72-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[shift](../resources/shift.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3ed72-131">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3ed72-132">例</span><span class="sxs-lookup"><span data-stu-id="3ed72-132">Example</span></span>

#### <a name="request"></a><span data-ttu-id="3ed72-133">要求</span><span class="sxs-lookup"><span data-stu-id="3ed72-133">Request</span></span>

<span data-ttu-id="3ed72-134">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3ed72-134">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3ed72-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3ed72-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "shift-put"
}-->
```http
PUT https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
Content-type: application/json
Prefer: return=representation

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
# <a name="ctabcsharp"></a>[<span data-ttu-id="3ed72-136">C#</span><span class="sxs-lookup"><span data-stu-id="3ed72-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/shift-put-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3ed72-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ed72-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/shift-put-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3ed72-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="3ed72-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/shift-put-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="3ed72-139">応答</span><span class="sxs-lookup"><span data-stu-id="3ed72-139">Response</span></span>

<span data-ttu-id="3ed72-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3ed72-140">The following is an example of the response.</span></span> 

><span data-ttu-id="3ed72-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3ed72-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "id": "string",
  "userId": "string",
  "schedulingGroupId": "string",
  "sharedShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "draftShift": {
    "notes": "string",
    "displayName": "string",
    "startDateTime": "2018-10-04T00:58:45.340Z",
    "endDateTime": "2018-10-04T00:58:45.340Z",
    "theme": "white",
    "activities": [
      {
        "isPaid": true,
        "startDateTime": "2018-10-04T00:58:45.340Z",
        "endDateTime": "2018-10-04T00:58:45.340Z",
        "code": "string",
        "displayName": "string"
      }
    ]
  },
  "createdDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedDateTime": "2018-10-04T00:58:45.340Z",
  "lastModifiedBy": {
    "user": {
      "id": "string",
      "displayName": "string"
    },
    "application": {
      "id": "string",
      "displayName": "string"
    },
    "device": {
      "id": "string",
      "displayName": "string"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Replace an existing shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
