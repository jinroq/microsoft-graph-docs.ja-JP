---
title: privilegedRoleAssignment を作成する
description: この API を使用して、新しい privilegedRoleAssignment を作成します。
localization_priority: Normal
ms.openlocfilehash: d6fb9462f429cfc19c5d4cf0e1829da6057674c4
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33593816"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="22ed9-103">privilegedRoleAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="22ed9-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22ed9-104">この API を使用して、新しい[privilegedRoleAssignment](../resources/privilegedroleassignment.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="22ed9-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="22ed9-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="22ed9-105">Permissions</span></span>
<span data-ttu-id="22ed9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22ed9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="22ed9-108">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="22ed9-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="22ed9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22ed9-109">Permission type</span></span>      | <span data-ttu-id="22ed9-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="22ed9-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="22ed9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22ed9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="22ed9-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="22ed9-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="22ed9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22ed9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="22ed9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22ed9-114">Not supported.</span></span>    |
|<span data-ttu-id="22ed9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22ed9-115">Application</span></span> | <span data-ttu-id="22ed9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22ed9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="22ed9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22ed9-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="22ed9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22ed9-118">Request headers</span></span>
| <span data-ttu-id="22ed9-119">名前</span><span class="sxs-lookup"><span data-stu-id="22ed9-119">Name</span></span>       | <span data-ttu-id="22ed9-120">説明</span><span class="sxs-lookup"><span data-stu-id="22ed9-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="22ed9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="22ed9-121">Authorization</span></span>  | <span data-ttu-id="22ed9-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="22ed9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="22ed9-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="22ed9-124">Request body</span></span>
<span data-ttu-id="22ed9-125">要求本文で、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22ed9-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="22ed9-126">応答</span><span class="sxs-lookup"><span data-stu-id="22ed9-126">Response</span></span>

<span data-ttu-id="22ed9-127">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="22ed9-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="22ed9-128">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="22ed9-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="22ed9-129">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="22ed9-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="22ed9-130">例</span><span class="sxs-lookup"><span data-stu-id="22ed9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="22ed9-131">要求</span><span class="sxs-lookup"><span data-stu-id="22ed9-131">Request</span></span>
<span data-ttu-id="22ed9-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22ed9-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="22ed9-133">要求本文で、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22ed9-133">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="22ed9-134">応答</span><span class="sxs-lookup"><span data-stu-id="22ed9-134">Response</span></span>
<span data-ttu-id="22ed9-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22ed9-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="22ed9-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="22ed9-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="22ed9-139">Visual</span><span class="sxs-lookup"><span data-stu-id="22ed9-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_privilegedroleassignment_from_privilegedroleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="22ed9-140">Java</span><span class="sxs-lookup"><span data-stu-id="22ed9-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_privilegedroleassignment_from_privilegedroleassignments-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
