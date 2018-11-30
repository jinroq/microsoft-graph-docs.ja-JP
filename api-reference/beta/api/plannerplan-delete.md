---
title: Delete plannerPlan
description: '**plannerPlan** を削除します。'
ms.openlocfilehash: 6395d51eaed38b26d07f9b1ba8b0d78e52394404
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072916"
---
# <a name="delete-plannerplan"></a><span data-ttu-id="ab2fb-103">Delete plannerPlan</span><span class="sxs-lookup"><span data-stu-id="ab2fb-103">Delete plannerPlan</span></span>

> <span data-ttu-id="ab2fb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab2fb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab2fb-106">**plannerPlan** を削除します。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-106">Delete **plannerPlan**.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab2fb-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ab2fb-107">Permissions</span></span>
<span data-ttu-id="ab2fb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab2fb-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ab2fb-110">Permission type</span></span>      | <span data-ttu-id="ab2fb-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ab2fb-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab2fb-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ab2fb-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab2fb-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab2fb-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab2fb-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ab2fb-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab2fb-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-115">Not supported.</span></span>    |
|<span data-ttu-id="ab2fb-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ab2fb-116">Application</span></span> | <span data-ttu-id="ab2fb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab2fb-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ab2fb-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /planner/plans/<id>

```
## <a name="request-headers"></a><span data-ttu-id="ab2fb-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ab2fb-119">Request headers</span></span>
| <span data-ttu-id="ab2fb-120">名前</span><span class="sxs-lookup"><span data-stu-id="ab2fb-120">Name</span></span>       | <span data-ttu-id="ab2fb-121">説明</span><span class="sxs-lookup"><span data-stu-id="ab2fb-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ab2fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab2fb-122">Authorization</span></span>  | <span data-ttu-id="ab2fb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ab2fb-125">If-Match</span><span class="sxs-lookup"><span data-stu-id="ab2fb-125">If-Match</span></span>  | <span data-ttu-id="ab2fb-p104">削除する **plannerPlan** の最後の既知の ETag 値。必須。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-p104">Last known ETag value for the **plannerPlan** to be deleted. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab2fb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ab2fb-128">Request body</span></span>
<span data-ttu-id="ab2fb-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab2fb-130">応答</span><span class="sxs-lookup"><span data-stu-id="ab2fb-130">Response</span></span>

<span data-ttu-id="ab2fb-p105">成功した場合、このメソッドは `204 No Content` 応答コードを返します。応答本文には何も返されません。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

<span data-ttu-id="ab2fb-p106">このメソッドは、いずれかの [HTTP 状態コード](/graph/errors)を返します。このメソッドでアプリが処理する最も一般的なエラーは、400、403、404、409、412 応答です。これらのエラーの詳細については、「[一般的なプランナーのエラー条件](../resources/planner-overview.md#common-planner-error-conditions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-p106">This method can return any of the [HTTP status codes](/graph/errors). The most common errors that apps should handle for this method are the 400, 403, 404, 409, and 412 responses. For more information about these errors, see [Common Planner error conditions](../resources/planner-overview.md#common-planner-error-conditions).</span></span>

## <a name="example"></a><span data-ttu-id="ab2fb-136">例</span><span class="sxs-lookup"><span data-stu-id="ab2fb-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab2fb-137">要求</span><span class="sxs-lookup"><span data-stu-id="ab2fb-137">Request</span></span>
<span data-ttu-id="ab2fb-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_plannerplan"
}-->
```http
DELETE https://graph.microsoft.com/beta/planner/plans/<id>
If-Match: W/"JzEtVGFzayAgQEBAQEBAQEBAQEBAQEBAWCc="
```
##### <a name="response"></a><span data-ttu-id="ab2fb-139">応答</span><span class="sxs-lookup"><span data-stu-id="ab2fb-139">Response</span></span>
<span data-ttu-id="ab2fb-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ab2fb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Delete plannerPlan",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->