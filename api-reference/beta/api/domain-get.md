---
title: ドメインを取得する
description: ドメイン オブジェクトのプロパティとリレーションシップを取得します。
author: lleonard-msft
ms.openlocfilehash: 00afe2423dd5c294a701d0a6f38e5f395d890571
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313791"
---
# <a name="get-domain"></a><span data-ttu-id="1ba50-103">ドメインを取得する</span><span class="sxs-lookup"><span data-stu-id="1ba50-103">Get domain</span></span>

> <span data-ttu-id="1ba50-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1ba50-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1ba50-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ba50-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1ba50-106">ドメイン オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="1ba50-106">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="1ba50-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1ba50-107">Permissions</span></span>

<span data-ttu-id="1ba50-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ba50-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1ba50-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ba50-110">Permission type</span></span>      | <span data-ttu-id="1ba50-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ba50-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1ba50-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ba50-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1ba50-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1ba50-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="1ba50-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ba50-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1ba50-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ba50-115">Not supported.</span></span>    |
|<span data-ttu-id="1ba50-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ba50-116">Application</span></span> | <span data-ttu-id="1ba50-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba50-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1ba50-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ba50-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="1ba50-119">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="1ba50-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="1ba50-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="1ba50-120">Optional query parameters</span></span>

<span data-ttu-id="1ba50-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="1ba50-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1ba50-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ba50-122">Request headers</span></span>

| <span data-ttu-id="1ba50-123">名前</span><span class="sxs-lookup"><span data-stu-id="1ba50-123">Name</span></span>      |<span data-ttu-id="1ba50-124">説明</span><span class="sxs-lookup"><span data-stu-id="1ba50-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="1ba50-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ba50-125">Authorization</span></span>  | <span data-ttu-id="1ba50-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="1ba50-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1ba50-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1ba50-128">Content-Type</span></span>  | <span data-ttu-id="1ba50-129">application/json</span><span class="sxs-lookup"><span data-stu-id="1ba50-129">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1ba50-130">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ba50-130">Request body</span></span>
<span data-ttu-id="1ba50-131">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1ba50-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1ba50-132">応答</span><span class="sxs-lookup"><span data-stu-id="1ba50-132">Response</span></span>

<span data-ttu-id="1ba50-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1ba50-133">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1ba50-134">例</span><span class="sxs-lookup"><span data-stu-id="1ba50-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1ba50-135">要求</span><span class="sxs-lookup"><span data-stu-id="1ba50-135">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="1ba50-136">応答</span><span class="sxs-lookup"><span data-stu-id="1ba50-136">Response</span></span>
<span data-ttu-id="1ba50-p104">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ba50-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->