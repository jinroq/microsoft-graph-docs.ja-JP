---
title: 契約を取得する
description: アグリーメントオブジェクトのプロパティと関係を取得します。
localization_priority: Normal
ms.openlocfilehash: c74ae07a27bd45798298e03ee9bf71c860ba62d2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322722"
---
# <a name="get-agreement"></a><span data-ttu-id="680c6-103">契約を取得する</span><span class="sxs-lookup"><span data-stu-id="680c6-103">Get agreement</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="680c6-104">[アグリーメント](../resources/agreement.md)オブジェクトのプロパティと関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="680c6-104">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="680c6-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="680c6-105">Permissions</span></span>
<span data-ttu-id="680c6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="680c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="680c6-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="680c6-108">Permission type</span></span>                        | <span data-ttu-id="680c6-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="680c6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="680c6-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="680c6-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="680c6-111">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="680c6-111">Agreement.Read.All</span></span> |
|<span data-ttu-id="680c6-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="680c6-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="680c6-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="680c6-113">Not supported.</span></span> |
|<span data-ttu-id="680c6-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="680c6-114">Application</span></span>                            | <span data-ttu-id="680c6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="680c6-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="680c6-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="680c6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="680c6-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="680c6-117">Request headers</span></span>
| <span data-ttu-id="680c6-118">名前</span><span class="sxs-lookup"><span data-stu-id="680c6-118">Name</span></span>         | <span data-ttu-id="680c6-119">型</span><span class="sxs-lookup"><span data-stu-id="680c6-119">Type</span></span>        | <span data-ttu-id="680c6-120">説明</span><span class="sxs-lookup"><span data-stu-id="680c6-120">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="680c6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="680c6-121">Authorization</span></span> | <span data-ttu-id="680c6-122">string</span><span class="sxs-lookup"><span data-stu-id="680c6-122">string</span></span> | <span data-ttu-id="680c6-p102">ベアラー \{トークン\}。必須。</span><span class="sxs-lookup"><span data-stu-id="680c6-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="680c6-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="680c6-125">Request body</span></span>
<span data-ttu-id="680c6-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="680c6-126">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="680c6-127">応答</span><span class="sxs-lookup"><span data-stu-id="680c6-127">Response</span></span>
<span data-ttu-id="680c6-128">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[アグリーメント](../resources/agreement.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="680c6-128">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="680c6-129">例</span><span class="sxs-lookup"><span data-stu-id="680c6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="680c6-130">要求</span><span class="sxs-lookup"><span data-stu-id="680c6-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="680c6-131">応答</span><span class="sxs-lookup"><span data-stu-id="680c6-131">Response</span></span>
><span data-ttu-id="680c6-p103">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="680c6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "id": "id-value",
  "files": [
    {
      "id": "id-value",
      "language": "en",
      "fileName": "TOU.pdf",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
