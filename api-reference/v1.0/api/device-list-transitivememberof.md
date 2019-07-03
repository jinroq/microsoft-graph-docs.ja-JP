---
title: デバイスの推移性のグループを一覧表示する
description: デバイスがメンバーであるグループを取得します。 この API 要求は推移的なので、デバイスがのネストされたメンバーであるすべてのグループも返します。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: f73efd6d096a860f51a4d86190e25bf7f26d8135
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/02/2019
ms.locfileid: "35461261"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="4580a-104">デバイスの推移性のグループを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="4580a-104">List device transitive groups</span></span>

<span data-ttu-id="4580a-105">デバイスがメンバーであるグループを取得します。</span><span class="sxs-lookup"><span data-stu-id="4580a-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="4580a-106">この API 要求は推移的なので、デバイスがのネストされたメンバーであるすべてのグループも返します。</span><span class="sxs-lookup"><span data-stu-id="4580a-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="4580a-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="4580a-107">Permissions</span></span>

<span data-ttu-id="4580a-p103">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4580a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4580a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4580a-110">Permission type</span></span>      | <span data-ttu-id="4580a-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="4580a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4580a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4580a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="4580a-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4580a-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4580a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4580a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4580a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4580a-115">Not supported.</span></span>    |
|<span data-ttu-id="4580a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4580a-116">Application</span></span> | <span data-ttu-id="4580a-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4580a-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4580a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4580a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4580a-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4580a-119">Optional query parameters</span></span>

<span data-ttu-id="4580a-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](/graph/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4580a-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4580a-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4580a-121">Request headers</span></span>

| <span data-ttu-id="4580a-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4580a-122">Header</span></span>       | <span data-ttu-id="4580a-123">値</span><span class="sxs-lookup"><span data-stu-id="4580a-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4580a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4580a-124">Authorization</span></span>  | <span data-ttu-id="4580a-p104">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="4580a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4580a-127">承諾</span><span class="sxs-lookup"><span data-stu-id="4580a-127">Accept</span></span>  | <span data-ttu-id="4580a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4580a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4580a-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="4580a-129">Request body</span></span>

<span data-ttu-id="4580a-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4580a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4580a-131">応答</span><span class="sxs-lookup"><span data-stu-id="4580a-131">Response</span></span>

<span data-ttu-id="4580a-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [directoryObject](../resources/directoryobject.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4580a-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4580a-133">例</span><span class="sxs-lookup"><span data-stu-id="4580a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="4580a-134">要求</span><span class="sxs-lookup"><span data-stu-id="4580a-134">Request</span></span>

<span data-ttu-id="4580a-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4580a-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="4580a-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="4580a-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="4580a-137">C#</span><span class="sxs-lookup"><span data-stu-id="4580a-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="4580a-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="4580a-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="4580a-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="4580a-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4580a-140">応答</span><span class="sxs-lookup"><span data-stu-id="4580a-140">Response</span></span>

<span data-ttu-id="4580a-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4580a-141">Here is an example of the response.</span></span> 

><span data-ttu-id="4580a-p105">**注:** 読みやすくするために、ここに示す応答オブジェクトは短縮されている場合があります。実際の呼び出しからは、すべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="4580a-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
