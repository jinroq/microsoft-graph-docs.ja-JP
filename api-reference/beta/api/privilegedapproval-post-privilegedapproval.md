---
title: privilegedApproval を作成する
description: この API を使用して、新しい privilegedApproval を作成します。
localization_priority: Normal
ms.openlocfilehash: 25f11589304ddaf1d5e2fc21bb787b17fab4f1fa
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35268174"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="d7b65-103">privilegedApproval を作成する</span><span class="sxs-lookup"><span data-stu-id="d7b65-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7b65-104">この API を使用して、新しい privilegedApproval を作成します。</span><span class="sxs-lookup"><span data-stu-id="d7b65-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="d7b65-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="d7b65-105">Permissions</span></span>
<span data-ttu-id="d7b65-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7b65-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d7b65-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d7b65-108">Permission type</span></span>      | <span data-ttu-id="d7b65-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="d7b65-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7b65-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d7b65-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d7b65-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d7b65-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d7b65-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d7b65-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d7b65-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b65-113">Not supported.</span></span>    |
|<span data-ttu-id="d7b65-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d7b65-114">Application</span></span> | <span data-ttu-id="d7b65-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d7b65-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d7b65-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d7b65-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="d7b65-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d7b65-117">Request headers</span></span>
| <span data-ttu-id="d7b65-118">名前</span><span class="sxs-lookup"><span data-stu-id="d7b65-118">Name</span></span>       | <span data-ttu-id="d7b65-119">説明</span><span class="sxs-lookup"><span data-stu-id="d7b65-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="d7b65-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7b65-120">Authorization</span></span>  | <span data-ttu-id="d7b65-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="d7b65-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d7b65-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d7b65-123">Request body</span></span>
<span data-ttu-id="d7b65-124">要求本文で、 [privilegedApproval](../resources/privilegedapproval.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d7b65-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d7b65-125">応答</span><span class="sxs-lookup"><span data-stu-id="d7b65-125">Response</span></span>

<span data-ttu-id="d7b65-126">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[privilegedApproval](../resources/privilegedapproval.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d7b65-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="d7b65-127">テナントが PIM に登録されている必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d7b65-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d7b65-128">それ以外の場合、HTTP 403 の禁止状態コードが返されます。</span><span class="sxs-lookup"><span data-stu-id="d7b65-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="d7b65-129">例</span><span class="sxs-lookup"><span data-stu-id="d7b65-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d7b65-130">要求</span><span class="sxs-lookup"><span data-stu-id="d7b65-130">Request</span></span>
<span data-ttu-id="d7b65-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d7b65-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
<span data-ttu-id="d7b65-132">要求本文で、 [privilegedApproval](../resources/privilegedapproval.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d7b65-132">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d7b65-133">応答</span><span class="sxs-lookup"><span data-stu-id="d7b65-133">Response</span></span>
<span data-ttu-id="d7b65-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d7b65-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d7b65-137">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="d7b65-137">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d7b65-138">C#</span><span class="sxs-lookup"><span data-stu-id="d7b65-138">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_privilegedapproval_from_privilegedapproval-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d7b65-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="d7b65-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_privilegedapproval_from_privilegedapproval-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d7b65-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="d7b65-140">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_privilegedapproval_from_privilegedapproval-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/privilegedapproval-post-privilegedapproval.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
