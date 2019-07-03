---
title: Create groupLifecyclePolicy
description: 新しい groupLifecyclePolicy を作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f022be2e393f10805e9d62c49a6dbfd8333d93e2
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35442609"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="48412-103">Create groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="48412-103">Create groupLifecyclePolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="48412-104">新しい [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="48412-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="48412-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="48412-105">Permissions</span></span>

<span data-ttu-id="48412-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="48412-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="48412-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="48412-108">Permission type</span></span>      | <span data-ttu-id="48412-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="48412-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="48412-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="48412-110">Delegated (work or school account)</span></span> | <span data-ttu-id="48412-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48412-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="48412-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="48412-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="48412-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="48412-113">Not supported</span></span> |
|<span data-ttu-id="48412-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="48412-114">Application</span></span> |  <span data-ttu-id="48412-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48412-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="48412-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="48412-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="48412-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="48412-117">Request headers</span></span>

| <span data-ttu-id="48412-118">名前</span><span class="sxs-lookup"><span data-stu-id="48412-118">Name</span></span> | <span data-ttu-id="48412-119">説明</span><span class="sxs-lookup"><span data-stu-id="48412-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="48412-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="48412-120">Authorization</span></span> | <span data-ttu-id="48412-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="48412-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="48412-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="48412-123">Content-Type</span></span>  | <span data-ttu-id="48412-124">application/json</span><span class="sxs-lookup"><span data-stu-id="48412-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="48412-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="48412-125">Request body</span></span>
<span data-ttu-id="48412-126">要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="48412-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="48412-127">応答</span><span class="sxs-lookup"><span data-stu-id="48412-127">Response</span></span>

<span data-ttu-id="48412-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="48412-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48412-129">例</span><span class="sxs-lookup"><span data-stu-id="48412-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="48412-130">要求</span><span class="sxs-lookup"><span data-stu-id="48412-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="48412-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="48412-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="48412-132">C#</span><span class="sxs-lookup"><span data-stu-id="48412-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-grouplifecyclepolicy-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="48412-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="48412-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-grouplifecyclepolicy-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="48412-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="48412-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-grouplifecyclepolicy-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="48412-135">要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="48412-135">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="48412-136">応答</span><span class="sxs-lookup"><span data-stu-id="48412-136">Response</span></span>

<span data-ttu-id="48412-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="48412-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.groupLifecyclePolicy"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 174

{
  "id": "ffffffff-ffff-ffff-ffff-ffffffffffff",
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
