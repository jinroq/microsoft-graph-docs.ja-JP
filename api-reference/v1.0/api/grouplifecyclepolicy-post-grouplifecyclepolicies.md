---
title: Create groupLifecyclePolicy
description: 新しい groupLifecyclePolicy を作成します。
author: dkershaw10
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 7fe5f1dd57039611d4c0378a1ce568b71a22ca28
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33613406"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="0e2f5-103">Create groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="0e2f5-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="0e2f5-104">新しい [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="0e2f5-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0e2f5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="0e2f5-105">Permissions</span></span>

<span data-ttu-id="0e2f5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e2f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e2f5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0e2f5-108">Permission type</span></span>      | <span data-ttu-id="0e2f5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="0e2f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0e2f5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0e2f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0e2f5-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e2f5-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="0e2f5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0e2f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0e2f5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0e2f5-113">Not supported.</span></span>    |
|<span data-ttu-id="0e2f5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0e2f5-114">Application</span></span> | <span data-ttu-id="0e2f5-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e2f5-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0e2f5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0e2f5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="0e2f5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0e2f5-117">Request headers</span></span>

| <span data-ttu-id="0e2f5-118">名前</span><span class="sxs-lookup"><span data-stu-id="0e2f5-118">Name</span></span> | <span data-ttu-id="0e2f5-119">説明</span><span class="sxs-lookup"><span data-stu-id="0e2f5-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="0e2f5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0e2f5-120">Authorization</span></span> | <span data-ttu-id="0e2f5-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="0e2f5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0e2f5-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0e2f5-123">Content-Type</span></span>  | <span data-ttu-id="0e2f5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="0e2f5-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0e2f5-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="0e2f5-125">Request body</span></span>
<span data-ttu-id="0e2f5-126">要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0e2f5-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0e2f5-127">応答</span><span class="sxs-lookup"><span data-stu-id="0e2f5-127">Response</span></span>

<span data-ttu-id="0e2f5-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0e2f5-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e2f5-129">例</span><span class="sxs-lookup"><span data-stu-id="0e2f5-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0e2f5-130">要求</span><span class="sxs-lookup"><span data-stu-id="0e2f5-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_grouplifecyclepolicy_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/groupLifecyclePolicies
Content-type: application/json
Content-length: 125

{
  "groupLifetimeInDays": 100,
  "managedGroupTypes": "Selected",
  "alternateNotificationEmails": "admin@contoso.com"
}
```
<span data-ttu-id="0e2f5-131">要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0e2f5-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="0e2f5-132">応答</span><span class="sxs-lookup"><span data-stu-id="0e2f5-132">Response</span></span>

<span data-ttu-id="0e2f5-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0e2f5-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0e2f5-135">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="0e2f5-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0e2f5-136">Visual</span><span class="sxs-lookup"><span data-stu-id="0e2f5-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0e2f5-137">Java</span><span class="sxs-lookup"><span data-stu-id="0e2f5-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_grouplifecyclepolicy_from_group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/grouplifecyclepolicy-post-grouplifecyclepolicies.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
