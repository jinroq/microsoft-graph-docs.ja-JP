---
title: privilegedRoleAssignment を作成する
description: この API を使用して、新しい privilegedRoleAssignment を作成します。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 14866f6e007c4b9c82cd1e90082b2027e96d347e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361060"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="2ca18-103">privilegedRoleAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="2ca18-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ca18-104">この API を使用して、新しい[privilegedRoleAssignment](../resources/privilegedroleassignment.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="2ca18-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="2ca18-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2ca18-105">Permissions</span></span>
<span data-ttu-id="2ca18-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ca18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2ca18-108">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2ca18-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="2ca18-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ca18-109">Permission type</span></span>      | <span data-ttu-id="2ca18-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ca18-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ca18-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ca18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2ca18-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2ca18-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2ca18-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ca18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ca18-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ca18-114">Not supported.</span></span>    |
|<span data-ttu-id="2ca18-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ca18-115">Application</span></span> | <span data-ttu-id="2ca18-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ca18-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ca18-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ca18-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="2ca18-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ca18-118">Request headers</span></span>
| <span data-ttu-id="2ca18-119">名前</span><span class="sxs-lookup"><span data-stu-id="2ca18-119">Name</span></span>       | <span data-ttu-id="2ca18-120">説明</span><span class="sxs-lookup"><span data-stu-id="2ca18-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2ca18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ca18-121">Authorization</span></span>  | <span data-ttu-id="2ca18-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2ca18-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ca18-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ca18-124">Request body</span></span>
<span data-ttu-id="2ca18-125">要求本文で、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ca18-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2ca18-126">応答</span><span class="sxs-lookup"><span data-stu-id="2ca18-126">Response</span></span>

<span data-ttu-id="2ca18-127">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2ca18-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="2ca18-128">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="2ca18-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2ca18-129">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="2ca18-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="2ca18-130">例</span><span class="sxs-lookup"><span data-stu-id="2ca18-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2ca18-131">要求</span><span class="sxs-lookup"><span data-stu-id="2ca18-131">Request</span></span>
<span data-ttu-id="2ca18-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2ca18-132">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2ca18-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2ca18-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ca18-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ca18-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedroleassignment-from-privilegedroleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ca18-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ca18-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedroleassignment-from-privilegedroleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ca18-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="2ca18-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedroleassignment-from-privilegedroleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2ca18-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ca18-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedroleassignment-from-privilegedroleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="2ca18-138">要求本文で、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ca18-138">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2ca18-139">応答</span><span class="sxs-lookup"><span data-stu-id="2ca18-139">Response</span></span>
<span data-ttu-id="2ca18-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2ca18-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
