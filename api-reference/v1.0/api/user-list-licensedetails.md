---
title: licenseDetails を一覧表示する
description: licenseDetails オブジェクトの一覧を取得します。
author: dkershaw10
ms.openlocfilehash: af15e2cf8fb2bb9484d4567517c71a735f11609c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301072"
---
# <a name="list-licensedetails"></a><span data-ttu-id="898b5-103">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="898b5-103">List licenseDetails</span></span>

<span data-ttu-id="898b5-104">licenseDetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="898b5-104">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="898b5-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="898b5-105">Permissions</span></span>
<span data-ttu-id="898b5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="898b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="898b5-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="898b5-108">Permission type</span></span>      | <span data-ttu-id="898b5-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="898b5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="898b5-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="898b5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="898b5-111">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="898b5-111">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="898b5-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="898b5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="898b5-113">User.Read</span><span class="sxs-lookup"><span data-stu-id="898b5-113">User.Read</span></span>    |
|<span data-ttu-id="898b5-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="898b5-114">Application</span></span> | <span data-ttu-id="898b5-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="898b5-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="898b5-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="898b5-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="898b5-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="898b5-117">Optional query parameters</span></span>
<span data-ttu-id="898b5-118">このメソッドは [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートして**いません**。</span><span class="sxs-lookup"><span data-stu-id="898b5-118">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="898b5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="898b5-119">Request headers</span></span>
| <span data-ttu-id="898b5-120">名前</span><span class="sxs-lookup"><span data-stu-id="898b5-120">Name</span></span>      |<span data-ttu-id="898b5-121">説明</span><span class="sxs-lookup"><span data-stu-id="898b5-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="898b5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="898b5-122">Authorization</span></span>  | <span data-ttu-id="898b5-123">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="898b5-123">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="898b5-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="898b5-124">Request body</span></span>
<span data-ttu-id="898b5-125">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="898b5-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="898b5-126">応答</span><span class="sxs-lookup"><span data-stu-id="898b5-126">Response</span></span>

<span data-ttu-id="898b5-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [licenseDetails](../resources/licensedetails.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="898b5-127">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="898b5-128">例</span><span class="sxs-lookup"><span data-stu-id="898b5-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="898b5-129">要求</span><span class="sxs-lookup"><span data-stu-id="898b5-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="898b5-130">応答</span><span class="sxs-lookup"><span data-stu-id="898b5-130">Response</span></span>
<span data-ttu-id="898b5-p102">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="898b5-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List licenseDetails",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->