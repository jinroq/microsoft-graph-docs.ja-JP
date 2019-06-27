---
title: EducationSynchronizationProfile の状態を取得する
description: テナント内の特定の学校データ同期プロファイルの状態を取得します。 応答は、同期の状態を示します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d9a5de844aeabad03364a6c984f2fd7c3ae7d9bf
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35259375"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="5ea90-104">EducationSynchronizationProfile の状態を取得する</span><span class="sxs-lookup"><span data-stu-id="5ea90-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ea90-105">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="5ea90-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="5ea90-106">応答は、同期の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="5ea90-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ea90-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5ea90-107">Permissions</span></span>
<span data-ttu-id="5ea90-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5ea90-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ea90-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5ea90-110">Permission type</span></span> | <span data-ttu-id="5ea90-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5ea90-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="5ea90-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5ea90-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ea90-113">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="5ea90-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="5ea90-114">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="5ea90-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="5ea90-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5ea90-115">Not supported.</span></span>|
|<span data-ttu-id="5ea90-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5ea90-116">Application</span></span>| <span data-ttu-id="5ea90-117">EduAdministration、EduAdministration のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="5ea90-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ea90-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5ea90-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="5ea90-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5ea90-119">Request headers</span></span>
| <span data-ttu-id="5ea90-120">名前</span><span class="sxs-lookup"><span data-stu-id="5ea90-120">Name</span></span>       | <span data-ttu-id="5ea90-121">型</span><span class="sxs-lookup"><span data-stu-id="5ea90-121">Type</span></span> | <span data-ttu-id="5ea90-122">説明</span><span class="sxs-lookup"><span data-stu-id="5ea90-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5ea90-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ea90-123">Authorization</span></span>  | <span data-ttu-id="5ea90-124">string</span><span class="sxs-lookup"><span data-stu-id="5ea90-124">string</span></span>  | <span data-ttu-id="5ea90-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="5ea90-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5ea90-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5ea90-127">Request body</span></span>
<span data-ttu-id="5ea90-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5ea90-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="5ea90-129">応答</span><span class="sxs-lookup"><span data-stu-id="5ea90-129">Response</span></span>
<span data-ttu-id="5ea90-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5ea90-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea90-131">例</span><span class="sxs-lookup"><span data-stu-id="5ea90-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5ea90-132">要求</span><span class="sxs-lookup"><span data-stu-id="5ea90-132">Request</span></span>
<span data-ttu-id="5ea90-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ea90-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="5ea90-134">応答</span><span class="sxs-lookup"><span data-stu-id="5ea90-134">Response</span></span>
<span data-ttu-id="5ea90-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ea90-135">The following is an example of the response.</span></span> 

><span data-ttu-id="5ea90-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="5ea90-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.educationSynchronizationProfileStatus",
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 232

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#education/synchronizationProfiles('{id}')/profileStatus/$entity",
    "status": "inProgress",
    "lastSynchronizationDateTime": "2017-07-04T22:06:37.6472621Z"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="5ea90-138">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="5ea90-138">SDK sample code</span></span>
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5ea90-139">Javascript</span><span class="sxs-lookup"><span data-stu-id="5ea90-139">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_status-Javascript-snippets.md)]

# <a name="ctabcs"></a>[<span data-ttu-id="5ea90-140">C#</span><span class="sxs-lookup"><span data-stu-id="5ea90-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_status-Cs-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="5ea90-141">目的-C</span><span class="sxs-lookup"><span data-stu-id="5ea90-141">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_status-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
