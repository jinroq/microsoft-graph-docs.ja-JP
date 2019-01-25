---
title: HistoryItem を削除します。
description: 既存のユーザー アクティビティの既存の履歴項目を削除します。
localization_priority: Normal
ms.prod: project-rome
ms.openlocfilehash: b3e9a505c47c4d43aff71d5b4e40f08e3fe29d2b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520425"
---
# <a name="delete-a-historyitem"></a><span data-ttu-id="d2235-103">HistoryItem を削除します。</span><span class="sxs-lookup"><span data-stu-id="d2235-103">Delete a historyItem</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2235-104">既存のユーザー アクティビティの既存の履歴項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="d2235-104">Delete an existing history item for an existing user activity.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2235-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d2235-105">Permissions</span></span>

<span data-ttu-id="d2235-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d2235-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2235-108">Permission type</span></span>      | <span data-ttu-id="d2235-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2235-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2235-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2235-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2235-111">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d2235-111">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d2235-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2235-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2235-113">UserActivity.ReadWrite.CreatedByApp</span><span class="sxs-lookup"><span data-stu-id="d2235-113">UserActivity.ReadWrite.CreatedByApp</span></span>    |
|<span data-ttu-id="d2235-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2235-114">Application</span></span> | <span data-ttu-id="d2235-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2235-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2235-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2235-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /me/activities/{id}/historyItems/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d2235-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2235-117">Request headers</span></span>

|<span data-ttu-id="d2235-118">名前</span><span class="sxs-lookup"><span data-stu-id="d2235-118">Name</span></span> | <span data-ttu-id="d2235-119">型</span><span class="sxs-lookup"><span data-stu-id="d2235-119">Type</span></span> | <span data-ttu-id="d2235-120">説明</span><span class="sxs-lookup"><span data-stu-id="d2235-120">Description</span></span>|
|:----|:-----|:-----------|
|<span data-ttu-id="d2235-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2235-121">Authorization</span></span> | <span data-ttu-id="d2235-122">string</span><span class="sxs-lookup"><span data-stu-id="d2235-122">string</span></span> | <span data-ttu-id="d2235-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d2235-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2235-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2235-125">Request body</span></span>

<span data-ttu-id="d2235-126">要求の本体がありません。</span><span class="sxs-lookup"><span data-stu-id="d2235-126">No request body.</span></span>

## <a name="response"></a><span data-ttu-id="d2235-127">応答</span><span class="sxs-lookup"><span data-stu-id="d2235-127">Response</span></span>

<span data-ttu-id="d2235-128">かどうかは成功すると、このメソッドが返されます、 `204 No Content` 、履歴項目が削除された場合の応答コード。</span><span class="sxs-lookup"><span data-stu-id="d2235-128">If successful, this method returns the `204 No Content` response code if the history item was deleted.</span></span>

## <a name="example"></a><span data-ttu-id="d2235-129">例</span><span class="sxs-lookup"><span data-stu-id="d2235-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d2235-130">要求</span><span class="sxs-lookup"><span data-stu-id="d2235-130">Request</span></span>

<span data-ttu-id="d2235-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2235-131">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_historyItem"
}-->

```http
PUT https://graph.microsoft.com/beta/me/activities/13881113971988980728/historyItems/390e06e2-7e5b-4133-8014-fac7ac5991af
```

##### <a name="response"></a><span data-ttu-id="d2235-132">応答</span><span class="sxs-lookup"><span data-stu-id="d2235-132">Response</span></span>

<span data-ttu-id="d2235-133">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="d2235-133">Here is an example of the response.</span></span>

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
  "description": "Delete historyitem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/projectrome-delete-historyitem.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
