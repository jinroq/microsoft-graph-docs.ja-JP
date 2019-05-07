---
title: Shift を取得する
description: ID でシフトを取得します。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 207c9b40557d2f75ba73ecb76983dc9b9c8129f2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33638656"
---
# <a name="get-shift"></a><span data-ttu-id="f42e1-103">Shift を取得する</span><span class="sxs-lookup"><span data-stu-id="f42e1-103">Get shift</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f42e1-104">[Shift](../resources/shift.md)オブジェクトのプロパティとリレーションシップを ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="f42e1-104">Retrieve the properties and relationships of a [shift](../resources/shift.md) object by ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="f42e1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f42e1-105">Permissions</span></span>

<span data-ttu-id="f42e1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f42e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f42e1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f42e1-108">Permission type</span></span>      | <span data-ttu-id="f42e1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f42e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f42e1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f42e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f42e1-111">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f42e1-111">Group.Read.All, Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="f42e1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f42e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f42e1-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f42e1-113">Not supported.</span></span>    |
|<span data-ttu-id="f42e1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f42e1-114">Application</span></span> | <span data-ttu-id="f42e1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f42e1-115">Not supported.</span></span> |

> <span data-ttu-id="f42e1-116">**注**: この API は、管理者のアクセス許可をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f42e1-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="f42e1-117">グローバル管理者は、所属していないグループにアクセスできます。</span><span class="sxs-lookup"><span data-stu-id="f42e1-117">Global admins can access groups that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="f42e1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f42e1-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /teams/{teamId}/schedule/shifts/{shiftId}
```

## <a name="request-headers"></a><span data-ttu-id="f42e1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f42e1-119">Request headers</span></span>

| <span data-ttu-id="f42e1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f42e1-120">Header</span></span>       | <span data-ttu-id="f42e1-121">値</span><span class="sxs-lookup"><span data-stu-id="f42e1-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f42e1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f42e1-122">Authorization</span></span>  | <span data-ttu-id="f42e1-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f42e1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f42e1-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f42e1-125">Content-Type</span></span>  | <span data-ttu-id="f42e1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f42e1-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f42e1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f42e1-127">Request body</span></span>
<span data-ttu-id="f42e1-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f42e1-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f42e1-129">応答</span><span class="sxs-lookup"><span data-stu-id="f42e1-129">Response</span></span>

<span data-ttu-id="f42e1-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[shift](../resources/shift.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f42e1-130">If successful, this method returns a `200 OK` response code and a [shift](../resources/shift.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f42e1-131">例</span><span class="sxs-lookup"><span data-stu-id="f42e1-131">Example</span></span>

#### <a name="request"></a><span data-ttu-id="f42e1-132">要求</span><span class="sxs-lookup"><span data-stu-id="f42e1-132">Request</span></span>

<span data-ttu-id="f42e1-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f42e1-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "shift-get"
}-->
```http
GET https://graph.microsoft.com/beta/teams/{teamId}/schedule/shifts/{shiftId}
```

#### <a name="response"></a><span data-ttu-id="f42e1-134">応答</span><span class="sxs-lookup"><span data-stu-id="f42e1-134">Response</span></span>

<span data-ttu-id="f42e1-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f42e1-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f42e1-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f42e1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f42e1-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="f42e1-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f42e1-139">Visual</span><span class="sxs-lookup"><span data-stu-id="f42e1-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/shift-get-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f42e1-140">Java</span><span class="sxs-lookup"><span data-stu-id="f42e1-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/shift-get-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/shift-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/shift-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
