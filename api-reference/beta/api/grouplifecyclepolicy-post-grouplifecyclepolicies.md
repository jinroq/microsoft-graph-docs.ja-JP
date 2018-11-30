---
title: Create groupLifecyclePolicy
description: 新しい groupLifecyclePolicy を作成します。
ms.openlocfilehash: ee7b4665f68bbbfeae268d7f86c10fa433c46cd3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073754"
---
# <a name="create-grouplifecyclepolicy"></a><span data-ttu-id="08424-103">Create groupLifecyclePolicy</span><span class="sxs-lookup"><span data-stu-id="08424-103">Create groupLifecyclePolicy</span></span>

> <span data-ttu-id="08424-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="08424-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08424-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08424-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08424-106">新しい [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) を作成します。</span><span class="sxs-lookup"><span data-stu-id="08424-106">Creates a new [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="08424-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08424-107">Permissions</span></span>

<span data-ttu-id="08424-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08424-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="08424-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08424-110">Permission type</span></span>      | <span data-ttu-id="08424-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08424-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08424-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08424-112">Delegated (work or school account)</span></span> | <span data-ttu-id="08424-113">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08424-113">Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="08424-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08424-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08424-115">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="08424-115">Not supported</span></span> |
|<span data-ttu-id="08424-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08424-116">Application</span></span> |  <span data-ttu-id="08424-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08424-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="08424-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08424-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groupLifecyclePolicies

```

## <a name="request-headers"></a><span data-ttu-id="08424-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08424-119">Request headers</span></span>

| <span data-ttu-id="08424-120">名前</span><span class="sxs-lookup"><span data-stu-id="08424-120">Name</span></span> | <span data-ttu-id="08424-121">説明</span><span class="sxs-lookup"><span data-stu-id="08424-121">Description</span></span> |
|:---------------|:----------|
| <span data-ttu-id="08424-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08424-122">Authorization</span></span> | <span data-ttu-id="08424-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="08424-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="08424-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="08424-125">Content-Type</span></span>  | <span data-ttu-id="08424-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08424-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="08424-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="08424-127">Request body</span></span>
<span data-ttu-id="08424-128">要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="08424-128">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="08424-129">応答</span><span class="sxs-lookup"><span data-stu-id="08424-129">Response</span></span>

<span data-ttu-id="08424-130">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="08424-130">If successful, this method returns `201 Created` response code and [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08424-131">例</span><span class="sxs-lookup"><span data-stu-id="08424-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08424-132">要求</span><span class="sxs-lookup"><span data-stu-id="08424-132">Request</span></span>

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
<span data-ttu-id="08424-133">要求本文で、[groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="08424-133">In the request body, supply a JSON representation of [groupLifecyclePolicy](../resources/grouplifecyclepolicy.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="08424-134">応答</span><span class="sxs-lookup"><span data-stu-id="08424-134">Response</span></span>

<span data-ttu-id="08424-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08424-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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