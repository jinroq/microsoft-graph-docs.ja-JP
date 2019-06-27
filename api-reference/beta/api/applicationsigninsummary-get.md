---
title: ApplicationSignInSummary を取得する
description: '**ApplicationSigninSummary**オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fb9dfa4f57226ed846fcf7e7b6668214ad4be7ca
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258395"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="f9b3c-103">ApplicationSignInSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="f9b3c-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9b3c-104">[ApplicationSigninSummary](../resources/applicationsigninsummary.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f9b3c-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f9b3c-105">Permissions</span></span>
<span data-ttu-id="f9b3c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="f9b3c-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9b3c-108">Permission type</span></span>      | <span data-ttu-id="f9b3c-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9b3c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f9b3c-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9b3c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f9b3c-111">すべてのレポートを取得します。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-111">Report.Read.All</span></span> |
|<span data-ttu-id="f9b3c-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9b3c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f9b3c-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="f9b3c-113">Not supported</span></span>   |
|<span data-ttu-id="f9b3c-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9b3c-114">Application</span></span> | <span data-ttu-id="f9b3c-115">すべてのレポートを取得します。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="f9b3c-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9b3c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="f9b3c-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="f9b3c-117">Function parameters</span></span>

| <span data-ttu-id="f9b3c-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="f9b3c-118">Parameter</span></span> | <span data-ttu-id="f9b3c-119">説明</span><span class="sxs-lookup"><span data-stu-id="f9b3c-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="f9b3c-120">period</span><span class="sxs-lookup"><span data-stu-id="f9b3c-120">period</span></span> | <span data-ttu-id="f9b3c-121">いずれ`D7`か (過去7日間) `D30`または (過去30日間)。他の値を指定すると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="f9b3c-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9b3c-122">Request headers</span></span>
| <span data-ttu-id="f9b3c-123">名前</span><span class="sxs-lookup"><span data-stu-id="f9b3c-123">Name</span></span>      |<span data-ttu-id="f9b3c-124">説明</span><span class="sxs-lookup"><span data-stu-id="f9b3c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f9b3c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9b3c-125">Authorization</span></span> | <span data-ttu-id="f9b3c-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f9b3c-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="f9b3c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9b3c-127">Request body</span></span>
<span data-ttu-id="f9b3c-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9b3c-129">応答</span><span class="sxs-lookup"><span data-stu-id="f9b3c-129">Response</span></span>
<span data-ttu-id="f9b3c-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[applicationSignInSummary](../resources/applicationsigninsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9b3c-131">例</span><span class="sxs-lookup"><span data-stu-id="f9b3c-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f9b3c-132">要求</span><span class="sxs-lookup"><span data-stu-id="f9b3c-132">Request</span></span>
<span data-ttu-id="f9b3c-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
### <a name="response"></a><span data-ttu-id="f9b3c-134">応答</span><span class="sxs-lookup"><span data-stu-id="f9b3c-134">Response</span></span>
<span data-ttu-id="f9b3c-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-135">The following is an example of the response.</span></span> 

><span data-ttu-id="f9b3c-136">**注:** ここに示す response オブジェクトは読みやすくするために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-136">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="f9b3c-137">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="f9b3c-137">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationSignInSummary"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "appId": "appId-value",
  "appDisplayName": "appDisplayName-value",
  "successfulSignInCount": 99,
  "failedSignInCount": 99,
  "successPercentage": 99
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f9b3c-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="f9b3c-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f9b3c-139">C#</span><span class="sxs-lookup"><span data-stu-id="f9b3c-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f9b3c-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="f9b3c-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f9b3c-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="f9b3c-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_applicationsigninsummary-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/applicationsigninsummary-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
