---
title: ドメインを取得する
description: ドメイン オブジェクトのプロパティとリレーションシップを取得します。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 03dcc7f5eff084ec79cb39a60688aadfaf0d63fc
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514538"
---
# <a name="get-domain"></a><span data-ttu-id="f7b14-103">ドメインを取得する</span><span class="sxs-lookup"><span data-stu-id="f7b14-103">Get domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7b14-104">ドメイン オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="f7b14-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7b14-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f7b14-105">Permissions</span></span>

<span data-ttu-id="f7b14-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f7b14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f7b14-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f7b14-108">Permission type</span></span>      | <span data-ttu-id="f7b14-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f7b14-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7b14-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f7b14-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f7b14-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7b14-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="f7b14-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f7b14-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7b14-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7b14-113">Not supported.</span></span>    |
|<span data-ttu-id="f7b14-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f7b14-114">Application</span></span> | <span data-ttu-id="f7b14-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7b14-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7b14-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f7b14-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="f7b14-117">{Id} には、ドメインを完全修飾ドメイン名で指定します。</span><span class="sxs-lookup"><span data-stu-id="f7b14-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f7b14-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f7b14-118">Optional query parameters</span></span>

<span data-ttu-id="f7b14-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f7b14-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f7b14-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f7b14-120">Request headers</span></span>

| <span data-ttu-id="f7b14-121">名前</span><span class="sxs-lookup"><span data-stu-id="f7b14-121">Name</span></span>      |<span data-ttu-id="f7b14-122">説明</span><span class="sxs-lookup"><span data-stu-id="f7b14-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f7b14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7b14-123">Authorization</span></span>  | <span data-ttu-id="f7b14-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="f7b14-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f7b14-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f7b14-126">Content-Type</span></span>  | <span data-ttu-id="f7b14-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f7b14-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f7b14-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="f7b14-128">Request body</span></span>
<span data-ttu-id="f7b14-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f7b14-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7b14-130">応答</span><span class="sxs-lookup"><span data-stu-id="f7b14-130">Response</span></span>

<span data-ttu-id="f7b14-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [domain](../resources/domain.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f7b14-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f7b14-132">例</span><span class="sxs-lookup"><span data-stu-id="f7b14-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f7b14-133">要求</span><span class="sxs-lookup"><span data-stu-id="f7b14-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
##### <a name="response"></a><span data-ttu-id="f7b14-134">応答</span><span class="sxs-lookup"><span data-stu-id="f7b14-134">Response</span></span>
<span data-ttu-id="f7b14-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f7b14-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
