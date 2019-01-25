---
title: アクティビティを削除する
description: アプリの既存のユーザーのアクティビティを削除します。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: 78a3d2363d569a66985199fa2a6b2c6a5f6e5d30
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526936"
---
# <a name="delete-an-activity"></a><span data-ttu-id="4d6fc-103">アクティビティを削除する</span><span class="sxs-lookup"><span data-stu-id="4d6fc-103">Delete an activity</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4d6fc-104">アプリの既存のユーザーのアクティビティを削除します。</span><span class="sxs-lookup"><span data-stu-id="4d6fc-104">Delete an existing user activity for your app.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d6fc-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4d6fc-105">Permissions</span></span>

<span data-ttu-id="4d6fc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4d6fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d6fc-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4d6fc-108">Permission type</span></span>      | <span data-ttu-id="4d6fc-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4d6fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d6fc-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4d6fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4d6fc-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4d6fc-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4d6fc-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4d6fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d6fc-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="4d6fc-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="4d6fc-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4d6fc-114">Application</span></span> | <span data-ttu-id="4d6fc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4d6fc-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d6fc-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4d6fc-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4d6fc-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4d6fc-117">Request headers</span></span>

|<span data-ttu-id="4d6fc-118">名前</span><span class="sxs-lookup"><span data-stu-id="4d6fc-118">Name</span></span> | <span data-ttu-id="4d6fc-119">型</span><span class="sxs-lookup"><span data-stu-id="4d6fc-119">Type</span></span> | <span data-ttu-id="4d6fc-120">説明</span><span class="sxs-lookup"><span data-stu-id="4d6fc-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="4d6fc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d6fc-121">Authorization</span></span> | <span data-ttu-id="4d6fc-122">string</span><span class="sxs-lookup"><span data-stu-id="4d6fc-122">string</span></span> | <span data-ttu-id="4d6fc-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4d6fc-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4d6fc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4d6fc-125">Request body</span></span>

<span data-ttu-id="4d6fc-126">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="4d6fc-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="4d6fc-127">応答</span><span class="sxs-lookup"><span data-stu-id="4d6fc-127">Response</span></span>

<span data-ttu-id="4d6fc-128">かどうかは成功すると、このメソッドが返されます、`204 No Content`応答コードの場合は、アクティビティが削除されました。</span><span class="sxs-lookup"><span data-stu-id="4d6fc-128">If successful, this method returns the `204 No Content` response code if the activity was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="4d6fc-129">例</span><span class="sxs-lookup"><span data-stu-id="4d6fc-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="4d6fc-130">要求</span><span class="sxs-lookup"><span data-stu-id="4d6fc-130">Request</span></span>

<span data-ttu-id="4d6fc-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4d6fc-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_activity"
}-->

```http
DELETE https://graph.microsoft.com/beta/me/activities/13881113971988980728/
```

##### <a name="response"></a><span data-ttu-id="4d6fc-132">応答</span><span class="sxs-lookup"><span data-stu-id="4d6fc-132">Response</span></span>

<span data-ttu-id="4d6fc-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4d6fc-133">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-07 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete activity",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-delete-activity.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
