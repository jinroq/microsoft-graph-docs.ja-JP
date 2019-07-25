---
title: securityAction を作成する
description: 新しい securityAction オブジェクトを作成します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 96f0c5b9ffbcdcda125cb43421fdcffc617c89ea
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35870251"
---
# <a name="create-securityaction"></a><span data-ttu-id="587b8-103">securityAction を作成する</span><span class="sxs-lookup"><span data-stu-id="587b8-103">Create securityAction</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="587b8-104">新しい[securityAction](../resources/securityaction.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="587b8-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="587b8-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="587b8-105">Permissions</span></span>

<span data-ttu-id="587b8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="587b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="587b8-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="587b8-108">Permission type</span></span>                        | <span data-ttu-id="587b8-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="587b8-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="587b8-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="587b8-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="587b8-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="587b8-111">Not supported.</span></span> |
| <span data-ttu-id="587b8-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="587b8-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="587b8-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="587b8-113">Not supported.</span></span> |
| <span data-ttu-id="587b8-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="587b8-114">Application</span></span>                            | <span data-ttu-id="587b8-115">SecurityActions.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="587b8-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="587b8-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="587b8-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="587b8-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="587b8-117">Request headers</span></span>

| <span data-ttu-id="587b8-118">名前</span><span class="sxs-lookup"><span data-stu-id="587b8-118">Name</span></span>          | <span data-ttu-id="587b8-119">説明</span><span class="sxs-lookup"><span data-stu-id="587b8-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="587b8-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="587b8-120">Authorization</span></span> | <span data-ttu-id="587b8-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="587b8-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="587b8-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="587b8-122">Request body</span></span>

<span data-ttu-id="587b8-123">要求本文で、 [securityAction](../resources/securityaction.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="587b8-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="587b8-124">応答</span><span class="sxs-lookup"><span data-stu-id="587b8-124">Response</span></span>

<span data-ttu-id="587b8-125">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[securityAction](../resources/securityaction.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="587b8-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="587b8-126">例</span><span class="sxs-lookup"><span data-stu-id="587b8-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="587b8-127">要求</span><span class="sxs-lookup"><span data-stu-id="587b8-127">Request</span></span>

<span data-ttu-id="587b8-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="587b8-128">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="587b8-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="587b8-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_securityaction_from_security"
}-->

```http
POST https://graph.microsoft.com/beta/security/securityActions
Content-type: application/json

{
  "name": "BlockIp",
  "actionReason": "Test",
  "parameters": [
    {
      "name": "IP",
      "value": "1.2.3.4"
    }
  ],
  "vendorInformation": {
    "provider": "Windows Defender ATP",
    "vendor": "Microsoft"
  }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="587b8-130">C#</span><span class="sxs-lookup"><span data-stu-id="587b8-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-securityaction-from-security-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="587b8-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="587b8-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-securityaction-from-security-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="587b8-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="587b8-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-securityaction-from-security-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="587b8-133">Java</span><span class="sxs-lookup"><span data-stu-id="587b8-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-securityaction-from-security-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="587b8-134">応答</span><span class="sxs-lookup"><span data-stu-id="587b8-134">Response</span></span>

<span data-ttu-id="587b8-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="587b8-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="587b8-136">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="587b8-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="587b8-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="587b8-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id" : "1234567890",
    "status" : "notStarted",
    "createdDateTime": "2019-01-10 12:23:23.33333",
    "lastActionDateTime": "2019-01-10 12:23:23.33333",
    "name": "blockIp",
    "actionReason": "Test",
    "errorInfo": null,
    "vendorInformation": {
        "provider": "Windows Defender ATP",
        "providerVersion": null,
        "subProvider": null,
        "vendor": "Microsoft"
    },
    "parameters": [
        {
            "name": "IP",
            "value": "1.2.3.4"
        }
    ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
