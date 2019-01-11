---
title: 契約を取得します。
description: プロパティと契約オブジェクトの関係を取得します。
localization_priority: Normal
ms.openlocfilehash: 0ca4e941705fe716c3aa11a73c934c40deb279d4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27818656"
---
# <a name="get-agreement"></a><span data-ttu-id="227b9-103">契約を取得します。</span><span class="sxs-lookup"><span data-stu-id="227b9-103">Get agreement</span></span>

> <span data-ttu-id="227b9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="227b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="227b9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="227b9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="227b9-106">プロパティと[契約](../resources/agreement.md)オブジェクトの関係を取得します。</span><span class="sxs-lookup"><span data-stu-id="227b9-106">Retrieve the properties and relationships of an [agreement](../resources/agreement.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="227b9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="227b9-107">Permissions</span></span>
<span data-ttu-id="227b9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="227b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="227b9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="227b9-110">Permission type</span></span>                        | <span data-ttu-id="227b9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="227b9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="227b9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="227b9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="227b9-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="227b9-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="227b9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="227b9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="227b9-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="227b9-115">Not supported.</span></span> |
|<span data-ttu-id="227b9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="227b9-116">Application</span></span>                            | <span data-ttu-id="227b9-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="227b9-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="227b9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="227b9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements/<id>
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="227b9-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="227b9-119">Request headers</span></span>
| <span data-ttu-id="227b9-120">名前</span><span class="sxs-lookup"><span data-stu-id="227b9-120">Name</span></span>         | <span data-ttu-id="227b9-121">種類</span><span class="sxs-lookup"><span data-stu-id="227b9-121">Type</span></span>        | <span data-ttu-id="227b9-122">説明</span><span class="sxs-lookup"><span data-stu-id="227b9-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="227b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="227b9-123">Authorization</span></span> | <span data-ttu-id="227b9-124">string</span><span class="sxs-lookup"><span data-stu-id="227b9-124">string</span></span> | <span data-ttu-id="227b9-125">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="227b9-125">Bearer \{token\}.</span></span> <span data-ttu-id="227b9-126">必須。</span><span class="sxs-lookup"><span data-stu-id="227b9-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="227b9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="227b9-127">Request body</span></span>
<span data-ttu-id="227b9-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="227b9-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="227b9-129">応答</span><span class="sxs-lookup"><span data-stu-id="227b9-129">Response</span></span>
<span data-ttu-id="227b9-130">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードおよび[契約](../resources/agreement.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="227b9-130">If successful, this method returns a `200 OK` response code and [agreement](../resources/agreement.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="227b9-131">例</span><span class="sxs-lookup"><span data-stu-id="227b9-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="227b9-132">要求</span><span class="sxs-lookup"><span data-stu-id="227b9-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreement"
}-->
```http
GET https://graph.microsoft.com/beta/agreements/<id>?$expand=files
```
##### <a name="response"></a><span data-ttu-id="227b9-133">応答</span><span class="sxs-lookup"><span data-stu-id="227b9-133">Response</span></span>
><span data-ttu-id="227b9-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="227b9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get agreement",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
