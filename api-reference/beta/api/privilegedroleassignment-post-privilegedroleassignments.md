---
title: privilegedRoleAssignment を作成する
description: この API を使用して、新しい privilegedRoleAssignment を作成します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8c46bc01ee9df4e252dda26453065ca73b67a0ed
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36412671"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="c4211-103">privilegedRoleAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="c4211-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4211-104">この API を使用して、新しい[privilegedRoleAssignment](../resources/privilegedroleassignment.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="c4211-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="c4211-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c4211-105">Permissions</span></span>
<span data-ttu-id="c4211-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4211-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c4211-108">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c4211-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="c4211-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c4211-109">Permission type</span></span>      | <span data-ttu-id="c4211-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c4211-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4211-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c4211-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c4211-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4211-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4211-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c4211-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4211-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4211-114">Not supported.</span></span>    |
|<span data-ttu-id="c4211-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c4211-115">Application</span></span> | <span data-ttu-id="c4211-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4211-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4211-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c4211-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="c4211-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c4211-118">Request headers</span></span>
| <span data-ttu-id="c4211-119">名前</span><span class="sxs-lookup"><span data-stu-id="c4211-119">Name</span></span>       | <span data-ttu-id="c4211-120">説明</span><span class="sxs-lookup"><span data-stu-id="c4211-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c4211-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4211-121">Authorization</span></span>  | <span data-ttu-id="c4211-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c4211-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4211-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="c4211-124">Request body</span></span>
<span data-ttu-id="c4211-125">要求本文で、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c4211-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c4211-126">応答</span><span class="sxs-lookup"><span data-stu-id="c4211-126">Response</span></span>

<span data-ttu-id="c4211-127">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c4211-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="c4211-128">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c4211-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c4211-129">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c4211-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c4211-130">例</span><span class="sxs-lookup"><span data-stu-id="c4211-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4211-131">要求</span><span class="sxs-lookup"><span data-stu-id="c4211-131">Request</span></span>
<span data-ttu-id="c4211-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c4211-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c4211-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c4211-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4211-134">C#</span><span class="sxs-lookup"><span data-stu-id="c4211-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4211-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4211-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4211-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="c4211-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="c4211-137">要求本文で、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c4211-137">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c4211-138">応答</span><span class="sxs-lookup"><span data-stu-id="c4211-138">Response</span></span>
<span data-ttu-id="c4211-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c4211-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
