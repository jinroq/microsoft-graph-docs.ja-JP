---
title: privilegedApproval を作成する
description: この API を使用して、新しい privilegedApproval を作成します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 271590a1526fca37a385471a0efcdbb2956b341f
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412846"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="3f8a2-103">privilegedApproval を作成する</span><span class="sxs-lookup"><span data-stu-id="3f8a2-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f8a2-104">この API を使用して、新しい privilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="3f8a2-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3f8a2-105">Permissions</span></span>
<span data-ttu-id="3f8a2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3f8a2-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3f8a2-108">Permission type</span></span>      | <span data-ttu-id="3f8a2-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3f8a2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f8a2-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3f8a2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3f8a2-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="3f8a2-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3f8a2-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3f8a2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f8a2-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-113">Not supported.</span></span>    |
|<span data-ttu-id="3f8a2-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3f8a2-114">Application</span></span> | <span data-ttu-id="3f8a2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f8a2-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3f8a2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="3f8a2-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3f8a2-117">Request headers</span></span>
| <span data-ttu-id="3f8a2-118">名前</span><span class="sxs-lookup"><span data-stu-id="3f8a2-118">Name</span></span>       | <span data-ttu-id="3f8a2-119">説明</span><span class="sxs-lookup"><span data-stu-id="3f8a2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3f8a2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f8a2-120">Authorization</span></span>  | <span data-ttu-id="3f8a2-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f8a2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="3f8a2-123">Request body</span></span>
<span data-ttu-id="3f8a2-124">要求本文で、 [privilegedApproval](../resources/privilegedapproval.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3f8a2-125">応答</span><span class="sxs-lookup"><span data-stu-id="3f8a2-125">Response</span></span>

<span data-ttu-id="3f8a2-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[privilegedApproval](../resources/privilegedapproval.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="3f8a2-127">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="3f8a2-128">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="3f8a2-129">例</span><span class="sxs-lookup"><span data-stu-id="3f8a2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f8a2-130">要求</span><span class="sxs-lookup"><span data-stu-id="3f8a2-130">Request</span></span>
<span data-ttu-id="3f8a2-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="3f8a2-132">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3f8a2-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3f8a2-133">C#</span><span class="sxs-lookup"><span data-stu-id="3f8a2-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3f8a2-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f8a2-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3f8a2-135">目的-C</span><span class="sxs-lookup"><span data-stu-id="3f8a2-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="3f8a2-136">要求本文で、 [privilegedApproval](../resources/privilegedapproval.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-136">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3f8a2-137">応答</span><span class="sxs-lookup"><span data-stu-id="3f8a2-137">Response</span></span>
<span data-ttu-id="3f8a2-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3f8a2-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
