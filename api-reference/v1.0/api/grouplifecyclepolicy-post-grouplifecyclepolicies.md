---
title: Create groupLifecyclePolicy
description: 新しい groupLifecyclePolicy を作成します。
author: dkershaw10
ms.openlocfilehash: 7161a99fb1ad7a9f27ca4d88746c4b3da1400ef4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331277"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="3d4ef-103">Create groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="3d4ef-103">Create groupLifecyclePolicy</span></span>

<span data-ttu-id="3d4ef-104">新しい [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="3d4ef-104">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3d4ef-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3d4ef-105">Permissions</span></span>

<span data-ttu-id="3d4ef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3d4ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d4ef-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3d4ef-108">Permission type</span></span>      | <span data-ttu-id="3d4ef-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3d4ef-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d4ef-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3d4ef-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d4ef-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4ef-111">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d4ef-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3d4ef-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d4ef-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3d4ef-113">Not supported.</span></span>    |
|<span data-ttu-id="3d4ef-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3d4ef-114">Application</span></span> | <span data-ttu-id="3d4ef-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d4ef-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3d4ef-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3d4ef-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="3d4ef-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3d4ef-117">Request headers</span></span>

| <span data-ttu-id="3d4ef-118">名前</span><span class="sxs-lookup"><span data-stu-id="3d4ef-118">Name</span></span> | <span data-ttu-id="3d4ef-119">説明</span><span class="sxs-lookup"><span data-stu-id="3d4ef-119">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="3d4ef-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d4ef-120">Authorization</span></span> | <span data-ttu-id="3d4ef-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3d4ef-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3d4ef-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3d4ef-123">Content-Type</span></span>  | <span data-ttu-id="3d4ef-124">application/json</span><span class="sxs-lookup"><span data-stu-id="3d4ef-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3d4ef-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="3d4ef-125">Request body</span></span>
<span data-ttu-id="3d4ef-126">要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d4ef-126">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="3d4ef-127">応答</span><span class="sxs-lookup"><span data-stu-id="3d4ef-127">Response</span></span>

<span data-ttu-id="3d4ef-128">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3d4ef-128">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d4ef-129">例</span><span class="sxs-lookup"><span data-stu-id="3d4ef-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="3d4ef-130">要求</span><span class="sxs-lookup"><span data-stu-id="3d4ef-130">Request</span></span>

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
<span data-ttu-id="3d4ef-131">要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3d4ef-131">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="3d4ef-132">応答</span><span class="sxs-lookup"><span data-stu-id="3d4ef-132">Response</span></span>

<span data-ttu-id="3d4ef-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3d4ef-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create groupLifecyclePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->