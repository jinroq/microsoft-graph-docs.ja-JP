---
title: Shift を作成する
description: 新しい shift キーを作成します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8f9983ad5dd5fb5a0f2f36ddad80b7a874f6f68b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978055"
---
# <a name="create-shift"></a><span data-ttu-id="323b6-103">Shift を作成する</span><span class="sxs-lookup"><span data-stu-id="323b6-103">Create shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="323b6-104">[スケジュール](../resources/schedule.md)に新しい[shift](../resources/shift.md)インスタンスを作成します。</span><span class="sxs-lookup"><span data-stu-id="323b6-104">Create a new [shift](../resources/shift.md) instance in a [schedule](../resources/schedule.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="323b6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="323b6-105">Permissions</span></span>

<span data-ttu-id="323b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="323b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="323b6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="323b6-108">Permission type</span></span>      | <span data-ttu-id="323b6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="323b6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="323b6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="323b6-110">Delegated (work or school account)</span></span> | <span data-ttu-id="323b6-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="323b6-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="323b6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="323b6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="323b6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="323b6-113">Not supported.</span></span>    |
|<span data-ttu-id="323b6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="323b6-114">Application</span></span> | <span data-ttu-id="323b6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="323b6-115">Not supported.</span></span> |

> <span data-ttu-id="323b6-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="323b6-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="323b6-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="323b6-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="323b6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="323b6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teams/{teamId}/schedule/shifts
```

## <a name="request-headers"></a><span data-ttu-id="323b6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="323b6-119">Request headers</span></span>

| <span data-ttu-id="323b6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="323b6-120">Header</span></span>       | <span data-ttu-id="323b6-121">値</span><span class="sxs-lookup"><span data-stu-id="323b6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="323b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="323b6-122">Authorization</span></span>  | <span data-ttu-id="323b6-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="323b6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="323b6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="323b6-125">Content-Type</span></span>  | <span data-ttu-id="323b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="323b6-126">application/json</span></span>  |

## <a name="response"></a><span data-ttu-id="323b6-127">応答</span><span class="sxs-lookup"><span data-stu-id="323b6-127">Response</span></span>

<span data-ttu-id="323b6-128">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[shift](../resources/shift.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="323b6-128">If successful, this method returns a `201 Created` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="323b6-129">例</span><span class="sxs-lookup"><span data-stu-id="323b6-129">Example</span></span>

#### <a name="request"></a><span data-ttu-id="323b6-130">要求</span><span class="sxs-lookup"><span data-stu-id="323b6-130">Request</span></span>

<span data-ttu-id="323b6-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="323b6-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="323b6-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="323b6-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "schedule-post-shifts"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts
Content-type: application/json

{
  "id": "SHFT_577b75d2-a927-48c0-a5d1-dc984894e7b8",
  "userId": "c5d0c76b-80c4-481c-be50-923cd8d680a1",
  "schedulingGroupId": "TAG_228940ed-ff84-4e25-b129-1b395cf78be0",
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="323b6-133">C#</span><span class="sxs-lookup"><span data-stu-id="323b6-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/schedule-post-shifts-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="323b6-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="323b6-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/schedule-post-shifts-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="323b6-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="323b6-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/schedule-post-shifts-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="323b6-136">Java</span><span class="sxs-lookup"><span data-stu-id="323b6-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/schedule-post-shifts-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="323b6-137">応答</span><span class="sxs-lookup"><span data-stu-id="323b6-137">Response</span></span>

<span data-ttu-id="323b6-138">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="323b6-138">The following is an example of the response.</span></span> 

><span data-ttu-id="323b6-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="323b6-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.shift"
} -->

```http
HTTP/1.1 201 Created
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
  "description": "Creates a new shift",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
