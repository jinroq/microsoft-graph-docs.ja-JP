---
title: 'privilegedRole: selfDeactivate'
description: リクエスターに割り当てられているロールを非アクティブ化します。
localization_priority: Normal
ms.openlocfilehash: 1cf76b59252516f75290c361d5c54e85895848cc
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35264219"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="158b4-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="158b4-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="158b4-104">リクエスターに割り当てられているロールを非アクティブ化します。</span><span class="sxs-lookup"><span data-stu-id="158b4-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="158b4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="158b4-105">Permissions</span></span>
<span data-ttu-id="158b4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="158b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="158b4-108">リクエスターは、自分に```selfDeactivate```割り当てられている役割に対してのみ呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="158b4-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="158b4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="158b4-109">Permission type</span></span>      | <span data-ttu-id="158b4-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="158b4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="158b4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="158b4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="158b4-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="158b4-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="158b4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="158b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="158b4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="158b4-114">Not supported.</span></span>    |
|<span data-ttu-id="158b4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="158b4-115">Application</span></span> | <span data-ttu-id="158b4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="158b4-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="158b4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="158b4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="158b4-118">これは``<id>`` 、ターゲットの役割 id であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="158b4-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="158b4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="158b4-119">Request headers</span></span>
| <span data-ttu-id="158b4-120">名前</span><span class="sxs-lookup"><span data-stu-id="158b4-120">Name</span></span>       | <span data-ttu-id="158b4-121">説明</span><span class="sxs-lookup"><span data-stu-id="158b4-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="158b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="158b4-122">Authorization</span></span>  | <span data-ttu-id="158b4-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="158b4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="158b4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="158b4-125">Request body</span></span>
<span data-ttu-id="158b4-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="158b4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="158b4-127">応答</span><span class="sxs-lookup"><span data-stu-id="158b4-127">Response</span></span>

<span data-ttu-id="158b4-128">成功した場合、この`200 OK`メソッドは応答コードと、応答本文で[privilegedRoleAssignment](../resources/privilegedroleassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="158b4-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="158b4-129">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="158b4-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="158b4-130">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="158b4-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="158b4-131">例</span><span class="sxs-lookup"><span data-stu-id="158b4-131">Example</span></span>
<span data-ttu-id="158b4-132">以下は、この API を呼び出す方法の例です。</span><span class="sxs-lookup"><span data-stu-id="158b4-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="158b4-133">要求</span><span class="sxs-lookup"><span data-stu-id="158b4-133">Request</span></span>
<span data-ttu-id="158b4-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="158b4-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="158b4-135">応答</span><span class="sxs-lookup"><span data-stu-id="158b4-135">Response</span></span>
<span data-ttu-id="158b4-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="158b4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="158b4-139">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="158b4-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="158b4-140">C#</span><span class="sxs-lookup"><span data-stu-id="158b4-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/privilegedrole_selfdeactivate-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="158b4-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="158b4-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/privilegedrole_selfdeactivate-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="158b4-142">目的-C</span><span class="sxs-lookup"><span data-stu-id="158b4-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/privilegedrole_selfdeactivate-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
