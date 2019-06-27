---
title: アクティビティを削除する
description: アプリの既存のユーザーアクティビティを削除します。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: bc739a8f65f477528d603f57427e74734261cfd0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35275160"
---
# <a name="delete-an-activity"></a><span data-ttu-id="ee0f9-103">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="ee0f9-103">Delete an activity</span></span>

<span data-ttu-id="ee0f9-104">アプリの既存のユーザーアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="ee0f9-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="ee0f9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ee0f9-105">Permissions</span></span>

<span data-ttu-id="ee0f9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee0f9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ee0f9-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee0f9-108">Permission type</span></span>      | <span data-ttu-id="ee0f9-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee0f9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ee0f9-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee0f9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ee0f9-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ee0f9-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ee0f9-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee0f9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ee0f9-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="ee0f9-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="ee0f9-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee0f9-114">Application</span></span> | <span data-ttu-id="ee0f9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee0f9-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ee0f9-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee0f9-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="ee0f9-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee0f9-117">Request headers</span></span>

|<span data-ttu-id="ee0f9-118">名前</span><span class="sxs-lookup"><span data-stu-id="ee0f9-118">Name</span></span> | <span data-ttu-id="ee0f9-119">型</span><span class="sxs-lookup"><span data-stu-id="ee0f9-119">Type</span></span> | <span data-ttu-id="ee0f9-120">説明</span><span class="sxs-lookup"><span data-stu-id="ee0f9-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="ee0f9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee0f9-121">Authorization</span></span> | <span data-ttu-id="ee0f9-122">string</span><span class="sxs-lookup"><span data-stu-id="ee0f9-122">string</span></span> | <span data-ttu-id="ee0f9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ee0f9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee0f9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee0f9-125">Request body</span></span>

<span data-ttu-id="ee0f9-126">要求本文がありません。</span><span class="sxs-lookup"><span data-stu-id="ee0f9-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="ee0f9-127">応答</span><span class="sxs-lookup"><span data-stu-id="ee0f9-127">Response</span></span>

<span data-ttu-id="ee0f9-128">成功した場合、このメソッド`204 No Content`は、アクティビティが削除された場合に応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ee0f9-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="ee0f9-129">例</span><span class="sxs-lookup"><span data-stu-id="ee0f9-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ee0f9-130">要求</span><span class="sxs-lookup"><span data-stu-id="ee0f9-130">Request</span></span>

<span data-ttu-id="ee0f9-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee0f9-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/me/activities/{activity-id}/
```

##### <a name="response"></a><span data-ttu-id="ee0f9-132">応答</span><span class="sxs-lookup"><span data-stu-id="ee0f9-132">Response</span></span>

<span data-ttu-id="ee0f9-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="ee0f9-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ee0f9-134">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="ee0f9-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ee0f9-135">C#</span><span class="sxs-lookup"><span data-stu-id="ee0f9-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_activity-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ee0f9-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="ee0f9-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_activity-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ee0f9-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="ee0f9-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/delete_activity-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/projectrome-delete-activity.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
