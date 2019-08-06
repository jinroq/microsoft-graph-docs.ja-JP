---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーを取得する
localization_priority: Priority
ms.prod: sharepoint
description: ドライブ内の DriveItem 用のメタデータを、ファイル システム パスまたは ID で取得します。
doc_type: apiPageType
ms.openlocfilehash: 6760af3b9cf28d325fcda325937f91ed417e2651
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015440"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="3feb4-103">DriveItem リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="3feb4-103">Get a DriveItem resource</span></span>

<span data-ttu-id="3feb4-104">[ドライブ](../resources/drive.md) 内の [DriveItem](../resources/driveitem.md) 用のメタデータを、ファイル システム パスまたは ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="3feb4-104">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="3feb4-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3feb4-105">Permissions</span></span>

<span data-ttu-id="3feb4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3feb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3feb4-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3feb4-108">Permission type</span></span>      | <span data-ttu-id="3feb4-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3feb4-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3feb4-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3feb4-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3feb4-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3feb4-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3feb4-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3feb4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3feb4-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3feb4-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3feb4-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3feb4-114">Application</span></span> | <span data-ttu-id="3feb4-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3feb4-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3feb4-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3feb4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drives/{drive-id}/items/{item-id}
GET /drives/{drive-id}/root:/{item-path}
GET /groups/{group-id}/drive/items/{item-id}
GET /groups/{group-id}/drive/root:/{item-path}
GET /me/drive/items/{item-id}
GET /me/drive/root:/{item-path}
GET /sites/{siteId}/drive/items/{itemId}
GET /sites/{siteId}/drive/root:/{item-path}
GET /users/{userId}/drive/items/{itemId}
GET /users/{userId}/drive/root:/{item-path}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3feb4-117">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="3feb4-117">Optional query parameters</span></span>

<span data-ttu-id="3feb4-118">このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="3feb4-118">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="3feb4-119">アイテムが**子**関係にある場合、[`$expand` クエリ文字列パラメーター](/graph/query-parameters) を使って、アイテムのメタデータを取得するのと同じように、同一呼び出し内のアイテムの子を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="3feb4-119">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="3feb4-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3feb4-120">Optional request headers</span></span>

| <span data-ttu-id="3feb4-121">名前</span><span class="sxs-lookup"><span data-stu-id="3feb4-121">Name</span></span>          | <span data-ttu-id="3feb4-122">値</span><span class="sxs-lookup"><span data-stu-id="3feb4-122">Value</span></span>  | <span data-ttu-id="3feb4-123">説明</span><span class="sxs-lookup"><span data-stu-id="3feb4-123">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="3feb4-124">if-none-match</span><span class="sxs-lookup"><span data-stu-id="3feb4-124">if-none-match</span></span> | <span data-ttu-id="3feb4-125">String</span><span class="sxs-lookup"><span data-stu-id="3feb4-125">String</span></span> | <span data-ttu-id="3feb4-126">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="3feb4-126">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="3feb4-127">応答</span><span class="sxs-lookup"><span data-stu-id="3feb4-127">Response</span></span>

<span data-ttu-id="3feb4-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="3feb4-128">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3feb4-129">例</span><span class="sxs-lookup"><span data-stu-id="3feb4-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="3feb4-130">要求</span><span class="sxs-lookup"><span data-stu-id="3feb4-130">Request</span></span>

<span data-ttu-id="3feb4-131">以下は、ユーザーの OneDrive のルート フォルダーへの要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3feb4-131">Here is an example of the request to the root folder of the user's OneDrive.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3feb4-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="3feb4-132">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-root", "tags": "service.graph" }-->

```http
GET /me/drive/root
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3feb4-133">C#</span><span class="sxs-lookup"><span data-stu-id="3feb4-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-root-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3feb4-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="3feb4-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-root-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3feb4-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3feb4-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-root-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="3feb4-136">Java</span><span class="sxs-lookup"><span data-stu-id="3feb4-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-root-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="response"></a><span data-ttu-id="3feb4-137">応答</span><span class="sxs-lookup"><span data-stu-id="3feb4-137">Response</span></span>

<span data-ttu-id="3feb4-138">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="3feb4-138">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.driveItem" } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "createdBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "createdDateTime": "2016-03-21T20:01:37Z",
  "cTag": "\"c:{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},0\"",
  "eTag": "\"{86EB4C8E-D20D-46B9-AD41-23B8868DDA8A},1\"",
  "folder": { "childCount": 120 },
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "lastModifiedBy": {
      "user": {
          "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
          "displayName": "Ryan Gregg"
      }
  },
  "lastModifiedDateTime": "2016-03-21T20:01:37Z",
  "name": "OneDrive",
  "root": { },
  "size": 157286400,
  "webUrl": "https://contoso-my.sharepoint.com/personal/rgregg_contoso_com/Documents"
}
```

## <a name="remarks"></a><span data-ttu-id="3feb4-139">注釈</span><span class="sxs-lookup"><span data-stu-id="3feb4-139">Remarks</span></span>

<span data-ttu-id="3feb4-140">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3feb4-140">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item",
  "suppressions": [
  ]
} -->
