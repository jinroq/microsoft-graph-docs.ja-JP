---
title: ApplicationSignInSummary を取得する
description: '**ApplicationSigninSummary**オブジェクトのプロパティとリレーションシップを取得します。'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 79a4da401899ce84b0929675da99b346086261a3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856732"
---
# <a name="get-applicationsigninsummary"></a><span data-ttu-id="08637-103">ApplicationSignInSummary を取得する</span><span class="sxs-lookup"><span data-stu-id="08637-103">Get applicationSignInSummary</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08637-104">[ApplicationSigninSummary](../resources/applicationsigninsummary.md)オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="08637-104">Retrieve the properties and relationships of an [applicationSigninSummary](../resources/applicationsigninsummary.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="08637-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="08637-105">Permissions</span></span>
<span data-ttu-id="08637-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08637-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference.md).</span></span>

|<span data-ttu-id="08637-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08637-108">Permission type</span></span>      | <span data-ttu-id="08637-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="08637-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08637-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08637-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08637-111">すべてのレポートを取得します。</span><span class="sxs-lookup"><span data-stu-id="08637-111">Report.Read.All</span></span> |
|<span data-ttu-id="08637-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08637-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08637-113">サポートされていません</span><span class="sxs-lookup"><span data-stu-id="08637-113">Not supported</span></span>   |
|<span data-ttu-id="08637-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08637-114">Application</span></span> | <span data-ttu-id="08637-115">すべてのレポートを取得します。</span><span class="sxs-lookup"><span data-stu-id="08637-115">Report.Read.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="08637-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08637-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
``` http
GET reports/getAzureADApplicationSignInSummary(period='{period}')
```

## <a name="function-parameters"></a><span data-ttu-id="08637-117">関数パラメーター</span><span class="sxs-lookup"><span data-stu-id="08637-117">Function parameters</span></span>

| <span data-ttu-id="08637-118">パラメーター</span><span class="sxs-lookup"><span data-stu-id="08637-118">Parameter</span></span> | <span data-ttu-id="08637-119">説明</span><span class="sxs-lookup"><span data-stu-id="08637-119">Description</span></span> |
|:----------|:----------|
| <span data-ttu-id="08637-120">period</span><span class="sxs-lookup"><span data-stu-id="08637-120">period</span></span> | <span data-ttu-id="08637-121">いずれ`D7`か (過去7日間) `D30`または (過去30日間)。他の値を指定すると、エラーが発生します。</span><span class="sxs-lookup"><span data-stu-id="08637-121">Either `D7` (last seven days) or `D30` (last 30 days); other values generate errors.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="08637-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08637-122">Request headers</span></span>
| <span data-ttu-id="08637-123">名前</span><span class="sxs-lookup"><span data-stu-id="08637-123">Name</span></span>      |<span data-ttu-id="08637-124">説明</span><span class="sxs-lookup"><span data-stu-id="08637-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="08637-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="08637-125">Authorization</span></span> | <span data-ttu-id="08637-126">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="08637-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="08637-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="08637-127">Request body</span></span>
<span data-ttu-id="08637-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="08637-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08637-129">応答</span><span class="sxs-lookup"><span data-stu-id="08637-129">Response</span></span>
<span data-ttu-id="08637-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[applicationSignInSummary](../resources/applicationsigninsummary.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="08637-130">If successful, this method returns a `200 OK` response code and an [applicationSignInSummary](../resources/applicationsigninsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08637-131">例</span><span class="sxs-lookup"><span data-stu-id="08637-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="08637-132">要求</span><span class="sxs-lookup"><span data-stu-id="08637-132">Request</span></span>
<span data-ttu-id="08637-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08637-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="08637-134">プロトコル</span><span class="sxs-lookup"><span data-stu-id="08637-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_applicationsigninsummary"
}-->
```http
GET https://graph.microsoft.com/beta/reports/getAzureADApplicationSignInSummary(period='D7')
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="08637-135">C#</span><span class="sxs-lookup"><span data-stu-id="08637-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-applicationsigninsummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="08637-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="08637-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-applicationsigninsummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="08637-137">目的-C</span><span class="sxs-lookup"><span data-stu-id="08637-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-applicationsigninsummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="08637-138">Java</span><span class="sxs-lookup"><span data-stu-id="08637-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-applicationsigninsummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="08637-139">応答</span><span class="sxs-lookup"><span data-stu-id="08637-139">Response</span></span>
<span data-ttu-id="08637-140">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="08637-140">The following is an example of the response.</span></span> 

><span data-ttu-id="08637-141">**注:** ここに示す response オブジェクトは読みやすくするために短縮されている場合があります。</span><span class="sxs-lookup"><span data-stu-id="08637-141">**Note:** The response object shown here mmight be shortened for readability.</span></span> <span data-ttu-id="08637-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="08637-142">All the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationSignInSummary",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
