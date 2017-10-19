---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "ファイルまたはフォルダーを取得する"
ms.openlocfilehash: 94f6981d817de638878f4876104f049ebfa383c7
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="get-a-driveitem-resource"></a><span data-ttu-id="79c5f-102">DriveItem リソースを取得する</span><span class="sxs-lookup"><span data-stu-id="79c5f-102">Get a DriveItem resource</span></span>

<span data-ttu-id="79c5f-103">[ドライブ](../resources/drive.md) 内の [DriveItem](../resources/driveitem.md) 用のメタデータを、ファイル システム パスまたは ID で取得します。</span><span class="sxs-lookup"><span data-stu-id="79c5f-103">Retrieve the metadata for a [DriveItem](../resources/driveitem.md) in a [Drive](../resources/drive.md) by file system path or ID.</span></span>

## <a name="permissions"></a><span data-ttu-id="79c5f-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="79c5f-104">Permissions</span></span>

<span data-ttu-id="79c5f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79c5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="79c5f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="79c5f-107">Permission type</span></span>      | <span data-ttu-id="79c5f-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="79c5f-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="79c5f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="79c5f-109">Delegated (work or school account)</span></span> | <span data-ttu-id="79c5f-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79c5f-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="79c5f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="79c5f-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79c5f-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79c5f-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="79c5f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="79c5f-113">Application</span></span> | <span data-ttu-id="79c5f-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79c5f-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="79c5f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="79c5f-115">HTTP request</span></span>

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

## <a name="optional-query-parameters"></a><span data-ttu-id="79c5f-116">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="79c5f-116">Optional query parameters</span></span>

<span data-ttu-id="79c5f-117">このメソッドは、応答をカスタマイズするための `$expand` と `$select` の [OData クエリ パラメーター](../../../concepts/query_parameters.md)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="79c5f-117">This method supports the `$expand` and `$select` [OData query parameters](../../../concepts/query_parameters.md) to customize the response.</span></span>

<span data-ttu-id="79c5f-118">アイテムが**子**関係にある場合、[`$expand` クエリ文字列パラメーター](../../../concepts/query_parameters.md) を使って、アイテムのメタデータを取得するのと同じように、同一呼び出し内のアイテムの子を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="79c5f-118">You can use the [`$expand` query string parameter](../../../concepts/query_parameters.md) to include the children of an item in the same call as retrieving the metadata of an item if the item has a **children** relationship.</span></span>

## <a name="optional-request-headers"></a><span data-ttu-id="79c5f-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="79c5f-119">Optional request headers</span></span>

| <span data-ttu-id="79c5f-120">名前</span><span class="sxs-lookup"><span data-stu-id="79c5f-120">Name</span></span>          | <span data-ttu-id="79c5f-121">値</span><span class="sxs-lookup"><span data-stu-id="79c5f-121">Value</span></span>  | <span data-ttu-id="79c5f-122">説明</span><span class="sxs-lookup"><span data-stu-id="79c5f-122">Description</span></span>                                                                                                                                              |
|:--------------|:-------|:---------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="79c5f-123">if-none-match</span><span class="sxs-lookup"><span data-stu-id="79c5f-123">if-none-match</span></span> | <span data-ttu-id="79c5f-124">String</span><span class="sxs-lookup"><span data-stu-id="79c5f-124">String</span></span> | <span data-ttu-id="79c5f-125">この要求ヘッダーが含まれている場合、指定された eTag (または cTag) がファイルの現在のタグに一致すると、`HTTP 304 Not Modified` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="79c5f-125">If this request header is included and the eTag (or cTag) provided matches the current tag on the file, an `HTTP 304 Not Modified` response is returned.</span></span> |

## <a name="response"></a><span data-ttu-id="79c5f-126">応答</span><span class="sxs-lookup"><span data-stu-id="79c5f-126">Response</span></span>

<span data-ttu-id="79c5f-127">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="79c5f-127">If successful, this method returns a `200 OK` response code and the [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79c5f-128">例</span><span class="sxs-lookup"><span data-stu-id="79c5f-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="79c5f-129">要求</span><span class="sxs-lookup"><span data-stu-id="79c5f-129">Request</span></span>

<span data-ttu-id="79c5f-130">以下は、ユーザーの OneDrive のルート フォルダーへの要求の例です。</span><span class="sxs-lookup"><span data-stu-id="79c5f-130">Here is an example of the request to the root folder of the user's OneDrive.</span></span>

<!-- { "blockType": "request", "name": "get-item-metadata" }-->

```http
GET /me/drive/root
```

## <a name="response"></a><span data-ttu-id="79c5f-131">応答</span><span class="sxs-lookup"><span data-stu-id="79c5f-131">Response</span></span>

<span data-ttu-id="79c5f-132">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="79c5f-132">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="79c5f-133">備考</span><span class="sxs-lookup"><span data-stu-id="79c5f-133">Remarks</span></span>

<span data-ttu-id="79c5f-134">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="79c5f-134">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: ../../../concepts/errors.md
[odata-parameters]: ../../../concepts/query_parameters.md
[item-resource]: ../resources/driveitem.md
[special-folder]: ../api/drive_get_specialfolder.md

<!-- {
  "type": "#page.annotation",
  "description": "Retrieve metadata about an item and its children in OneDrive",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Items/Get item"
} -->
