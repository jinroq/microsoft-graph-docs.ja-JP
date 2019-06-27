---
title: licenseDetails を一覧表示する
description: LicenseDetails オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6d5da3abef365ad02bc363df5ef01d9f4e1c1fe2
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35271751"
---
# <a name="list-licensedetails"></a><span data-ttu-id="11f2e-103">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="11f2e-103">List licenseDetails</span></span>

<span data-ttu-id="11f2e-104">LicenseDetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="11f2e-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="11f2e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="11f2e-105">Permissions</span></span>
<span data-ttu-id="11f2e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11f2e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11f2e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="11f2e-108">Permission type</span></span>      | <span data-ttu-id="11f2e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="11f2e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11f2e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="11f2e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11f2e-111">Directory.accessasuser.all、すべてのユーザーが読み取り、すべてのディレクトリを取得します。すべてのユーザーが参照します。すべてのディレクトリ。</span><span class="sxs-lookup"><span data-stu-id="11f2e-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="11f2e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="11f2e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11f2e-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="11f2e-113">User.Read</span></span>    |
|<span data-ttu-id="11f2e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="11f2e-114">Application</span></span> | <span data-ttu-id="11f2e-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11f2e-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="11f2e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="11f2e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="11f2e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="11f2e-117">Optional query parameters</span></span>
<span data-ttu-id="11f2e-118">このメソッドは、 [OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートし**ていません**。</span><span class="sxs-lookup"><span data-stu-id="11f2e-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="11f2e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="11f2e-119">Request headers</span></span>
| <span data-ttu-id="11f2e-120">名前</span><span class="sxs-lookup"><span data-stu-id="11f2e-120">Name</span></span>      |<span data-ttu-id="11f2e-121">説明</span><span class="sxs-lookup"><span data-stu-id="11f2e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11f2e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11f2e-122">Authorization</span></span>  | <span data-ttu-id="11f2e-123">ベアラー &lt;コード&gt;</span><span class="sxs-lookup"><span data-stu-id="11f2e-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="11f2e-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="11f2e-124">Request body</span></span>
<span data-ttu-id="11f2e-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="11f2e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11f2e-126">応答</span><span class="sxs-lookup"><span data-stu-id="11f2e-126">Response</span></span>

<span data-ttu-id="11f2e-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[licensedetails](../resources/licensedetails.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="11f2e-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="11f2e-128">例</span><span class="sxs-lookup"><span data-stu-id="11f2e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="11f2e-129">要求</span><span class="sxs-lookup"><span data-stu-id="11f2e-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="11f2e-130">応答</span><span class="sxs-lookup"><span data-stu-id="11f2e-130">Response</span></span>
<span data-ttu-id="11f2e-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="11f2e-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.licenseDetails",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 389

{
  "value": [
    {
      "servicePlans": [
        {
          "servicePlanId": "servicePlanId-value",
          "servicePlanName": "servicePlanName-value",
          "provisioningStatus": "provisioningStatus-value",
          "appliesTo": "appliesTo-value"
        }
      ],
      "skuId": "skuId-value",
      "skuPartNumber": "skuPartNumber-value",
      "id": "id-value"
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="11f2e-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="11f2e-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="11f2e-134">C#</span><span class="sxs-lookup"><span data-stu-id="11f2e-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_licensedetails-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="11f2e-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="11f2e-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_licensedetails-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="11f2e-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="11f2e-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_licensedetails-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-licensedetails.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/user-list-licensedetails.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-licensedetails.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
