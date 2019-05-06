---
title: EducationSynchronizationProfile の状態を取得する
description: テナント内の特定の学校データ同期プロファイルの状態を取得します。 応答は、同期の状態を示します。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 74f33c53e850babed98536fba74de6d6162e9045
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33587532"
---
# <a name="get-the-status-of-an-educationsynchronizationprofile"></a><span data-ttu-id="3e69e-104">EducationSynchronizationProfile の状態を取得する</span><span class="sxs-lookup"><span data-stu-id="3e69e-104">Get the status of an educationSynchronizationProfile</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e69e-105">テナント内の特定の学校データ[同期プロファイル](../resources/educationsynchronizationprofile.md)の状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="3e69e-105">Get the status of a specific school data [synchronization profile](../resources/educationsynchronizationprofile.md) in the tenant.</span></span> <span data-ttu-id="3e69e-106">応答は、同期の状態を示します。</span><span class="sxs-lookup"><span data-stu-id="3e69e-106">The response will indicate the status of the sync.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e69e-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3e69e-107">Permissions</span></span>
<span data-ttu-id="3e69e-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3e69e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e69e-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3e69e-110">Permission type</span></span> | <span data-ttu-id="3e69e-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3e69e-111">Permissions (from least to most privileged)</span></span> |
|:-----------|:----------|
| <span data-ttu-id="3e69e-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3e69e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3e69e-113">EduAdministration、EduAdministration</span><span class="sxs-lookup"><span data-stu-id="3e69e-113">EduAdministration.Read, EduAdministration.ReadWrite</span></span> |
|<span data-ttu-id="3e69e-114">委任 (個人 Microsoft アカウント</span><span class="sxs-lookup"><span data-stu-id="3e69e-114">Delegated (personal Microsoft account</span></span>|<span data-ttu-id="3e69e-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3e69e-115">Not supported.</span></span>|
|<span data-ttu-id="3e69e-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3e69e-116">Application</span></span>| <span data-ttu-id="3e69e-117">EduAdministration、EduAdministration のいずれかを取得します。</span><span class="sxs-lookup"><span data-stu-id="3e69e-117">EduAdministration.Read.All, EduAdministration.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e69e-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3e69e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /synchronizationProfiles/{id}/profileStatus
```

## <a name="request-headers"></a><span data-ttu-id="3e69e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3e69e-119">Request headers</span></span>
| <span data-ttu-id="3e69e-120">名前</span><span class="sxs-lookup"><span data-stu-id="3e69e-120">Name</span></span>       | <span data-ttu-id="3e69e-121">型</span><span class="sxs-lookup"><span data-stu-id="3e69e-121">Type</span></span> | <span data-ttu-id="3e69e-122">説明</span><span class="sxs-lookup"><span data-stu-id="3e69e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="3e69e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e69e-123">Authorization</span></span>  | <span data-ttu-id="3e69e-124">string</span><span class="sxs-lookup"><span data-stu-id="3e69e-124">string</span></span>  | <span data-ttu-id="3e69e-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="3e69e-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e69e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3e69e-127">Request body</span></span>
<span data-ttu-id="3e69e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3e69e-128">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="3e69e-129">応答</span><span class="sxs-lookup"><span data-stu-id="3e69e-129">Response</span></span>
<span data-ttu-id="3e69e-130">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3e69e-130">If successful, this method returns a `200 OK` response code and an [educationsynchronizationprofilestatus](../resources/educationsynchronizationprofilestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e69e-131">例</span><span class="sxs-lookup"><span data-stu-id="3e69e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3e69e-132">要求</span><span class="sxs-lookup"><span data-stu-id="3e69e-132">Request</span></span>
<span data-ttu-id="3e69e-133">要求の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e69e-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_educationSynchronizationProfile_status"
}-->
```http
GET https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/profileStatus
```

##### <a name="response"></a><span data-ttu-id="3e69e-134">応答</span><span class="sxs-lookup"><span data-stu-id="3e69e-134">Response</span></span>
<span data-ttu-id="3e69e-135">応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3e69e-135">The following is an example of the response.</span></span> 

><span data-ttu-id="3e69e-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短くされている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="3e69e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3e69e-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="3e69e-138">SDK sample code</span></span>

# <a name="ctabcs"></a>[<span data-ttu-id="3e69e-139">Visual</span><span class="sxs-lookup"><span data-stu-id="3e69e-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_educationSynchronizationProfile_status-Cs-snippets.md)]

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
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/educationsynchronizationprofilestatus-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
