---
title: PublishedResources のリスト
description: PublishedResource オブジェクトのリストを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 02d92e294afdb5af49e48ffefe375d84e5680c34
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840997"
---
# <a name="list-publishedresources"></a><span data-ttu-id="51787-103">PublishedResources のリスト</span><span class="sxs-lookup"><span data-stu-id="51787-103">List publishedResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51787-104">[Publishedresource](../resources/publishedresource.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="51787-104">Retrieve a list of [publishedResource](../resources/publishedresource.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="51787-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="51787-105">Permissions</span></span>

<span data-ttu-id="51787-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51787-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="51787-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51787-108">Permission type</span></span>                        | <span data-ttu-id="51787-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="51787-109">Permissions (from least to most privileged)</span></span> |
|:--------------------------------------|:---------------------------------------------------------|
| <span data-ttu-id="51787-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51787-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="51787-111">OnPremisesPublishingProfiles</span><span class="sxs-lookup"><span data-stu-id="51787-111">OnPremisesPublishingProfiles.ReadWrite.All</span></span> |
| <span data-ttu-id="51787-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51787-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51787-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51787-113">Not supported.</span></span> |
| <span data-ttu-id="51787-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51787-114">Application</span></span>                            | <span data-ttu-id="51787-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51787-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="51787-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51787-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET ~/onPremisesPublishingProfiles/{publishingType}/publishedResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51787-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="51787-117">Optional query parameters</span></span>

<span data-ttu-id="51787-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="51787-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="51787-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51787-119">Request headers</span></span>

| <span data-ttu-id="51787-120">名前</span><span class="sxs-lookup"><span data-stu-id="51787-120">Name</span></span>      |<span data-ttu-id="51787-121">説明</span><span class="sxs-lookup"><span data-stu-id="51787-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="51787-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51787-122">Authorization</span></span> | <span data-ttu-id="51787-123">ベアラー {トークン}</span><span class="sxs-lookup"><span data-stu-id="51787-123">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="51787-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="51787-124">Request body</span></span>

<span data-ttu-id="51787-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="51787-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51787-126">応答</span><span class="sxs-lookup"><span data-stu-id="51787-126">Response</span></span>

<span data-ttu-id="51787-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[publishedresource](../resources/publishedresource.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="51787-127">If successful, this method returns a `200 OK` response code and a collection of [publishedResource](../resources/publishedresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51787-128">例</span><span class="sxs-lookup"><span data-stu-id="51787-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="51787-129">要求</span><span class="sxs-lookup"><span data-stu-id="51787-129">Request</span></span>

<span data-ttu-id="51787-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51787-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_publishedresources"
}-->

```http
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/{publishingType}/publishedResources?$expand=agentGroups
```

### <a name="response"></a><span data-ttu-id="51787-131">応答</span><span class="sxs-lookup"><span data-stu-id="51787-131">Response</span></span>

<span data-ttu-id="51787-132">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="51787-132">The following is an example of the response.</span></span>

> <span data-ttu-id="51787-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="51787-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.publishedResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "publishingType": "provisioning",
      "displayName": "Demo provisioning",
      "id": "aed0b780-965f-4149-85c5-a8c73e58b67d",
      "resourceName": "domain1.contoso.com",
      "agentGroups": [
          {
              "id": "2d55ed41-1619-4848-92bb-0576d3038682",
              "displayName": "Group 1"
          }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List publishedResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
