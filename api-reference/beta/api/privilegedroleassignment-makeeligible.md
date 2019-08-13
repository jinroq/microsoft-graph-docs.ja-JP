---
title: 'privilegedRoleAssignment: makeEligible'
description: ロールの割り当てを有効にします。 呼び出し前に役割の割り当てが既に適用されている場合は、何も行われません。 役割の割り当てが永続的で、要求元がターゲットユーザーと異なる場合は、役割の割り当てが対象となり、その役割は対象ユーザーに対して無効になります。 リクエスターが対象ユーザーで、役割がセキュリティ管理者または特権の役割管理者である場合、役割は既定の有効期限を使用してアクティブ化されます。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 215d15709fc0225933ce171909aef3f70808be5d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361038"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="d5ade-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="d5ade-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5ade-107">ロールの割り当てを有効にします。</span><span class="sxs-lookup"><span data-stu-id="d5ade-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="d5ade-108">呼び出し前に役割の割り当てが既に適用されている場合は、何も行われません。</span><span class="sxs-lookup"><span data-stu-id="d5ade-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="d5ade-109">役割の割り当てが永続的で、要求元がターゲットユーザーと異なる場合は、役割の割り当てが対象となり、その役割は対象ユーザーに対して無効になります。</span><span class="sxs-lookup"><span data-stu-id="d5ade-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="d5ade-110">リクエスターが対象ユーザーで、役割がセキュリティ管理者または特権の役割管理者である場合、役割は既定の有効期限を使用してアクティブ化されます。</span><span class="sxs-lookup"><span data-stu-id="d5ade-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="d5ade-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5ade-111">Permissions</span></span>
<span data-ttu-id="d5ade-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5ade-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d5ade-114">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5ade-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="d5ade-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5ade-115">Permission type</span></span>      | <span data-ttu-id="d5ade-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5ade-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5ade-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5ade-117">Delegated (work or school account)</span></span> | <span data-ttu-id="d5ade-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5ade-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5ade-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5ade-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5ade-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5ade-120">Not supported.</span></span>    |
|<span data-ttu-id="d5ade-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5ade-121">Application</span></span> | <span data-ttu-id="d5ade-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5ade-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5ade-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5ade-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="d5ade-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5ade-124">Request headers</span></span>
| <span data-ttu-id="d5ade-125">名前</span><span class="sxs-lookup"><span data-stu-id="d5ade-125">Name</span></span>       | <span data-ttu-id="d5ade-126">説明</span><span class="sxs-lookup"><span data-stu-id="d5ade-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5ade-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5ade-127">Authorization</span></span>  | <span data-ttu-id="d5ade-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d5ade-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5ade-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5ade-130">Request body</span></span>
<span data-ttu-id="d5ade-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d5ade-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5ade-132">応答</span><span class="sxs-lookup"><span data-stu-id="d5ade-132">Response</span></span>

<span data-ttu-id="d5ade-133">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d5ade-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="d5ade-134">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d5ade-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d5ade-135">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="d5ade-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d5ade-136">例</span><span class="sxs-lookup"><span data-stu-id="d5ade-136">Example</span></span>
<span data-ttu-id="d5ade-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="d5ade-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="d5ade-138">要求</span><span class="sxs-lookup"><span data-stu-id="d5ade-138">Request</span></span>
<span data-ttu-id="d5ade-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5ade-139">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d5ade-140">プロトコル</span><span class="sxs-lookup"><span data-stu-id="d5ade-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d5ade-141">C#</span><span class="sxs-lookup"><span data-stu-id="d5ade-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makeeligible-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d5ade-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d5ade-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makeeligible-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d5ade-143">目的-C</span><span class="sxs-lookup"><span data-stu-id="d5ade-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makeeligible-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d5ade-144">Java</span><span class="sxs-lookup"><span data-stu-id="d5ade-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makeeligible-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d5ade-145">応答</span><span class="sxs-lookup"><span data-stu-id="d5ade-145">Response</span></span>
<span data-ttu-id="d5ade-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5ade-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
