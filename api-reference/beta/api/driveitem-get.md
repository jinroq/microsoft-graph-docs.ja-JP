---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーを取得する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: a238e1dd459ee04d5c6c7c3453edaac2d569ed84
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33589313"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="e0ccf-102">DriveItem リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="e0ccf-102">Get a DriveItem resource</span></span>

<span data-ttu-id="e0ccf-103">[ドライブ](../resources/drive.md) 内の [DriveItem](../resources/driveitem.md) 用のメタデータを、ファイル システム パスまたは ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-103">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0ccf-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e0ccf-104">Permissions</span></span>

<span data-ttu-id="e0ccf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0ccf-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e0ccf-107">Permission type</span></span>      | <span data-ttu-id="e0ccf-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e0ccf-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e0ccf-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e0ccf-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e0ccf-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ccf-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0ccf-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e0ccf-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0ccf-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ccf-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="e0ccf-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e0ccf-113">Application</span></span> | <span data-ttu-id="e0ccf-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0ccf-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0ccf-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e0ccf-115">HTTP request</span></span>

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

## <a name="optional-query-parameters"></a><span data-ttu-id="e0ccf-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e0ccf-116">Optional query parameters</span></span>

<span data-ttu-id="e0ccf-117">このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-117">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="e0ccf-118">アイテムが**子**関係にある場合、[`$expand` クエリ文字列パラメーター](/graph/query-parameters) を使って、アイテムのメタデータを取得するのと同じように、同一呼び出し内のアイテムの子を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-118">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="e0ccf-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0ccf-119">Optional request headers</span></span>

| <span data-ttu-id="e0ccf-120">名前</span><span class="sxs-lookup"><span data-stu-id="e0ccf-120">Name</span></span>          | <span data-ttu-id="e0ccf-121">値</span><span class="sxs-lookup"><span data-stu-id="e0ccf-121">Value</span></span>  | <span data-ttu-id="e0ccf-122">説明</span><span class="sxs-lookup"><span data-stu-id="e0ccf-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="e0ccf-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="e0ccf-123">if-none-match</span></span> | <span data-ttu-id="e0ccf-124">String</span><span class="sxs-lookup"><span data-stu-id="e0ccf-124">String</span></span> | <span data-ttu-id="e0ccf-125">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="e0ccf-126">応答</span><span class="sxs-lookup"><span data-stu-id="e0ccf-126">Response</span></span>

<span data-ttu-id="e0ccf-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0ccf-128">例</span><span class="sxs-lookup"><span data-stu-id="e0ccf-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0ccf-129">要求</span><span class="sxs-lookup"><span data-stu-id="e0ccf-129">Request</span></span>

<span data-ttu-id="e0ccf-130">以下は、ユーザーの OneDrive のルート フォルダーへの要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "get-drive-root", "tags": "service.graph" }-->

```http
GET /me/drive/root
```

## <a name="response"></a><span data-ttu-id="e0ccf-131">応答</span><span class="sxs-lookup"><span data-stu-id="e0ccf-131">Response</span></span>

<span data-ttu-id="e0ccf-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-132">Here is an example of the response.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e0ccf-133">SDK サンプル コード</span><span class="sxs-lookup"><span data-stu-id="e0ccf-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e0ccf-134">C#</span><span class="sxs-lookup"><span data-stu-id="e0ccf-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-root-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e0ccf-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="e0ccf-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-root-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="remarks"></a><span data-ttu-id="e0ccf-136">注釈</span><span class="sxs-lookup"><span data-stu-id="e0ccf-136">Remarks</span></span>

<span data-ttu-id="e0ccf-137">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e0ccf-137">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

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
    "Error: /api-reference/v1.0/api/driveitem-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
