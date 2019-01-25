---
title: 'privilegedRole: selfActivate'
description: 依頼者に割り当てられているロールをアクティブにします。
localization_priority: Normal
ms.openlocfilehash: e0197599373246853906b879c0f3d13e61a45244
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29515070"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="6089d-103">privilegedRole: selfActivate</span><span class="sxs-lookup"><span data-stu-id="6089d-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6089d-104">依頼者に割り当てられているロールをアクティブにします。</span><span class="sxs-lookup"><span data-stu-id="6089d-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="6089d-105">**注:** 2018年 12 月の効果的なこの API は、サポートされていない、使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6089d-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="6089d-106">[PrivilegedRoleAssignmentRequest の作成](privilegedroleassignmentrequest-post.md)を使用してください。</span><span class="sxs-lookup"><span data-stu-id="6089d-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="6089d-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6089d-107">Permissions</span></span>
<span data-ttu-id="6089d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6089d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6089d-110">リクエスターは呼び出すことができますのみ```selfActivate```彼に割り当てられているロールです。</span><span class="sxs-lookup"><span data-stu-id="6089d-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="6089d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6089d-111">Permission type</span></span>      | <span data-ttu-id="6089d-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6089d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6089d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6089d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6089d-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6089d-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6089d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6089d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6089d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6089d-116">Not supported.</span></span>    |
|<span data-ttu-id="6089d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6089d-117">Application</span></span> | <span data-ttu-id="6089d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6089d-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6089d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6089d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="6089d-120">注意してください``<id>``は、ターゲットのロールの id。</span><span class="sxs-lookup"><span data-stu-id="6089d-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6089d-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6089d-121">Request headers</span></span>
| <span data-ttu-id="6089d-122">名前</span><span class="sxs-lookup"><span data-stu-id="6089d-122">Name</span></span>       | <span data-ttu-id="6089d-123">説明</span><span class="sxs-lookup"><span data-stu-id="6089d-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6089d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="6089d-124">Authorization</span></span>  | <span data-ttu-id="6089d-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6089d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6089d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6089d-127">Request body</span></span>
<span data-ttu-id="6089d-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6089d-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6089d-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="6089d-129">Parameter</span></span>    | <span data-ttu-id="6089d-130">型</span><span class="sxs-lookup"><span data-stu-id="6089d-130">Type</span></span>   |<span data-ttu-id="6089d-131">説明</span><span class="sxs-lookup"><span data-stu-id="6089d-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6089d-132">理由</span><span class="sxs-lookup"><span data-stu-id="6089d-132">reason</span></span>|<span data-ttu-id="6089d-133">string</span><span class="sxs-lookup"><span data-stu-id="6089d-133">string</span></span>|<span data-ttu-id="6089d-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6089d-134">Optional.</span></span> <span data-ttu-id="6089d-135">このロールのアクティブ化の理由について説明します。</span><span class="sxs-lookup"><span data-stu-id="6089d-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="6089d-136">duration</span><span class="sxs-lookup"><span data-stu-id="6089d-136">duration</span></span>|<span data-ttu-id="6089d-137">string</span><span class="sxs-lookup"><span data-stu-id="6089d-137">string</span></span>|<span data-ttu-id="6089d-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6089d-138">Optional.</span></span> <span data-ttu-id="6089d-139">有効な値である可能性があります```min```(最低限のライセンス認証の期間)、 ```default``` (アクティブ化の既定の期間、ロール)、または時間数は、ライセンス認証の手続きを指定する double 型の値です。</span><span class="sxs-lookup"><span data-stu-id="6089d-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="6089d-140">指定した期間をロールの設定をロールのアクティブ化の期間よりも長いことはできません。</span><span class="sxs-lookup"><span data-stu-id="6089d-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="6089d-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="6089d-141">ticketNumber</span></span>|<span data-ttu-id="6089d-142">string</span><span class="sxs-lookup"><span data-stu-id="6089d-142">string</span></span>|<span data-ttu-id="6089d-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6089d-143">Optional.</span></span> <span data-ttu-id="6089d-144">このロールのアクティブ化の追跡に使用されるチケットの数です。</span><span class="sxs-lookup"><span data-stu-id="6089d-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="6089d-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="6089d-145">ticketSystem</span></span>|<span data-ttu-id="6089d-146">string</span><span class="sxs-lookup"><span data-stu-id="6089d-146">string</span></span>|<span data-ttu-id="6089d-147">省略可能。</span><span class="sxs-lookup"><span data-stu-id="6089d-147">Optional.</span></span> <span data-ttu-id="6089d-148">チケット システムです。</span><span class="sxs-lookup"><span data-stu-id="6089d-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="6089d-149">応答</span><span class="sxs-lookup"><span data-stu-id="6089d-149">Response</span></span>

<span data-ttu-id="6089d-150">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6089d-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="6089d-151">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6089d-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6089d-152">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="6089d-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6089d-153">例</span><span class="sxs-lookup"><span data-stu-id="6089d-153">Example</span></span>
<span data-ttu-id="6089d-154">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="6089d-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6089d-155">要求</span><span class="sxs-lookup"><span data-stu-id="6089d-155">Request</span></span>
<span data-ttu-id="6089d-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6089d-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="6089d-157">応答</span><span class="sxs-lookup"><span data-stu-id="6089d-157">Response</span></span>
<span data-ttu-id="6089d-158">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6089d-158">Here is an example of the response.</span></span> 

><span data-ttu-id="6089d-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="6089d-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedrole-selfactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
