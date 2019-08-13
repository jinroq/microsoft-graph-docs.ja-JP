---
title: ApplicationSignInDetailedSummary を取得する
description: ApplicationSignInDetailSummary オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c847aefb1a7e9ab7b18821d2c002bbc96f3c1a7d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318678"
---
# <a name="get-applicationsignindetailedsummary"></a><span data-ttu-id="9ffbf-103">ApplicationSignInDetailedSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="9ffbf-103">Get applicationSignInDetailedSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ffbf-104">[ApplicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-104">Retrieve the properties and relationships of an [applicationSignInDetailSummary](../resources/applicationsignindetailedsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ffbf-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="9ffbf-105">Permissions</span></span>
<span data-ttu-id="9ffbf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="9ffbf-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ffbf-108">Permission type</span></span>                        | <span data-ttu-id="9ffbf-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ffbf-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ffbf-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ffbf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ffbf-111">すべてのレポートを取得します。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-111">Report.Read.All</span></span> |
|<span data-ttu-id="9ffbf-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ffbf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ffbf-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-113">Not supported.</span></span> |
|<span data-ttu-id="9ffbf-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ffbf-114">Application</span></span>                            | <span data-ttu-id="9ffbf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ffbf-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ffbf-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET /reports/applicationSignInDetailedSummary/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ffbf-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="9ffbf-117">Optional query parameters</span></span>

<span data-ttu-id="9ffbf-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-118">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ffbf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ffbf-119">Request headers</span></span>

| <span data-ttu-id="9ffbf-120">名前</span><span class="sxs-lookup"><span data-stu-id="9ffbf-120">Name</span></span>      |<span data-ttu-id="9ffbf-121">説明</span><span class="sxs-lookup"><span data-stu-id="9ffbf-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9ffbf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ffbf-122">Authorization</span></span> | <span data-ttu-id="9ffbf-123">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="9ffbf-123">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ffbf-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ffbf-124">Request body</span></span>
<span data-ttu-id="9ffbf-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ffbf-126">応答</span><span class="sxs-lookup"><span data-stu-id="9ffbf-126">Response</span></span>
<span data-ttu-id="9ffbf-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-127">If successful, this method returns a `200 OK` response code and an [applicationSignInDetailedSummary](../resources/applicationsignindetailedsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ffbf-128">例</span><span class="sxs-lookup"><span data-stu-id="9ffbf-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ffbf-129">要求</span><span class="sxs-lookup"><span data-stu-id="9ffbf-129">Request</span></span>
<span data-ttu-id="9ffbf-130">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ffbf-131">プロトコル</span><span class="sxs-lookup"><span data-stu-id="9ffbf-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsignindetailedsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/applicationSignInDetailedSummary/<id>
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ffbf-132">C#</span><span class="sxs-lookup"><span data-stu-id="9ffbf-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsignindetailedsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ffbf-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ffbf-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsignindetailedsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ffbf-134">目的-C</span><span class="sxs-lookup"><span data-stu-id="9ffbf-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsignindetailedsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="9ffbf-135">Java</span><span class="sxs-lookup"><span data-stu-id="9ffbf-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsignindetailedsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9ffbf-136">応答</span><span class="sxs-lookup"><span data-stu-id="9ffbf-136">Response</span></span>
<span data-ttu-id="9ffbf-137">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-137">The following is an example of the response.</span></span> 

><span data-ttu-id="9ffbf-p102">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="9ffbf-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInDetailedSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 295

{
  "id": "id-value",
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "status": {
    "errorCode": 99,
    "failureReason": "failureReason-value",
    "additionalDetails": "additionalDetails-value"
  },
  "signInCount": 99,
  "aggregatedEventDateTime": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInDetailedSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
