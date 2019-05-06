---
title: 'privilegedRoleAssignment: makePermanent'
description: ロールの割り当てを永続的にします。
localization_priority: Normal
ms.openlocfilehash: 3a3c6956546a88bebea5ce023f8f0e490894a2b1
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33594395"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="2edfa-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="2edfa-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2edfa-104">ロールの割り当てを永続的にします。</span><span class="sxs-lookup"><span data-stu-id="2edfa-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="2edfa-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2edfa-105">Permissions</span></span>
<span data-ttu-id="2edfa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2edfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2edfa-108">テナントは PIM に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2edfa-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2edfa-109">それ以外の場合、HTTP 403 禁止のエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="2edfa-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="2edfa-110">リクエスターは、特権の_役割管理者_の役割を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2edfa-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="2edfa-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2edfa-111">Permission type</span></span>      | <span data-ttu-id="2edfa-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2edfa-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2edfa-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2edfa-113">Delegated (work or school account)</span></span> | <span data-ttu-id="2edfa-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2edfa-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2edfa-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2edfa-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2edfa-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2edfa-116">Not supported.</span></span>    |
|<span data-ttu-id="2edfa-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2edfa-117">Application</span></span> | <span data-ttu-id="2edfa-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2edfa-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2edfa-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2edfa-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="2edfa-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2edfa-120">Request headers</span></span>
| <span data-ttu-id="2edfa-121">名前</span><span class="sxs-lookup"><span data-stu-id="2edfa-121">Name</span></span>       | <span data-ttu-id="2edfa-122">説明</span><span class="sxs-lookup"><span data-stu-id="2edfa-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2edfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2edfa-123">Authorization</span></span>  | <span data-ttu-id="2edfa-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2edfa-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2edfa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2edfa-126">Request body</span></span>
<span data-ttu-id="2edfa-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2edfa-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2edfa-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2edfa-128">Parameter</span></span>    | <span data-ttu-id="2edfa-129">型</span><span class="sxs-lookup"><span data-stu-id="2edfa-129">Type</span></span>   |<span data-ttu-id="2edfa-130">説明</span><span class="sxs-lookup"><span data-stu-id="2edfa-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2edfa-131">したがっ</span><span class="sxs-lookup"><span data-stu-id="2edfa-131">reason</span></span>|<span data-ttu-id="2edfa-132">string</span><span class="sxs-lookup"><span data-stu-id="2edfa-132">string</span></span>|<span data-ttu-id="2edfa-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2edfa-133">Optional.</span></span> <span data-ttu-id="2edfa-134">この呼び出しを行う理由。</span><span class="sxs-lookup"><span data-stu-id="2edfa-134">The reason to make this call.</span></span>|
|<span data-ttu-id="2edfa-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="2edfa-135">ticketNumber</span></span>|<span data-ttu-id="2edfa-136">string</span><span class="sxs-lookup"><span data-stu-id="2edfa-136">string</span></span>|<span data-ttu-id="2edfa-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2edfa-137">Optional.</span></span> <span data-ttu-id="2edfa-138">このアクションに関連付けられているチケット番号。</span><span class="sxs-lookup"><span data-stu-id="2edfa-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="2edfa-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="2edfa-139">ticketSystem</span></span>|<span data-ttu-id="2edfa-140">string</span><span class="sxs-lookup"><span data-stu-id="2edfa-140">string</span></span>|<span data-ttu-id="2edfa-141">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2edfa-141">Optional.</span></span> <span data-ttu-id="2edfa-142">チケットシステム。</span><span class="sxs-lookup"><span data-stu-id="2edfa-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="2edfa-143">応答</span><span class="sxs-lookup"><span data-stu-id="2edfa-143">Response</span></span>

<span data-ttu-id="2edfa-144">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2edfa-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2edfa-145">例</span><span class="sxs-lookup"><span data-stu-id="2edfa-145">Example</span></span>
<span data-ttu-id="2edfa-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="2edfa-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2edfa-147">要求</span><span class="sxs-lookup"><span data-stu-id="2edfa-147">Request</span></span>
<span data-ttu-id="2edfa-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2edfa-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2edfa-149">応答</span><span class="sxs-lookup"><span data-stu-id="2edfa-149">Response</span></span>
<span data-ttu-id="2edfa-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2edfa-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="2edfa-153">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="2edfa-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="2edfa-154">Visual</span><span class="sxs-lookup"><span data-stu-id="2edfa-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_makepermanent-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2edfa-155">Java</span><span class="sxs-lookup"><span data-stu-id="2edfa-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedroleassignment_makepermanent-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
