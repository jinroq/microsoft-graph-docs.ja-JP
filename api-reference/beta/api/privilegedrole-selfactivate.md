---
title: 'privilegedRole: selfActivate'
description: 要求者に割り当てられている役割をアクティブ化します。
localization_priority: Normal
ms.openlocfilehash: f2a8db8b56af011be1f5a07c02b730da1faa242c
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35445024"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="b598c-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="b598c-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b598c-104">要求者に割り当てられている役割をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="b598c-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="b598c-105">**注:** 2018年12月有効になると、この API はサポートされなくなり、使用されなくなります。</span><span class="sxs-lookup"><span data-stu-id="b598c-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="b598c-106">代わりに、 [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="b598c-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="b598c-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="b598c-107">Permissions</span></span>
<span data-ttu-id="b598c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b598c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b598c-110">リクエスターは、自分に```selfActivate```割り当てられている役割に対してのみ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="b598c-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="b598c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b598c-111">Permission type</span></span>      | <span data-ttu-id="b598c-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="b598c-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b598c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b598c-113">Delegated (work or school account)</span></span> | <span data-ttu-id="b598c-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b598c-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b598c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b598c-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b598c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b598c-116">Not supported.</span></span>    |
|<span data-ttu-id="b598c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b598c-117">Application</span></span> | <span data-ttu-id="b598c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b598c-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b598c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b598c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="b598c-120">これは``<id>`` 、ターゲットの役割 ID であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b598c-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="b598c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b598c-121">Request headers</span></span>
| <span data-ttu-id="b598c-122">名前</span><span class="sxs-lookup"><span data-stu-id="b598c-122">Name</span></span>       | <span data-ttu-id="b598c-123">説明</span><span class="sxs-lookup"><span data-stu-id="b598c-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b598c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b598c-124">Authorization</span></span>  | <span data-ttu-id="b598c-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="b598c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b598c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="b598c-127">Request body</span></span>
<span data-ttu-id="b598c-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="b598c-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="b598c-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="b598c-129">Parameter</span></span>    | <span data-ttu-id="b598c-130">型</span><span class="sxs-lookup"><span data-stu-id="b598c-130">Type</span></span>   |<span data-ttu-id="b598c-131">説明</span><span class="sxs-lookup"><span data-stu-id="b598c-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b598c-132">したがっ</span><span class="sxs-lookup"><span data-stu-id="b598c-132">reason</span></span>|<span data-ttu-id="b598c-133">string</span><span class="sxs-lookup"><span data-stu-id="b598c-133">string</span></span>|<span data-ttu-id="b598c-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b598c-134">Optional.</span></span> <span data-ttu-id="b598c-135">この役割のライセンス認証の理由についての説明。</span><span class="sxs-lookup"><span data-stu-id="b598c-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="b598c-136">duration</span><span class="sxs-lookup"><span data-stu-id="b598c-136">duration</span></span>|<span data-ttu-id="b598c-137">string</span><span class="sxs-lookup"><span data-stu-id="b598c-137">string</span></span>|<span data-ttu-id="b598c-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b598c-138">Optional.</span></span> <span data-ttu-id="b598c-139">有効な値は```min``` 、(最小ライセンス認証の```default```期間)、(ロールの既定のライセンス認証の期間)、または倍精度の値を使用してライセンス認証の時間数を指定します。</span><span class="sxs-lookup"><span data-stu-id="b598c-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="b598c-140">指定した期間は、役割の設定から、役割のアクティブ化の期間より長くすることはできません。</span><span class="sxs-lookup"><span data-stu-id="b598c-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="b598c-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="b598c-141">ticketNumber</span></span>|<span data-ttu-id="b598c-142">string</span><span class="sxs-lookup"><span data-stu-id="b598c-142">string</span></span>|<span data-ttu-id="b598c-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b598c-143">Optional.</span></span> <span data-ttu-id="b598c-144">この役割のライセンス認証の追跡に使用されるチケット番号。</span><span class="sxs-lookup"><span data-stu-id="b598c-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="b598c-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="b598c-145">ticketSystem</span></span>|<span data-ttu-id="b598c-146">string</span><span class="sxs-lookup"><span data-stu-id="b598c-146">string</span></span>|<span data-ttu-id="b598c-147">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b598c-147">Optional.</span></span> <span data-ttu-id="b598c-148">チケットシステム。</span><span class="sxs-lookup"><span data-stu-id="b598c-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="b598c-149">応答</span><span class="sxs-lookup"><span data-stu-id="b598c-149">Response</span></span>

<span data-ttu-id="b598c-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b598c-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="b598c-151">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b598c-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b598c-152">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="b598c-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="b598c-153">例</span><span class="sxs-lookup"><span data-stu-id="b598c-153">Example</span></span>
<span data-ttu-id="b598c-154">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="b598c-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="b598c-155">要求</span><span class="sxs-lookup"><span data-stu-id="b598c-155">Request</span></span>
<span data-ttu-id="b598c-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b598c-156">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b598c-157">プロトコル</span><span class="sxs-lookup"><span data-stu-id="b598c-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfActivate
Content-type: application/json
Content-length: 142

{
  "reason": "reason-value",
  "duration": "duration-value",
  "ticketNumber": "ticketNumber-value",
  "ticketSystem": "ticketSystem-value"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b598c-158">C#</span><span class="sxs-lookup"><span data-stu-id="b598c-158">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedrole-selfactivate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b598c-159">Javascript</span><span class="sxs-lookup"><span data-stu-id="b598c-159">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedrole-selfactivate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b598c-160">目的-C</span><span class="sxs-lookup"><span data-stu-id="b598c-160">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedrole-selfactivate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b598c-161">応答</span><span class="sxs-lookup"><span data-stu-id="b598c-161">Response</span></span>
<span data-ttu-id="b598c-162">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="b598c-162">Here is an example of the response.</span></span> 

><span data-ttu-id="b598c-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="b598c-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
