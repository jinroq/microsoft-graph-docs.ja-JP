---
title: 写真を取得する
description: 写真オブジェクトのプロパティとリレーションシップを取得します。
ms.openlocfilehash: 16e0849d3cc1a9a98226b6f34221a8a37cec72b1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066466"
---
# <a name="get-photo"></a><span data-ttu-id="941d0-103">写真を取得する</span><span class="sxs-lookup"><span data-stu-id="941d0-103">Get photo</span></span>

> <span data-ttu-id="941d0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="941d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="941d0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="941d0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="941d0-106">写真オブジェクトのプロパティとリレーションシップを取得します。</span><span class="sxs-lookup"><span data-stu-id="941d0-106">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="941d0-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="941d0-107">Permissions</span></span>
<span data-ttu-id="941d0-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="941d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="941d0-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="941d0-110">Permission type</span></span>      | <span data-ttu-id="941d0-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="941d0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="941d0-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="941d0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="941d0-113">Files.Read</span><span class="sxs-lookup"><span data-stu-id="941d0-113">Files.Read</span></span>    |
|<span data-ttu-id="941d0-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="941d0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="941d0-115">Files.Read</span><span class="sxs-lookup"><span data-stu-id="941d0-115">Files.Read</span></span>    |
|<span data-ttu-id="941d0-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="941d0-116">Application</span></span> | <span data-ttu-id="941d0-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="941d0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="941d0-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="941d0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="941d0-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="941d0-119">Optional query parameters</span></span>
<span data-ttu-id="941d0-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="941d0-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="941d0-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="941d0-121">Request headers</span></span>
| <span data-ttu-id="941d0-122">名前</span><span class="sxs-lookup"><span data-stu-id="941d0-122">Name</span></span>       | <span data-ttu-id="941d0-123">型</span><span class="sxs-lookup"><span data-stu-id="941d0-123">Type</span></span> | <span data-ttu-id="941d0-124">説明</span><span class="sxs-lookup"><span data-stu-id="941d0-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="941d0-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="941d0-125">Authorization</span></span>  | <span data-ttu-id="941d0-126">string</span><span class="sxs-lookup"><span data-stu-id="941d0-126">string</span></span>  | <span data-ttu-id="941d0-p103">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="941d0-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="941d0-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="941d0-129">Request body</span></span>
<span data-ttu-id="941d0-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="941d0-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="941d0-131">応答</span><span class="sxs-lookup"><span data-stu-id="941d0-131">Response</span></span>

<span data-ttu-id="941d0-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で[写真](../resources/photo.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="941d0-132">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="941d0-133">例</span><span class="sxs-lookup"><span data-stu-id="941d0-133">Examples</span></span>
##### <a name="request"></a><span data-ttu-id="941d0-134">要求</span><span class="sxs-lookup"><span data-stu-id="941d0-134">Request</span></span>
<span data-ttu-id="941d0-135">以下は、写真のメタデータに対する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="941d0-135">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="941d0-136">応答</span><span class="sxs-lookup"><span data-stu-id="941d0-136">Response</span></span>
<span data-ttu-id="941d0-137">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="941d0-137">Here is an example of the response.</span></span>
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
##### <a name="request"></a><span data-ttu-id="941d0-138">要求</span><span class="sxs-lookup"><span data-stu-id="941d0-138">Request</span></span>
<span data-ttu-id="941d0-139">以下は、写真のバイト数に対する要求の例です。</span><span class="sxs-lookup"><span data-stu-id="941d0-139">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/beta/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="941d0-140">応答</span><span class="sxs-lookup"><span data-stu-id="941d0-140">Response</span></span>
<span data-ttu-id="941d0-141">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="941d0-141">Here is an example of the response.</span></span>

<!-- { "blockType": "ignored","@odata.type": "stream" } -->

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




<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
