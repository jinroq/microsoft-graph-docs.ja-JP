---
title: セキュリティアクションの作成
description: 新しいセキュリティアクションオブジェクトを作成します。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: e1958f80219234fcae54220491629a921dd8bcfd
ms.sourcegitcommit: 88ddd033de0f36eedade277d57c922ebd0db5bba
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/02/2019
ms.locfileid: "30366890"
---
# <a name="create-security-action"></a><span data-ttu-id="161b5-103">セキュリティアクションの作成</span><span class="sxs-lookup"><span data-stu-id="161b5-103">Create security action</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="161b5-104">新しい[securityAction](../resources/securityaction.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="161b5-104">Create a new [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="161b5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="161b5-105">Permissions</span></span>

<span data-ttu-id="161b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="161b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="161b5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="161b5-108">Permission type</span></span>                        | <span data-ttu-id="161b5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="161b5-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="161b5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="161b5-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="161b5-111">securityactions</span><span class="sxs-lookup"><span data-stu-id="161b5-111">SecurityActions.ReadWrite.All</span></span> |
| <span data-ttu-id="161b5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="161b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="161b5-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="161b5-113">Not supported.</span></span> |
| <span data-ttu-id="161b5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="161b5-114">Application</span></span>                            | <span data-ttu-id="161b5-115">securityactions</span><span class="sxs-lookup"><span data-stu-id="161b5-115">SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="161b5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="161b5-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /security/securityActions
```

## <a name="request-headers"></a><span data-ttu-id="161b5-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="161b5-117">Request headers</span></span>

| <span data-ttu-id="161b5-118">名前</span><span class="sxs-lookup"><span data-stu-id="161b5-118">Name</span></span>          | <span data-ttu-id="161b5-119">説明</span><span class="sxs-lookup"><span data-stu-id="161b5-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="161b5-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="161b5-120">Authorization</span></span> | <span data-ttu-id="161b5-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="161b5-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="161b5-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="161b5-122">Request body</span></span>

<span data-ttu-id="161b5-123">要求本文で、 [securityAction](../resources/securityaction.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="161b5-123">In the request body, supply a JSON representation of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="161b5-124">応答</span><span class="sxs-lookup"><span data-stu-id="161b5-124">Response</span></span>

<span data-ttu-id="161b5-125">成功した場合、この`201 Created`メソッドは応答コードと、応答本文で[securityAction](../resources/securityaction.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="161b5-125">If successful, this method returns `201 Created` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="161b5-126">例</span><span class="sxs-lookup"><span data-stu-id="161b5-126">Examples</span></span>

### <a name="request"></a><span data-ttu-id="161b5-127">要求</span><span class="sxs-lookup"><span data-stu-id="161b5-127">Request</span></span>

<span data-ttu-id="161b5-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="161b5-128">The following is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="161b5-129">応答</span><span class="sxs-lookup"><span data-stu-id="161b5-129">Response</span></span>

<span data-ttu-id="161b5-130">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="161b5-130">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="161b5-131">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="161b5-131">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="161b5-132">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="161b5-132">All the properties will be returned from an actual call.</span></span>

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
  "tocPath": ""
}-->
