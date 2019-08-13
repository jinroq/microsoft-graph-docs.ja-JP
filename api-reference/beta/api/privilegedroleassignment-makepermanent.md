---
title: 'privilegedRoleAssignment: makePermanent'
description: ロールの割り当てを永続的にします。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 7b1db98c98c1da5268b4019c20a3a1fe04851c74
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361066"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="0cdfb-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="0cdfb-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cdfb-104">ロールの割り当てを永続的にします。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="0cdfb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0cdfb-105">Permissions</span></span>
<span data-ttu-id="0cdfb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0cdfb-108">テナントは PIM に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="0cdfb-109">それ以外の場合、HTTP 403 禁止のエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="0cdfb-110">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="0cdfb-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0cdfb-111">Permission type</span></span>      | <span data-ttu-id="0cdfb-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0cdfb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0cdfb-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0cdfb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0cdfb-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0cdfb-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0cdfb-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0cdfb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0cdfb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-116">Not supported.</span></span>    |
|<span data-ttu-id="0cdfb-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0cdfb-117">Application</span></span> | <span data-ttu-id="0cdfb-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0cdfb-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0cdfb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="0cdfb-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0cdfb-120">Request headers</span></span>
| <span data-ttu-id="0cdfb-121">名前</span><span class="sxs-lookup"><span data-stu-id="0cdfb-121">Name</span></span>       | <span data-ttu-id="0cdfb-122">説明</span><span class="sxs-lookup"><span data-stu-id="0cdfb-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0cdfb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cdfb-123">Authorization</span></span>  | <span data-ttu-id="0cdfb-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0cdfb-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0cdfb-126">Request body</span></span>
<span data-ttu-id="0cdfb-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="0cdfb-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="0cdfb-128">Parameter</span></span>    | <span data-ttu-id="0cdfb-129">型</span><span class="sxs-lookup"><span data-stu-id="0cdfb-129">Type</span></span>   |<span data-ttu-id="0cdfb-130">説明</span><span class="sxs-lookup"><span data-stu-id="0cdfb-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cdfb-131">したがっ</span><span class="sxs-lookup"><span data-stu-id="0cdfb-131">reason</span></span>|<span data-ttu-id="0cdfb-132">string</span><span class="sxs-lookup"><span data-stu-id="0cdfb-132">string</span></span>|<span data-ttu-id="0cdfb-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-133">Optional.</span></span> <span data-ttu-id="0cdfb-134">この呼び出しを行う理由。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-134">The reason to make this call.</span></span>|
|<span data-ttu-id="0cdfb-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="0cdfb-135">ticketNumber</span></span>|<span data-ttu-id="0cdfb-136">string</span><span class="sxs-lookup"><span data-stu-id="0cdfb-136">string</span></span>|<span data-ttu-id="0cdfb-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-137">Optional.</span></span> <span data-ttu-id="0cdfb-138">このアクションに関連付けられているチケット番号。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="0cdfb-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="0cdfb-139">ticketSystem</span></span>|<span data-ttu-id="0cdfb-140">string</span><span class="sxs-lookup"><span data-stu-id="0cdfb-140">string</span></span>|<span data-ttu-id="0cdfb-141">省略可能。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-141">Optional.</span></span> <span data-ttu-id="0cdfb-142">チケットシステム。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="0cdfb-143">応答</span><span class="sxs-lookup"><span data-stu-id="0cdfb-143">Response</span></span>

<span data-ttu-id="0cdfb-144">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cdfb-145">例</span><span class="sxs-lookup"><span data-stu-id="0cdfb-145">Example</span></span>
<span data-ttu-id="0cdfb-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0cdfb-147">要求</span><span class="sxs-lookup"><span data-stu-id="0cdfb-147">Request</span></span>
<span data-ttu-id="0cdfb-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-148">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0cdfb-149">プロトコル</span><span class="sxs-lookup"><span data-stu-id="0cdfb-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makepermanent"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makePermanent
Content-type: application/json
Content-length: 110

{
  "reason": "reason-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0cdfb-150">C#</span><span class="sxs-lookup"><span data-stu-id="0cdfb-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-makepermanent-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0cdfb-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0cdfb-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-makepermanent-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0cdfb-152">目的-C</span><span class="sxs-lookup"><span data-stu-id="0cdfb-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-makepermanent-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="0cdfb-153">Java</span><span class="sxs-lookup"><span data-stu-id="0cdfb-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedroleassignment-makepermanent-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="0cdfb-154">応答</span><span class="sxs-lookup"><span data-stu-id="0cdfb-154">Response</span></span>
<span data-ttu-id="0cdfb-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0cdfb-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
