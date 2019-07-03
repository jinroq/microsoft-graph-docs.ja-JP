---
title: licenseDetails を一覧表示する
description: LicenseDetails オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e2cbfe52d684a3c1ddf198fae7653f5da4b0099d
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35456772"
---
# <a name="list-licensedetails"></a><span data-ttu-id="8be1e-103">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="8be1e-103">List licenseDetails</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8be1e-104">LicenseDetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="8be1e-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8be1e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="8be1e-105">Permissions</span></span>
<span data-ttu-id="8be1e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8be1e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8be1e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8be1e-108">Permission type</span></span>      | <span data-ttu-id="8be1e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="8be1e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8be1e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8be1e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8be1e-111">Directory.accessasuser.all、すべてのユーザーが読み取り、すべてのディレクトリを取得します。すべてのユーザーが参照します。すべてのディレクトリ。</span><span class="sxs-lookup"><span data-stu-id="8be1e-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8be1e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8be1e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8be1e-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="8be1e-113">User.Read</span></span>    |
|<span data-ttu-id="8be1e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8be1e-114">Application</span></span> | <span data-ttu-id="8be1e-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8be1e-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8be1e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8be1e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="8be1e-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="8be1e-117">Optional query parameters</span></span>
<span data-ttu-id="8be1e-118">このメソッドは、 [OData クエリパラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートし**ていません**。</span><span class="sxs-lookup"><span data-stu-id="8be1e-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="8be1e-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8be1e-119">Request headers</span></span>
| <span data-ttu-id="8be1e-120">名前</span><span class="sxs-lookup"><span data-stu-id="8be1e-120">Name</span></span>      |<span data-ttu-id="8be1e-121">説明</span><span class="sxs-lookup"><span data-stu-id="8be1e-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="8be1e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8be1e-122">Authorization</span></span>  | <span data-ttu-id="8be1e-123">ベアラー &lt;コード&gt;</span><span class="sxs-lookup"><span data-stu-id="8be1e-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="8be1e-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="8be1e-124">Request body</span></span>
<span data-ttu-id="8be1e-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8be1e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8be1e-126">応答</span><span class="sxs-lookup"><span data-stu-id="8be1e-126">Response</span></span>

<span data-ttu-id="8be1e-127">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[licensedetails](../resources/licensedetails.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8be1e-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="8be1e-128">例</span><span class="sxs-lookup"><span data-stu-id="8be1e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8be1e-129">要求</span><span class="sxs-lookup"><span data-stu-id="8be1e-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="8be1e-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="8be1e-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="8be1e-131">C#</span><span class="sxs-lookup"><span data-stu-id="8be1e-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-licensedetails-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8be1e-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="8be1e-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-licensedetails-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="8be1e-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="8be1e-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-licensedetails-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="8be1e-134">応答</span><span class="sxs-lookup"><span data-stu-id="8be1e-134">Response</span></span>
<span data-ttu-id="8be1e-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8be1e-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
