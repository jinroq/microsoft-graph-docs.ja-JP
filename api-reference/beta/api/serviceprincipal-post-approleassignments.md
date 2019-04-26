---
title: appRoleAssignment を作成する
description: この API を使用して、新しい approleassignment を作成します。
localization_priority: Normal
ms.openlocfilehash: cb171e4d6149de5ba169dbf7ad48e87cb055fb47
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335813"
---
# <a name="create-approleassignment"></a><span data-ttu-id="2cc8d-103">appRoleAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="2cc8d-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2cc8d-104">この API を使用して、新しい approleassignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="2cc8d-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2cc8d-105">Permissions</span></span>
<span data-ttu-id="2cc8d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cc8d-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2cc8d-108">Permission type</span></span>      | <span data-ttu-id="2cc8d-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2cc8d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2cc8d-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2cc8d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2cc8d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2cc8d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2cc8d-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2cc8d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2cc8d-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-113">Not supported.</span></span>    |
|<span data-ttu-id="2cc8d-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2cc8d-114">Application</span></span> | <span data-ttu-id="2cc8d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2cc8d-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2cc8d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="2cc8d-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2cc8d-117">Request headers</span></span>
| <span data-ttu-id="2cc8d-118">名前</span><span class="sxs-lookup"><span data-stu-id="2cc8d-118">Name</span></span>       | <span data-ttu-id="2cc8d-119">型</span><span class="sxs-lookup"><span data-stu-id="2cc8d-119">Type</span></span> | <span data-ttu-id="2cc8d-120">説明</span><span class="sxs-lookup"><span data-stu-id="2cc8d-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="2cc8d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cc8d-121">Authorization</span></span>  | <span data-ttu-id="2cc8d-122">string</span><span class="sxs-lookup"><span data-stu-id="2cc8d-122">string</span></span>  | <span data-ttu-id="2cc8d-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2cc8d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2cc8d-125">Request body</span></span>
<span data-ttu-id="2cc8d-126">要求本文で、 [approleassignment](../resources/approleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="2cc8d-127">応答</span><span class="sxs-lookup"><span data-stu-id="2cc8d-127">Response</span></span>

<span data-ttu-id="2cc8d-128">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[approleassignment](../resources/approleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2cc8d-129">例</span><span class="sxs-lookup"><span data-stu-id="2cc8d-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2cc8d-130">要求</span><span class="sxs-lookup"><span data-stu-id="2cc8d-130">Request</span></span>
<span data-ttu-id="2cc8d-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="2cc8d-132">要求本文で、 [approleassignment](../resources/approleassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-132">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="2cc8d-133">応答</span><span class="sxs-lookup"><span data-stu-id="2cc8d-133">Response</span></span>
<span data-ttu-id="2cc8d-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2cc8d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
