---
title: Delete plannerBucket
description: '**plannerBucket** を削除します。'
ms.openlocfilehash: 43ec9c8481482ef7ea3eadab0c5a9e2c0a3b356e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022527"
---
# <a name="delete-plannerbucket"></a><span data-ttu-id="48e53-103">Delete plannerBucket</span><span class="sxs-lookup"><span data-stu-id="48e53-103">Delete plannerBucket</span></span>

<span data-ttu-id="48e53-104">**plannerBucket** を削除します。</span><span class="sxs-lookup"><span data-stu-id="48e53-104">Delete **plannerBucket**.</span></span>
## <a name="permissions"></a><span data-ttu-id="48e53-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48e53-105">Permissions</span></span>
<span data-ttu-id="48e53-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48e53-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="48e53-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48e53-108">Permission type</span></span>      | <span data-ttu-id="48e53-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48e53-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48e53-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48e53-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48e53-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48e53-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="48e53-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48e53-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48e53-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48e53-113">Not supported.</span></span>    |
|<span data-ttu-id="48e53-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48e53-114">Application</span></span> | <span data-ttu-id="48e53-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="48e53-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="48e53-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48e53-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/buckets/{id}
```
## <a name="request-headers"></a><span data-ttu-id="48e53-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48e53-117">Request headers</span></span>
| <span data-ttu-id="48e53-118">名前</span><span class="sxs-lookup"><span data-stu-id="48e53-118">Name</span></span>       | <span data-ttu-id="48e53-119">説明</span><span class="sxs-lookup"><span data-stu-id="48e53-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="48e53-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="48e53-120">Authorization</span></span>  | <span data-ttu-id="48e53-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="48e53-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48e53-123">If-Match</span><span class="sxs-lookup"><span data-stu-id="48e53-123">If-Match</span></span>  | <span data-ttu-id="48e53-p103">削除する **plannerBucket** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="48e53-p103">Last known ETag value for the **plannerBucket** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="48e53-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="48e53-126">Request body</span></span>
<span data-ttu-id="48e53-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="48e53-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="48e53-128">応答</span><span class="sxs-lookup"><span data-stu-id="48e53-128">Response</span></span>

<span data-ttu-id="48e53-p104">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="48e53-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="48e53-p105">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48e53-p105">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="48e53-134">例</span><span class="sxs-lookup"><span data-stu-id="48e53-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="48e53-135">要求</span><span class="sxs-lookup"><span data-stu-id="48e53-135">Request</span></span>
<span data-ttu-id="48e53-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="48e53-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerbucket"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/planner/buckets/{id}
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="48e53-137">応答</span><span class="sxs-lookup"><span data-stu-id="48e53-137">Response</span></span>
<span data-ttu-id="48e53-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48e53-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete plannerBucket",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->