---
title: 'directoryDefinition: discover'
description: 'アプリケーションへのプロビジョニングに関する最新のスキーマ定義を検出します。 '
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bcdb7d9c0130183b16e6d7458ad9f2624ff9defb
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35931031"
---
# <a name="directorydefinition-discover"></a><span data-ttu-id="89dbb-103">directoryDefinition: discover</span><span class="sxs-lookup"><span data-stu-id="89dbb-103">directoryDefinition: discover</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89dbb-104">アプリケーションへのプロビジョニングに関する最新のスキーマ定義を検出します。</span><span class="sxs-lookup"><span data-stu-id="89dbb-104">Discover the latest schema definition for provisioning to an application.</span></span> 

## <a name="permissions"></a><span data-ttu-id="89dbb-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="89dbb-105">Permissions</span></span>

<span data-ttu-id="89dbb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="89dbb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89dbb-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="89dbb-108">Permission type</span></span>                        | <span data-ttu-id="89dbb-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="89dbb-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="89dbb-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="89dbb-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="89dbb-111">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89dbb-111">Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="89dbb-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="89dbb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89dbb-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="89dbb-113">Not supported.</span></span> |
| <span data-ttu-id="89dbb-114">アプリケーション専用</span><span class="sxs-lookup"><span data-stu-id="89dbb-114">Application-only</span></span>                            | <span data-ttu-id="89dbb-115">なし。</span><span class="sxs-lookup"><span data-stu-id="89dbb-115">None.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89dbb-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="89dbb-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```

## <a name="request-headers"></a><span data-ttu-id="89dbb-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89dbb-117">Request headers</span></span>

| <span data-ttu-id="89dbb-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="89dbb-118">Header</span></span>        | <span data-ttu-id="89dbb-119">値</span><span class="sxs-lookup"><span data-stu-id="89dbb-119">Value</span></span>                      |
|:--------------|:---------------------------|
| <span data-ttu-id="89dbb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="89dbb-120">Authorization</span></span> | <span data-ttu-id="89dbb-121">Bearer {トークン} (必須)</span><span class="sxs-lookup"><span data-stu-id="89dbb-121">Bearer {token} (required)</span></span>  |

## <a name="request-body"></a><span data-ttu-id="89dbb-122">要求本文</span><span class="sxs-lookup"><span data-stu-id="89dbb-122">Request body</span></span>

<span data-ttu-id="89dbb-123">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="89dbb-123">Do not supply a request body for this method.</span></span> 

## <a name="response"></a><span data-ttu-id="89dbb-124">応答</span><span class="sxs-lookup"><span data-stu-id="89dbb-124">Response</span></span>

<span data-ttu-id="89dbb-125">成功した場合、このメソッド`200 OK`は[directorydefinition](../resources/synchronization-directorydefinition.md)オブジェクトを持つ応答を返します。</span><span class="sxs-lookup"><span data-stu-id="89dbb-125">If successful, this method returns a `200 OK` response with a [directoryDefinition](../resources/synchronization-directorydefinition.md) object.</span></span>

## <a name="example"></a><span data-ttu-id="89dbb-126">例</span><span class="sxs-lookup"><span data-stu-id="89dbb-126">Example</span></span>

### <a name="request"></a><span data-ttu-id="89dbb-127">要求</span><span class="sxs-lookup"><span data-stu-id="89dbb-127">Request</span></span>
<span data-ttu-id="89dbb-128">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89dbb-128">The following is an example of a request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="89dbb-129">プロトコル</span><span class="sxs-lookup"><span data-stu-id="89dbb-129">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "discover_directorydefinition"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema/directories/{directoryId}/discover
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="89dbb-130">C#</span><span class="sxs-lookup"><span data-stu-id="89dbb-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/discover-directorydefinition-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="89dbb-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="89dbb-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/discover-directorydefinition-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="89dbb-132">目的-C</span><span class="sxs-lookup"><span data-stu-id="89dbb-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/discover-directorydefinition-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="89dbb-133">Java</span><span class="sxs-lookup"><span data-stu-id="89dbb-133">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/discover-directorydefinition-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89dbb-134">応答</span><span class="sxs-lookup"><span data-stu-id="89dbb-134">Response</span></span>

<span data-ttu-id="89dbb-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="89dbb-135">The following is an example of a response.</span></span>

><span data-ttu-id="89dbb-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="89dbb-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryDefinition"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "discoverabilities": "AttributeNames, AttributeDataTypes",
  "discoveryDateTime": "2019-03-20T15:47:50.4707552Z",
  "id": "directoryDefinitionId",
  "objects": [{
        "name": "User",
        "attributes": [{
                "name": "Id",
                "type": "String"
            }, {
                "name": "FirstName",
                "type": "String"
            },
            {
                "name": "CustomExendedAttribute",
                "type": "String"
            }  
        ]
    }],
  "version": "bf8c03ac-d45e-47fe-b3a1-711a9418b2b1"
}
 ```