---
title: 生徒を追加する
description: クラスにメンバーを追加します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d368b67f16440cb54cb5f1d7ec306e7db7150662
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259774"
---
# <a name="add-a-student"></a><span data-ttu-id="9fe54-103">生徒を追加する</span><span class="sxs-lookup"><span data-stu-id="9fe54-103">Add a student</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fe54-104">クラスにメンバーを追加します。</span><span class="sxs-lookup"><span data-stu-id="9fe54-104">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fe54-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9fe54-105">Permissions</span></span>
<span data-ttu-id="9fe54-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9fe54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9fe54-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9fe54-108">Permission type</span></span>      | <span data-ttu-id="9fe54-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9fe54-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fe54-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9fe54-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="9fe54-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fe54-111">Not supported.</span></span>  |
|<span data-ttu-id="9fe54-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9fe54-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="9fe54-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9fe54-113">Not supported.</span></span>  |
|<span data-ttu-id="9fe54-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9fe54-114">Application</span></span> | <span data-ttu-id="9fe54-115">Eduroster.readbasic の正の値を取得します。</span><span class="sxs-lookup"><span data-stu-id="9fe54-115">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="9fe54-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9fe54-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="9fe54-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9fe54-117">Request headers</span></span>
| <span data-ttu-id="9fe54-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9fe54-118">Header</span></span>       | <span data-ttu-id="9fe54-119">値</span><span class="sxs-lookup"><span data-stu-id="9fe54-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="9fe54-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fe54-120">Authorization</span></span>  | <span data-ttu-id="9fe54-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="9fe54-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="9fe54-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="9fe54-123">Content-Type</span></span>  | <span data-ttu-id="9fe54-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9fe54-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="9fe54-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9fe54-125">Request body</span></span>
<span data-ttu-id="9fe54-126">要求本文で、[educationUser](../resources/educationuser.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9fe54-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="9fe54-127">応答</span><span class="sxs-lookup"><span data-stu-id="9fe54-127">Response</span></span>
<span data-ttu-id="9fe54-128">成功した場合、このメソッドは `204 No Content` 応答コードと、応答本文で [educationClass](../resources/educationclass.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9fe54-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fe54-129">例</span><span class="sxs-lookup"><span data-stu-id="9fe54-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9fe54-130">要求</span><span class="sxs-lookup"><span data-stu-id="9fe54-130">Request</span></span>
<span data-ttu-id="9fe54-131">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9fe54-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="9fe54-132">応答</span><span class="sxs-lookup"><span data-stu-id="9fe54-132">Response</span></span>
<span data-ttu-id="9fe54-133">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9fe54-133">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="9fe54-134">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="9fe54-134">SDK sample code</span></span>

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9fe54-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="9fe54-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationclass-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="9fe54-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="9fe54-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_educationuser_from_educationclass-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationclass-post-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationclass-post-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
