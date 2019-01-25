---
title: 'privilegedRoleAssignment: makePermanent'
description: として永続的な役割の割り当てを確認します。
localization_priority: Normal
ms.openlocfilehash: 9c6334662cf8496262b49b14ceb3f51f7a4f8dbc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511395"
---
# <a name="privilegedroleassignment-makepermanent"></a><span data-ttu-id="393ee-103">privilegedRoleAssignment: makePermanent</span><span class="sxs-lookup"><span data-stu-id="393ee-103">privilegedRoleAssignment: makePermanent</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="393ee-104">として永続的な役割の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="393ee-104">Make the role assignment as permanent.</span></span>

## <a name="permissions"></a><span data-ttu-id="393ee-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="393ee-105">Permissions</span></span>
<span data-ttu-id="393ee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="393ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="393ee-108">テナントは、PIM に登録する必要があります。</span><span class="sxs-lookup"><span data-stu-id="393ee-108">The tenant needs to be registered to PIM.</span></span> <span data-ttu-id="393ee-109">それ以外の場合、HTTP 403 アクセス不可のエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="393ee-109">Otherwise, HTTP 403 Forbidden error will be returned.</span></span>

<span data-ttu-id="393ee-110">リクエスターでは、_ロールの権限を持つ管理者_のロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="393ee-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="393ee-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="393ee-111">Permission type</span></span>      | <span data-ttu-id="393ee-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="393ee-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="393ee-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="393ee-113">Delegated (work or school account)</span></span> | <span data-ttu-id="393ee-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="393ee-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="393ee-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="393ee-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="393ee-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="393ee-116">Not supported.</span></span>    |
|<span data-ttu-id="393ee-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="393ee-117">Application</span></span> | <span data-ttu-id="393ee-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="393ee-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="393ee-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="393ee-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makePermanent
```
## <a name="request-headers"></a><span data-ttu-id="393ee-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="393ee-120">Request headers</span></span>
| <span data-ttu-id="393ee-121">名前</span><span class="sxs-lookup"><span data-stu-id="393ee-121">Name</span></span>       | <span data-ttu-id="393ee-122">説明</span><span class="sxs-lookup"><span data-stu-id="393ee-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="393ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="393ee-123">Authorization</span></span>  | <span data-ttu-id="393ee-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="393ee-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="393ee-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="393ee-126">Request body</span></span>
<span data-ttu-id="393ee-127">要求本文で、次のパラメーターを含む JSON オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="393ee-127">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="393ee-128">パラメーター</span><span class="sxs-lookup"><span data-stu-id="393ee-128">Parameter</span></span>    | <span data-ttu-id="393ee-129">型</span><span class="sxs-lookup"><span data-stu-id="393ee-129">Type</span></span>   |<span data-ttu-id="393ee-130">説明</span><span class="sxs-lookup"><span data-stu-id="393ee-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="393ee-131">理由</span><span class="sxs-lookup"><span data-stu-id="393ee-131">reason</span></span>|<span data-ttu-id="393ee-132">string</span><span class="sxs-lookup"><span data-stu-id="393ee-132">string</span></span>|<span data-ttu-id="393ee-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="393ee-133">Optional.</span></span> <span data-ttu-id="393ee-134">この呼び出しを実行する理由です。</span><span class="sxs-lookup"><span data-stu-id="393ee-134">The reason to make this call.</span></span>|
|<span data-ttu-id="393ee-135">ticketNumber</span><span class="sxs-lookup"><span data-stu-id="393ee-135">ticketNumber</span></span>|<span data-ttu-id="393ee-136">string</span><span class="sxs-lookup"><span data-stu-id="393ee-136">string</span></span>|<span data-ttu-id="393ee-137">省略可能。</span><span class="sxs-lookup"><span data-stu-id="393ee-137">Optional.</span></span> <span data-ttu-id="393ee-138">このアクションに関連付けられているチケットの数です。</span><span class="sxs-lookup"><span data-stu-id="393ee-138">The ticket number that is associated with this action.</span></span>|
|<span data-ttu-id="393ee-139">ticketSystem</span><span class="sxs-lookup"><span data-stu-id="393ee-139">ticketSystem</span></span>|<span data-ttu-id="393ee-140">string</span><span class="sxs-lookup"><span data-stu-id="393ee-140">string</span></span>|<span data-ttu-id="393ee-141">省略可能。</span><span class="sxs-lookup"><span data-stu-id="393ee-141">Optional.</span></span> <span data-ttu-id="393ee-142">チケット システムです。</span><span class="sxs-lookup"><span data-stu-id="393ee-142">The ticket system.</span></span>|

## <a name="response"></a><span data-ttu-id="393ee-143">応答</span><span class="sxs-lookup"><span data-stu-id="393ee-143">Response</span></span>

<span data-ttu-id="393ee-144">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="393ee-144">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="393ee-145">例</span><span class="sxs-lookup"><span data-stu-id="393ee-145">Example</span></span>
<span data-ttu-id="393ee-146">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="393ee-146">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="393ee-147">要求</span><span class="sxs-lookup"><span data-stu-id="393ee-147">Request</span></span>
<span data-ttu-id="393ee-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="393ee-148">Here is an example of the request.</span></span>
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

##### <a name="response"></a><span data-ttu-id="393ee-149">応答</span><span class="sxs-lookup"><span data-stu-id="393ee-149">Response</span></span>
<span data-ttu-id="393ee-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="393ee-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedroleassignment-makepermanent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
