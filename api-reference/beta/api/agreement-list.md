---
title: リスト契約
description: 契約オブジェクトのリストを取得します。
localization_priority: Normal
ms.openlocfilehash: 3ae255a386986b5627aed99f29dca5bfb9934e30
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27859921"
---
# <a name="list-agreements"></a><span data-ttu-id="eaa9a-103">リスト契約</span><span class="sxs-lookup"><span data-stu-id="eaa9a-103">List agreements</span></span>

> <span data-ttu-id="eaa9a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eaa9a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="eaa9a-106">[契約](../resources/agreement.md)オブジェクトのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-106">Retrieve a list of [agreement](../resources/agreement.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="eaa9a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="eaa9a-107">Permissions</span></span>
<span data-ttu-id="eaa9a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eaa9a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eaa9a-110">Permission type</span></span>                        | <span data-ttu-id="eaa9a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="eaa9a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="eaa9a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eaa9a-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="eaa9a-113">Agreement.Read.All</span><span class="sxs-lookup"><span data-stu-id="eaa9a-113">Agreement.Read.All</span></span> |
|<span data-ttu-id="eaa9a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eaa9a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eaa9a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-115">Not supported.</span></span> |
|<span data-ttu-id="eaa9a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eaa9a-116">Application</span></span>                            | <span data-ttu-id="eaa9a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eaa9a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eaa9a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /agreements
```
<!--
## Optional query parameters
This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.
-->

## <a name="request-headers"></a><span data-ttu-id="eaa9a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eaa9a-119">Request headers</span></span>
| <span data-ttu-id="eaa9a-120">名前</span><span class="sxs-lookup"><span data-stu-id="eaa9a-120">Name</span></span>         | <span data-ttu-id="eaa9a-121">種類</span><span class="sxs-lookup"><span data-stu-id="eaa9a-121">Type</span></span>        | <span data-ttu-id="eaa9a-122">説明</span><span class="sxs-lookup"><span data-stu-id="eaa9a-122">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="eaa9a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eaa9a-123">Authorization</span></span> | <span data-ttu-id="eaa9a-124">string</span><span class="sxs-lookup"><span data-stu-id="eaa9a-124">string</span></span> | <span data-ttu-id="eaa9a-125">ベアラー\{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-125">Bearer \{token\}.</span></span> <span data-ttu-id="eaa9a-126">必須。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="eaa9a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="eaa9a-127">Request body</span></span>
<span data-ttu-id="eaa9a-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="eaa9a-129">応答</span><span class="sxs-lookup"><span data-stu-id="eaa9a-129">Response</span></span>
<span data-ttu-id="eaa9a-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文の[許可書](../resources/agreement.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-130">If successful, this method returns a `200 OK` response code and collection of [agreement](../resources/agreement.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="eaa9a-131">例</span><span class="sxs-lookup"><span data-stu-id="eaa9a-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="eaa9a-132">要求</span><span class="sxs-lookup"><span data-stu-id="eaa9a-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "get_agreements"
}-->
```http
GET https://graph.microsoft.com/beta/agreements
```
##### <a name="response"></a><span data-ttu-id="eaa9a-133">応答</span><span class="sxs-lookup"><span data-stu-id="eaa9a-133">Response</span></span>
><span data-ttu-id="eaa9a-p104">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="eaa9a-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.agreement",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 146

{
  "value": [
    {
      "displayName": "displayName-value",
      "isViewingBeforeAcceptanceRequired": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List agreements",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
