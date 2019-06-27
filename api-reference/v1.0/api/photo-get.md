---
title: 写真を取得する
description: 写真オブジェクトのプロパティとリレーションシップを取得します。
localization_priority: Normal
ms.openlocfilehash: 513382d58690fdb2198e4974030cd1d9cafd65c7
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/27/2019
ms.locfileid: "35274236"
---
# <a name="get-photo"></a><span data-ttu-id="52198-103">写真を取得する</span><span class="sxs-lookup"><span data-stu-id="52198-103">Get photo</span></span>

<span data-ttu-id="52198-104">写真オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="52198-104">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="52198-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="52198-105">Permissions</span></span>
<span data-ttu-id="52198-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52198-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="52198-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="52198-108">Permission type</span></span>      | <span data-ttu-id="52198-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="52198-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="52198-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="52198-110">Delegated (work or school account)</span></span> | <span data-ttu-id="52198-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="52198-111">Files.Read</span></span>    |
|<span data-ttu-id="52198-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="52198-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="52198-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="52198-113">Files.Read</span></span>    |
|<span data-ttu-id="52198-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="52198-114">Application</span></span> | <span data-ttu-id="52198-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52198-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="52198-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="52198-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="52198-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="52198-117">Optional query parameters</span></span>
<span data-ttu-id="52198-118">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="52198-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="52198-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="52198-119">Request headers</span></span>
| <span data-ttu-id="52198-120">名前</span><span class="sxs-lookup"><span data-stu-id="52198-120">Name</span></span>       | <span data-ttu-id="52198-121">型</span><span class="sxs-lookup"><span data-stu-id="52198-121">Type</span></span> | <span data-ttu-id="52198-122">説明</span><span class="sxs-lookup"><span data-stu-id="52198-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="52198-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="52198-123">Authorization</span></span>  | <span data-ttu-id="52198-124">string</span><span class="sxs-lookup"><span data-stu-id="52198-124">string</span></span>  | <span data-ttu-id="52198-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="52198-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="52198-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="52198-127">Request body</span></span>
<span data-ttu-id="52198-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="52198-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="52198-129">応答</span><span class="sxs-lookup"><span data-stu-id="52198-129">Response</span></span>

<span data-ttu-id="52198-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[写真](../resources/photo.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="52198-130">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="52198-131">例</span><span class="sxs-lookup"><span data-stu-id="52198-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="52198-132">要求</span><span class="sxs-lookup"><span data-stu-id="52198-132">Request</span></span>
<span data-ttu-id="52198-133">以下は、写真のメタデータに対する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52198-133">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="52198-134">応答</span><span class="sxs-lookup"><span data-stu-id="52198-134">Response</span></span>
<span data-ttu-id="52198-135">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="52198-135">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="52198-136">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="52198-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52198-137">C#</span><span class="sxs-lookup"><span data-stu-id="52198-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photo-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52198-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="52198-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photo-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52198-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="52198-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_photo-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
##### <a name="request"></a><span data-ttu-id="52198-140">要求</span><span class="sxs-lookup"><span data-stu-id="52198-140">Request</span></span>
<span data-ttu-id="52198-141">以下は、写真のバイト数に対する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="52198-141">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="52198-142">応答</span><span class="sxs-lookup"><span data-stu-id="52198-142">Response</span></span>
<span data-ttu-id="52198-143">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="52198-143">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Edm.Stream" } -->

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: image/jpeg
ETag: "A19A6498"
request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
client-request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
x-ms-ags-diagnostic: {"ServerInfo":{"DataCenter":"West US","Slice":"SliceA","Ring":"5","ScaleUnit":"003","Host":"AGSFE_IN_14","ADSiteName":"WST"}}
Access-Control-Allow-Origin: *
Access-Control-Expose-Headers: ETag, Location, Preference-Applied, Content-Range, request-id, client-request-id
Duration: 125.9389
Date: Wed, 13 Dec 2017 22:02:17 GMT
Content-Length: 250526

<binary image data>
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="52198-144">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="52198-144">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="52198-145">C#</span><span class="sxs-lookup"><span data-stu-id="52198-145">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_photo_value-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="52198-146">Javascript</span><span class="sxs-lookup"><span data-stu-id="52198-146">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_photo_value-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="52198-147">目的-C</span><span class="sxs-lookup"><span data-stu-id="52198-147">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_photo_value-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/photo-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
