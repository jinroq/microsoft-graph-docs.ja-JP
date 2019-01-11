---
title: licenseDetails を一覧表示する
description: licenseDetails オブジェクトの一覧を取得します。
author: dkershaw10
localization_priority: Normal
ms.openlocfilehash: f000cc390673887a7708f8615769416cbc2204b3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27863358"
---
# <a name="list-licensedetails"></a><span data-ttu-id="ca9f9-103">licenseDetails を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="ca9f9-103">List licenseDetails</span></span>

> <span data-ttu-id="ca9f9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ca9f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca9f9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca9f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca9f9-106">licenseDetails オブジェクトの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="ca9f9-106">Retrieve a list of licenseDetails objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca9f9-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ca9f9-107">Permissions</span></span>
<span data-ttu-id="ca9f9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca9f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca9f9-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca9f9-110">Permission type</span></span>      | <span data-ttu-id="ca9f9-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca9f9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca9f9-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca9f9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ca9f9-113">User.Read、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca9f9-113">User.Read, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca9f9-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca9f9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca9f9-115">User.Read</span><span class="sxs-lookup"><span data-stu-id="ca9f9-115">User.Read</span></span>    |
|<span data-ttu-id="ca9f9-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca9f9-116">Application</span></span> | <span data-ttu-id="ca9f9-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca9f9-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca9f9-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca9f9-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/licenseDetails
GET /users/{id}/licenseDetails
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ca9f9-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ca9f9-119">Optional query parameters</span></span>
<span data-ttu-id="ca9f9-120">このメソッドは [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートして**いません**。</span><span class="sxs-lookup"><span data-stu-id="ca9f9-120">This method does **not** support [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca9f9-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca9f9-121">Request headers</span></span>
| <span data-ttu-id="ca9f9-122">名前</span><span class="sxs-lookup"><span data-stu-id="ca9f9-122">Name</span></span>      |<span data-ttu-id="ca9f9-123">説明</span><span class="sxs-lookup"><span data-stu-id="ca9f9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ca9f9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca9f9-124">Authorization</span></span>  | <span data-ttu-id="ca9f9-125">Bearer &lt;code&gt;</span><span class="sxs-lookup"><span data-stu-id="ca9f9-125">Bearer &lt;code&gt;</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca9f9-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca9f9-126">Request body</span></span>
<span data-ttu-id="ca9f9-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ca9f9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca9f9-128">応答</span><span class="sxs-lookup"><span data-stu-id="ca9f9-128">Response</span></span>

<span data-ttu-id="ca9f9-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [licenseDetails](../resources/licensedetails.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ca9f9-129">If successful, this method returns a `200 OK` response code and collection of [licenseDetails](../resources/licensedetails.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ca9f9-130">例</span><span class="sxs-lookup"><span data-stu-id="ca9f9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ca9f9-131">要求</span><span class="sxs-lookup"><span data-stu-id="ca9f9-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_licensedetails"
}-->
```http
GET https://graph.microsoft.com/beta/me/licenseDetails
```
##### <a name="response"></a><span data-ttu-id="ca9f9-132">応答</span><span class="sxs-lookup"><span data-stu-id="ca9f9-132">Response</span></span>
<span data-ttu-id="ca9f9-p103">注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca9f9-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
