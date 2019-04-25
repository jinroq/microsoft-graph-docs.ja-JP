---
title: 'privilegedRole: selfactivate'
description: 要求者に割り当てられている役割をアクティブ化します。
localization_priority: Normal
ms.openlocfilehash: e0197599373246853906b879c0f3d13e61a45244
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32546592"
---
# <a name="privilegedrole-selfactivate"></a><span data-ttu-id="c12de-103">privilegedRole: selfactivate</span><span class="sxs-lookup"><span data-stu-id="c12de-103">privilegedRole: selfActivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c12de-104">要求者に割り当てられている役割をアクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="c12de-104">Activate the role that is assigned to the requester.</span></span>

><span data-ttu-id="c12de-105">**注:** 2018年12月有効になると、この API はサポートされなくなり、使用されなくなります。</span><span class="sxs-lookup"><span data-stu-id="c12de-105">**Note:** Effective December 2018, this API will no longer be supported and should not be used.</span></span> <span data-ttu-id="c12de-106">代わりに、 [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md)を使用します。</span><span class="sxs-lookup"><span data-stu-id="c12de-106">Use the [Create PrivilegedRoleAssignmentRequest](privilegedroleassignmentrequest-post.md) instead.</span></span>


## <a name="permissions"></a><span data-ttu-id="c12de-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c12de-107">Permissions</span></span>
<span data-ttu-id="c12de-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c12de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c12de-110">リクエスターは、自分に```selfActivate```割り当てられている役割に対してのみ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="c12de-110">The requestor can only call ```selfActivate``` for the role that is assigned to him.</span></span>
 

|<span data-ttu-id="c12de-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c12de-111">Permission type</span></span>      | <span data-ttu-id="c12de-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c12de-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c12de-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c12de-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c12de-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c12de-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c12de-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c12de-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c12de-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c12de-116">Not supported.</span></span>    |
|<span data-ttu-id="c12de-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c12de-117">Application</span></span> | <span data-ttu-id="c12de-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c12de-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c12de-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c12de-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfActivate
```

<span data-ttu-id="c12de-120">これは``<id>`` 、ターゲットの役割 ID であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c12de-120">Note that ``<id>`` is the target role ID.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c12de-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c12de-121">Request headers</span></span>
| <span data-ttu-id="c12de-122">名前</span><span class="sxs-lookup"><span data-stu-id="c12de-122">Name</span></span>       | <span data-ttu-id="c12de-123">説明</span><span class="sxs-lookup"><span data-stu-id="c12de-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c12de-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c12de-124">Authorization</span></span>  | <span data-ttu-id="c12de-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="c12de-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c12de-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c12de-127">Request body</span></span>
<span data-ttu-id="c12de-128">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="c12de-128">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="c12de-129">パラメーター</span><span class="sxs-lookup"><span data-stu-id="c12de-129">Parameter</span></span>    | <span data-ttu-id="c12de-130">型</span><span class="sxs-lookup"><span data-stu-id="c12de-130">Type</span></span>   |<span data-ttu-id="c12de-131">説明</span><span class="sxs-lookup"><span data-stu-id="c12de-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c12de-132">したがっ</span><span class="sxs-lookup"><span data-stu-id="c12de-132">reason</span></span>|<span data-ttu-id="c12de-133">string</span><span class="sxs-lookup"><span data-stu-id="c12de-133">string</span></span>|<span data-ttu-id="c12de-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c12de-134">Optional.</span></span> <span data-ttu-id="c12de-135">この役割のライセンス認証の理由についての説明。</span><span class="sxs-lookup"><span data-stu-id="c12de-135">Description about the reason for this role activation.</span></span>|
|<span data-ttu-id="c12de-136">duration</span><span class="sxs-lookup"><span data-stu-id="c12de-136">duration</span></span>|<span data-ttu-id="c12de-137">string</span><span class="sxs-lookup"><span data-stu-id="c12de-137">string</span></span>|<span data-ttu-id="c12de-138">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c12de-138">Optional.</span></span> <span data-ttu-id="c12de-139">有効な値は```min``` 、(最小ライセンス認証の```default```期間)、(ロールの既定のライセンス認証の期間)、または倍精度の値を使用してライセンス認証の時間数を指定します。</span><span class="sxs-lookup"><span data-stu-id="c12de-139">Valid values could be ```min``` (minimal activation duration), ```default``` (default activation duration for the role), or a double value to specify how many hours is the activation.</span></span> <span data-ttu-id="c12de-140">指定した期間は、役割の設定から、役割のアクティブ化の期間より長くすることはできません。</span><span class="sxs-lookup"><span data-stu-id="c12de-140">The specified duration cannot be longer than the role's activation duration from the role setting.</span></span> |
|<span data-ttu-id="c12de-141">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="c12de-141">ticketNumber</span></span>|<span data-ttu-id="c12de-142">string</span><span class="sxs-lookup"><span data-stu-id="c12de-142">string</span></span>|<span data-ttu-id="c12de-143">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c12de-143">Optional.</span></span> <span data-ttu-id="c12de-144">この役割のライセンス認証の追跡に使用されるチケット番号。</span><span class="sxs-lookup"><span data-stu-id="c12de-144">The ticket number that is used to tracking this role activation.</span></span>|
|<span data-ttu-id="c12de-145">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="c12de-145">ticketSystem</span></span>|<span data-ttu-id="c12de-146">string</span><span class="sxs-lookup"><span data-stu-id="c12de-146">string</span></span>|<span data-ttu-id="c12de-147">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c12de-147">Optional.</span></span> <span data-ttu-id="c12de-148">チケットシステム。</span><span class="sxs-lookup"><span data-stu-id="c12de-148">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="c12de-149">応答</span><span class="sxs-lookup"><span data-stu-id="c12de-149">Response</span></span>

<span data-ttu-id="c12de-150">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c12de-150">If successful, this method returns a `200 OK` response code and a [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="c12de-151">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c12de-151">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="c12de-152">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="c12de-152">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="c12de-153">例</span><span class="sxs-lookup"><span data-stu-id="c12de-153">Example</span></span>
<span data-ttu-id="c12de-154">次の例は、この API を呼び出す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c12de-154">The following example shows how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c12de-155">要求</span><span class="sxs-lookup"><span data-stu-id="c12de-155">Request</span></span>
<span data-ttu-id="c12de-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c12de-156">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="c12de-157">応答</span><span class="sxs-lookup"><span data-stu-id="c12de-157">Response</span></span>
<span data-ttu-id="c12de-158">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="c12de-158">Here is an example of the response.</span></span> 

><span data-ttu-id="c12de-p109">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="c12de-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
