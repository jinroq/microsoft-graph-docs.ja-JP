---
title: 'privilegedRoleAssignment: makeEligible'
description: 対象となるように、役割の割り当てを確認します。 ロールの割り当ては、呼び出しの前に対象が既にいる場合は、何も行われません。 ロールの割り当ては、永続的なリクエスターは、ターゲットのユーザーと異なる場合は、ロールの割り当てができるようになり、ロールはターゲット ユーザーの非アクティブ化します。 リクエスターは、ターゲット ユーザーと役割は、セキュリティ管理者、またはロールの権限を持つ管理者を既定の有効期限を持つロールがアクティブになります。
localization_priority: Normal
ms.openlocfilehash: 54260da3f69819a1f7a351e072f8af851f0e3d3a
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527237"
---
# <a name="privilegedroleassignment-makeeligible"></a><span data-ttu-id="cab78-106">privilegedRoleAssignment: makeEligible</span><span class="sxs-lookup"><span data-stu-id="cab78-106">privilegedRoleAssignment: makeEligible</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cab78-107">対象となるように、役割の割り当てを確認します。</span><span class="sxs-lookup"><span data-stu-id="cab78-107">Make the role assignment as eligible.</span></span> <span data-ttu-id="cab78-108">ロールの割り当ては、呼び出しの前に対象が既にいる場合は、何も行われません。</span><span class="sxs-lookup"><span data-stu-id="cab78-108">If the role assignment is already eligible before the call, it does nothing.</span></span> <span data-ttu-id="cab78-109">ロールの割り当ては、永続的なリクエスターは、ターゲットのユーザーと異なる場合は、ロールの割り当てができるようになり、ロールはターゲット ユーザーの非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="cab78-109">If the role assignment is permanent and the requestor is different from the target user, the role assignment will become eligible and the role will be deactivated for the target user.</span></span> <span data-ttu-id="cab78-110">リクエスターは、ターゲット ユーザーと役割は、セキュリティ管理者、またはロールの権限を持つ管理者を既定の有効期限を持つロールがアクティブになります。</span><span class="sxs-lookup"><span data-stu-id="cab78-110">If the requestor is the target user and the role is Security Administrator or Privileged Role Administrator, the role will be activated with the default expiration.</span></span>

## <a name="permissions"></a><span data-ttu-id="cab78-111">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="cab78-111">Permissions</span></span>
<span data-ttu-id="cab78-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cab78-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="cab78-114">リクエスターでは、_ロールの権限を持つ管理者_のロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cab78-114">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="cab78-115">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cab78-115">Permission type</span></span>      | <span data-ttu-id="cab78-116">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="cab78-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cab78-117">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cab78-117">Delegated (work or school account)</span></span> | <span data-ttu-id="cab78-118">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cab78-118">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cab78-119">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cab78-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cab78-120">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cab78-120">Not supported.</span></span>    |
|<span data-ttu-id="cab78-121">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cab78-121">Application</span></span> | <span data-ttu-id="cab78-122">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cab78-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cab78-123">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cab78-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments/{id}/makeEligible
```
## <a name="request-headers"></a><span data-ttu-id="cab78-124">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cab78-124">Request headers</span></span>
| <span data-ttu-id="cab78-125">名前</span><span class="sxs-lookup"><span data-stu-id="cab78-125">Name</span></span>       | <span data-ttu-id="cab78-126">説明</span><span class="sxs-lookup"><span data-stu-id="cab78-126">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cab78-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="cab78-127">Authorization</span></span>  | <span data-ttu-id="cab78-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="cab78-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cab78-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="cab78-130">Request body</span></span>
<span data-ttu-id="cab78-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cab78-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cab78-132">応答</span><span class="sxs-lookup"><span data-stu-id="cab78-132">Response</span></span>

<span data-ttu-id="cab78-133">かどうかは成功すると、このメソッドを返します`200 OK`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="cab78-133">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="cab78-134">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="cab78-134">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cab78-135">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="cab78-135">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="cab78-136">例</span><span class="sxs-lookup"><span data-stu-id="cab78-136">Example</span></span>
<span data-ttu-id="cab78-137">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="cab78-137">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="cab78-138">要求</span><span class="sxs-lookup"><span data-stu-id="cab78-138">Request</span></span>
<span data-ttu-id="cab78-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cab78-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_makeeligible"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments/{id}/makeEligible
```

##### <a name="response"></a><span data-ttu-id="cab78-140">応答</span><span class="sxs-lookup"><span data-stu-id="cab78-140">Response</span></span>
<span data-ttu-id="cab78-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cab78-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/privilegedroleassignment-makeeligible.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
