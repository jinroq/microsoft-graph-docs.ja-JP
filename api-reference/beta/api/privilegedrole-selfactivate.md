---
title: 'privilegedRole: selfActivate'
description: 依頼者に割り当てられているロールをアクティブにします。
localization_priority: Normal
ms.openlocfilehash: 9423d87714fcd4a7b7cce1dd5cd03bcef3e0ef9f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872129"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="2310c-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="2310c-103">privilegedRole: selfActivate</span></span>

><span data-ttu-id="2310c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2310c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2310c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2310c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2310c-106">依頼者に割り当てられているロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="2310c-106">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="2310c-107">**注:** 2018年 12 月の効果的なこの API は、サポートされていない、使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="2310c-107">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="2310c-108">[PrivilegedRoleAssignmentRequest の作成](privilegedroleassignmentrequest-post.md)を使用してください。</span><span class="sxs-lookup"><span data-stu-id="2310c-108">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="2310c-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2310c-109">Permissions</span></span>
<span data-ttu-id="2310c-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2310c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2310c-112">リクエスターは呼び出すことができますのみ```selfActivate```彼に割り当てられているロールです。</span><span class="sxs-lookup"><span data-stu-id="2310c-112">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="2310c-113">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2310c-113">Permission type</span></span>      | <span data-ttu-id="2310c-114">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2310c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2310c-115">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2310c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2310c-116">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2310c-116">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2310c-117">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2310c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2310c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2310c-118">Not supported.</span></span>    |
|<span data-ttu-id="2310c-119">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2310c-119">Application</span></span> | <span data-ttu-id="2310c-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2310c-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2310c-121">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2310c-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="2310c-122">注意してください``<id>``は、ターゲットのロールの id。</span><span class="sxs-lookup"><span data-stu-id="2310c-122">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="2310c-123">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2310c-123">Request headers</span></span>
| <span data-ttu-id="2310c-124">名前</span><span class="sxs-lookup"><span data-stu-id="2310c-124">Name</span></span>       | <span data-ttu-id="2310c-125">説明</span><span class="sxs-lookup"><span data-stu-id="2310c-125">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2310c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="2310c-126">Authorization</span></span>  | <span data-ttu-id="2310c-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2310c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2310c-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="2310c-129">Request body</span></span>
<span data-ttu-id="2310c-130">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2310c-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2310c-131">パラメーター</span><span class="sxs-lookup"><span data-stu-id="2310c-131">Parameter</span></span>    | <span data-ttu-id="2310c-132">Type</span><span class="sxs-lookup"><span data-stu-id="2310c-132">Type</span></span>   |<span data-ttu-id="2310c-133">説明</span><span class="sxs-lookup"><span data-stu-id="2310c-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2310c-134">理由</span><span class="sxs-lookup"><span data-stu-id="2310c-134">reason</span></span>|<span data-ttu-id="2310c-135">文字列</span><span class="sxs-lookup"><span data-stu-id="2310c-135">string</span></span>|<span data-ttu-id="2310c-136">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2310c-136">Optional.</span></span> <span data-ttu-id="2310c-137">このロールのアクティブ化の理由について説明します。</span><span class="sxs-lookup"><span data-stu-id="2310c-137">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="2310c-138">duration</span><span class="sxs-lookup"><span data-stu-id="2310c-138">duration</span></span>|<span data-ttu-id="2310c-139">文字列</span><span class="sxs-lookup"><span data-stu-id="2310c-139">string</span></span>|<span data-ttu-id="2310c-140">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2310c-140">Optional.</span></span> <span data-ttu-id="2310c-141">有効な値である可能性があります```min```(最低限のライセンス認証の期間)、 ```default``` (アクティブ化の既定の期間、ロール)、または時間数は、ライセンス認証の手続きを指定する double 型の値です。</span><span class="sxs-lookup"><span data-stu-id="2310c-141">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="2310c-142">指定した期間をロールの設定をロールのアクティブ化の期間よりも長いことはできません。</span><span class="sxs-lookup"><span data-stu-id="2310c-142">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="2310c-143">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="2310c-143">ticketNumber</span></span>|<span data-ttu-id="2310c-144">文字列</span><span class="sxs-lookup"><span data-stu-id="2310c-144">string</span></span>|<span data-ttu-id="2310c-145">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2310c-145">Optional.</span></span> <span data-ttu-id="2310c-146">このロールのアクティブ化の追跡に使用されるチケットの数です。</span><span class="sxs-lookup"><span data-stu-id="2310c-146">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="2310c-147">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="2310c-147">ticketSystem</span></span>|<span data-ttu-id="2310c-148">文字列</span><span class="sxs-lookup"><span data-stu-id="2310c-148">string</span></span>|<span data-ttu-id="2310c-149">省略可能。</span><span class="sxs-lookup"><span data-stu-id="2310c-149">Optional.</span></span> <span data-ttu-id="2310c-150">チケット システムです。</span><span class="sxs-lookup"><span data-stu-id="2310c-150">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="2310c-151">応答</span><span class="sxs-lookup"><span data-stu-id="2310c-151">Response</span></span>

<span data-ttu-id="2310c-152">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="2310c-152">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="2310c-153">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="2310c-153">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="2310c-154">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="2310c-154">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="2310c-155">例</span><span class="sxs-lookup"><span data-stu-id="2310c-155">Example</span></span>
<span data-ttu-id="2310c-156">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2310c-156">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2310c-157">要求</span><span class="sxs-lookup"><span data-stu-id="2310c-157">Request</span></span>
<span data-ttu-id="2310c-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2310c-158">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="2310c-159">応答</span><span class="sxs-lookup"><span data-stu-id="2310c-159">Response</span></span>
<span data-ttu-id="2310c-160">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="2310c-160">Here is an example of the response.</span></span> 

><span data-ttu-id="2310c-p110">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="2310c-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRole: selfActivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
