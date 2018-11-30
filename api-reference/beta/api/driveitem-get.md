---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルまたはフォルダーを取得する
ms.openlocfilehash: 1ad021e724c807bf15e777b5438c22b5a532a4aa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071115"
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="aac03-102">DriveItem リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="aac03-102">Get a DriveItem resource</span></span>

> <span data-ttu-id="aac03-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="aac03-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aac03-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aac03-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aac03-105">[ドライブ](../resources/drive.md) 内の [DriveItem](../resources/driveitem.md) 用のメタデータを、ファイル システム パスまたは ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="aac03-105">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="aac03-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="aac03-106">Permissions</span></span>

<span data-ttu-id="aac03-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aac03-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aac03-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aac03-109">Permission type</span></span>      | <span data-ttu-id="aac03-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="aac03-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aac03-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aac03-111">Delegated (work or school account)</span></span> | <span data-ttu-id="aac03-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac03-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="aac03-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aac03-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aac03-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac03-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="aac03-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aac03-115">Application</span></span> | <span data-ttu-id="aac03-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aac03-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aac03-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aac03-117">HTTP request</span></span>

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

## <a name="optional-query-parameters"></a><span data-ttu-id="aac03-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="aac03-118">Optional query parameters</span></span>

<span data-ttu-id="aac03-119">このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="aac03-119">This method supports the `$expand` and `$select` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<span data-ttu-id="aac03-120">アイテムが**子**関係にある場合、[`$expand` クエリ文字列パラメーター](/graph/query-parameters) を使って、アイテムのメタデータを取得するのと同じように、同一呼び出し内のアイテムの子を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="aac03-120">You can use the [`$expand` query string parameter](/graph/query-parameters) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="aac03-121">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aac03-121">Optional request headers</span></span>

| <span data-ttu-id="aac03-122">名前</span><span class="sxs-lookup"><span data-stu-id="aac03-122">Name</span></span>          | <span data-ttu-id="aac03-123">値</span><span class="sxs-lookup"><span data-stu-id="aac03-123">Value</span></span>  | <span data-ttu-id="aac03-124">説明</span><span class="sxs-lookup"><span data-stu-id="aac03-124">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="aac03-125">if-none-match</span><span class="sxs-lookup"><span data-stu-id="aac03-125">if-none-match</span></span> | <span data-ttu-id="aac03-126">String</span><span class="sxs-lookup"><span data-stu-id="aac03-126">String</span></span> | <span data-ttu-id="aac03-127">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="aac03-127">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="aac03-128">応答</span><span class="sxs-lookup"><span data-stu-id="aac03-128">Response</span></span>

<span data-ttu-id="aac03-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="aac03-129">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aac03-130">例</span><span class="sxs-lookup"><span data-stu-id="aac03-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="aac03-131">要求</span><span class="sxs-lookup"><span data-stu-id="aac03-131">Request</span></span>

<span data-ttu-id="aac03-132">以下は、ユーザーの OneDrive のルート フォルダーへの要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aac03-132">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "get-item-metadata" }-->

```http
GET /me/drive/root
```

## <a name="response"></a><span data-ttu-id="aac03-133">応答</span><span class="sxs-lookup"><span data-stu-id="aac03-133">Response</span></span>

<span data-ttu-id="aac03-134">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="aac03-134">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="aac03-135">備考</span><span class="sxs-lookup"><span data-stu-id="aac03-135">Remarks</span></span>

<span data-ttu-id="aac03-136">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aac03-136">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors
[odata-parameters]: /graph/query-parameters
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive-get-specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item"
} -->
