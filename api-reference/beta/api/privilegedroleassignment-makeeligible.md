---
title: 'privilegedRoleAssignment: makeEligible'
description: 対象となるように、役割の割り当てを確認します。 ロールの割り当ては、呼び出しの前に対象が既にいる場合は、何も行われません。 ロールの割り当ては、永続的なリクエスターは、ターゲットのユーザーと異なる場合は、ロールの割り当てができるようになり、ロールはターゲット ユーザーの非アクティブ化します。 リクエスターは、ターゲット ユーザーと役割は、セキュリティ管理者、またはロールの権限を持つ管理者を既定の有効期限を持つロールがアクティブになります。
ms.openlocfilehash: f39f508c7aeae4d85db92b43f406cd3497533e38
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067111"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="6c79c-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="6c79c-106">privilegedRoleAssignment: makeEligible</span></span>

> <span data-ttu-id="6c79c-107">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c79c-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c79c-108">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c79c-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c79c-109">対象となるように、役割の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="6c79c-109">Make the role assignment as eligible.</span></span> <span data-ttu-id="6c79c-110">ロールの割り当ては、呼び出しの前に対象が既にいる場合は、何も行われません。</span><span class="sxs-lookup"><span data-stu-id="6c79c-110">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="6c79c-111">ロールの割り当ては、永続的なリクエスターは、ターゲットのユーザーと異なる場合は、ロールの割り当てができるようになり、ロールはターゲット ユーザーの非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="6c79c-111">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="6c79c-112">リクエスターは、ターゲット ユーザーと役割は、セキュリティ管理者、またはロールの権限を持つ管理者を既定の有効期限を持つロールがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="6c79c-112">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c79c-113">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6c79c-113">Permissions</span></span>
<span data-ttu-id="6c79c-p104">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c79c-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6c79c-116">リクエスターでは、_ロールの権限を持つ管理者_のロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c79c-116">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="6c79c-117">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c79c-117">Permission type</span></span>      | <span data-ttu-id="6c79c-118">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c79c-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6c79c-119">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c79c-119">Delegated (work or school account)</span></span> | <span data-ttu-id="6c79c-120">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6c79c-120">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6c79c-121">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c79c-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c79c-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c79c-122">Not supported.</span></span>    |
|<span data-ttu-id="6c79c-123">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c79c-123">Application</span></span> | <span data-ttu-id="6c79c-124">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c79c-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c79c-125">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c79c-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="6c79c-126">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c79c-126">Request headers</span></span>
| <span data-ttu-id="6c79c-127">名前</span><span class="sxs-lookup"><span data-stu-id="6c79c-127">Name</span></span>       | <span data-ttu-id="6c79c-128">説明</span><span class="sxs-lookup"><span data-stu-id="6c79c-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6c79c-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c79c-129">Authorization</span></span>  | <span data-ttu-id="6c79c-p105">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6c79c-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c79c-132">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c79c-132">Request body</span></span>
<span data-ttu-id="6c79c-133">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6c79c-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c79c-134">応答</span><span class="sxs-lookup"><span data-stu-id="6c79c-134">Response</span></span>

<span data-ttu-id="6c79c-135">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6c79c-135">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="6c79c-136">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="6c79c-136">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6c79c-137">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="6c79c-137">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6c79c-138">例</span><span class="sxs-lookup"><span data-stu-id="6c79c-138">Example</span></span>
<span data-ttu-id="6c79c-139">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="6c79c-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="6c79c-140">要求</span><span class="sxs-lookup"><span data-stu-id="6c79c-140">Request</span></span>
<span data-ttu-id="6c79c-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c79c-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="6c79c-142">応答</span><span class="sxs-lookup"><span data-stu-id="6c79c-142">Response</span></span>
<span data-ttu-id="6c79c-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6c79c-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedRoleAssignment: makeEligible",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->