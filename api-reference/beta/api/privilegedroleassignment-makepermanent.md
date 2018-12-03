---
title: 'privilegedRoleAssignment: makePermanent'
description: として永続的な役割の割り当てを確認します。
ms.openlocfilehash: 06875fc62539598a5e1e806714fcae3d973ba29c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074164"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="e6f47-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="e6f47-103">privilegedRoleAssignment: makePermanent</span></span>

> <span data-ttu-id="e6f47-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e6f47-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e6f47-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6f47-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e6f47-106">として永続的な役割の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="e6f47-106">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="e6f47-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e6f47-107">Permissions</span></span>
<span data-ttu-id="e6f47-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e6f47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e6f47-110">テナントは、PIM に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6f47-110">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e6f47-111">それ以外の場合、HTTP 403 アクセス不可のエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="e6f47-111">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="e6f47-112">リクエスターでは、_ロールの権限を持つ管理者_のロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e6f47-112">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="e6f47-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e6f47-113">Permission type</span></span>      | <span data-ttu-id="e6f47-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e6f47-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6f47-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e6f47-115">Delegated (work or school account)</span></span> | <span data-ttu-id="e6f47-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6f47-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6f47-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e6f47-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6f47-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6f47-118">Not supported.</span></span>    |
|<span data-ttu-id="e6f47-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e6f47-119">Application</span></span> | <span data-ttu-id="e6f47-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e6f47-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6f47-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e6f47-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="e6f47-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e6f47-122">Request headers</span></span>
| <span data-ttu-id="e6f47-123">名前</span><span class="sxs-lookup"><span data-stu-id="e6f47-123">Name</span></span>       | <span data-ttu-id="e6f47-124">説明</span><span class="sxs-lookup"><span data-stu-id="e6f47-124">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e6f47-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6f47-125">Authorization</span></span>  | <span data-ttu-id="e6f47-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="e6f47-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e6f47-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="e6f47-128">Request body</span></span>
<span data-ttu-id="e6f47-129">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e6f47-129">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="e6f47-130">パラメーター</span><span class="sxs-lookup"><span data-stu-id="e6f47-130">Parameter</span></span>    | <span data-ttu-id="e6f47-131">型</span><span class="sxs-lookup"><span data-stu-id="e6f47-131">Type</span></span>   |<span data-ttu-id="e6f47-132">説明</span><span class="sxs-lookup"><span data-stu-id="e6f47-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e6f47-133">理由</span><span class="sxs-lookup"><span data-stu-id="e6f47-133">reason</span></span>|<span data-ttu-id="e6f47-134">文字列</span><span class="sxs-lookup"><span data-stu-id="e6f47-134">string</span></span>|<span data-ttu-id="e6f47-135">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e6f47-135">Optional.</span></span> <span data-ttu-id="e6f47-136">この呼び出しを実行する理由です。</span><span class="sxs-lookup"><span data-stu-id="e6f47-136">The reason to make this call.</span></span>|
|<span data-ttu-id="e6f47-137">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="e6f47-137">ticketNumber</span></span>|<span data-ttu-id="e6f47-138">文字列</span><span class="sxs-lookup"><span data-stu-id="e6f47-138">string</span></span>|<span data-ttu-id="e6f47-139">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e6f47-139">Optional.</span></span> <span data-ttu-id="e6f47-140">このアクションに関連付けられているチケットの数です。</span><span class="sxs-lookup"><span data-stu-id="e6f47-140">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="e6f47-141">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="e6f47-141">ticketSystem</span></span>|<span data-ttu-id="e6f47-142">文字列</span><span class="sxs-lookup"><span data-stu-id="e6f47-142">string</span></span>|<span data-ttu-id="e6f47-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="e6f47-143">Optional.</span></span> <span data-ttu-id="e6f47-144">チケット システムです。</span><span class="sxs-lookup"><span data-stu-id="e6f47-144">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="e6f47-145">応答</span><span class="sxs-lookup"><span data-stu-id="e6f47-145">Response</span></span>

<span data-ttu-id="e6f47-146">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e6f47-146">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e6f47-147">例</span><span class="sxs-lookup"><span data-stu-id="e6f47-147">Example</span></span>
<span data-ttu-id="e6f47-148">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="e6f47-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="e6f47-149">要求</span><span class="sxs-lookup"><span data-stu-id="e6f47-149">Request</span></span>
<span data-ttu-id="e6f47-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e6f47-150">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="e6f47-151">応答</span><span class="sxs-lookup"><span data-stu-id="e6f47-151">Response</span></span>
<span data-ttu-id="e6f47-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e6f47-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: makePermanent",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->