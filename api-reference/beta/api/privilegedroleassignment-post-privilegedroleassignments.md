---
title: PrivilegedRoleAssignment を作成します。
description: この API を使用すると、新しい privilegedRoleAssignment を作成します。
localization_priority: Normal
ms.openlocfilehash: 5522956b129eae8a19fd00b0e70b41380dbdd25e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513404"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="d5d73-103">PrivilegedRoleAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5d73-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d5d73-104">この API を使用すると、新しい[privilegedRoleAssignment](../resources/privilegedroleassignment.md)を作成します。</span><span class="sxs-lookup"><span data-stu-id="d5d73-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="d5d73-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d5d73-105">Permissions</span></span>
<span data-ttu-id="d5d73-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5d73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d5d73-108">リクエスターでは、_ロールの権限を持つ管理者_のロールを持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5d73-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="d5d73-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d5d73-109">Permission type</span></span>      | <span data-ttu-id="d5d73-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d5d73-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d5d73-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d5d73-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d5d73-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d5d73-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d5d73-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d5d73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d5d73-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5d73-114">Not supported.</span></span>    |
|<span data-ttu-id="d5d73-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d5d73-115">Application</span></span> | <span data-ttu-id="d5d73-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d5d73-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d5d73-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d5d73-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="d5d73-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d5d73-118">Request headers</span></span>
| <span data-ttu-id="d5d73-119">名前</span><span class="sxs-lookup"><span data-stu-id="d5d73-119">Name</span></span>       | <span data-ttu-id="d5d73-120">説明</span><span class="sxs-lookup"><span data-stu-id="d5d73-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d5d73-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5d73-121">Authorization</span></span>  | <span data-ttu-id="d5d73-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d5d73-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d5d73-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="d5d73-124">Request body</span></span>
<span data-ttu-id="d5d73-125">要求の本文には、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5d73-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d5d73-126">応答</span><span class="sxs-lookup"><span data-stu-id="d5d73-126">Response</span></span>

<span data-ttu-id="d5d73-127">かどうかは成功すると、このメソッドを返します`201 Created`、応答の本体で応答コードと[privilegedRoleAssignment](../resources/privilegedroleassignment.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d5d73-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="d5d73-128">テナントの PIM を登録する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d5d73-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d5d73-129">それ以外の場合、HTTP 403 アクセス不可の状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="d5d73-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d5d73-130">例</span><span class="sxs-lookup"><span data-stu-id="d5d73-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d5d73-131">要求</span><span class="sxs-lookup"><span data-stu-id="d5d73-131">Request</span></span>
<span data-ttu-id="d5d73-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d5d73-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
<span data-ttu-id="d5d73-133">要求の本文には、 [privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="d5d73-133">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d5d73-134">応答</span><span class="sxs-lookup"><span data-stu-id="d5d73-134">Response</span></span>
<span data-ttu-id="d5d73-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d5d73-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
