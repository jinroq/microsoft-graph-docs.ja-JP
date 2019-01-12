---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルまたはフォルダーを更新する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: de95ea9263bb3491bfcb02168cb26e1eb3cb94c7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950936"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="68e78-102">DriveItem プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="68e78-102">Update DriveItem properties</span></span>

<span data-ttu-id="68e78-103">[DriveItem](../resources/driveitem.md) のメタデータを、ID またはパスで更新します。</span><span class="sxs-lookup"><span data-stu-id="68e78-103">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="68e78-104">別の親に[アイテムを移動](driveitem-move.md)するために更新を使用することもできます。その場合は、アイテムの **parentReference** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="68e78-104">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="68e78-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="68e78-105">Permissions</span></span>

<span data-ttu-id="68e78-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68e78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68e78-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68e78-108">Permission type</span></span>      | <span data-ttu-id="68e78-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="68e78-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68e78-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68e78-110">Delegated (work or school account)</span></span> | <span data-ttu-id="68e78-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68e78-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="68e78-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68e78-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68e78-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68e78-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="68e78-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68e78-114">Application</span></span> | <span data-ttu-id="68e78-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68e78-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68e78-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68e78-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="68e78-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68e78-117">Optional request headers</span></span>

| <span data-ttu-id="68e78-118">名前</span><span class="sxs-lookup"><span data-stu-id="68e78-118">Name</span></span>          | <span data-ttu-id="68e78-119">種類</span><span class="sxs-lookup"><span data-stu-id="68e78-119">Type</span></span>   | <span data-ttu-id="68e78-120">説明</span><span class="sxs-lookup"><span data-stu-id="68e78-120">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="68e78-121">if-match</span><span class="sxs-lookup"><span data-stu-id="68e78-121">if-match</span></span>      | <span data-ttu-id="68e78-122">String</span><span class="sxs-lookup"><span data-stu-id="68e78-122">String</span></span> | <span data-ttu-id="68e78-123">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="68e78-123">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68e78-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="68e78-124">Request body</span></span>

<span data-ttu-id="68e78-125">要求本文で、更新すべきプロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="68e78-125">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="68e78-126">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="68e78-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="68e78-127">最高のパフォーマンスのためには、変更されていないプロパティをアプリケーションに含めないでください。</span><span class="sxs-lookup"><span data-stu-id="68e78-127">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="68e78-128">応答</span><span class="sxs-lookup"><span data-stu-id="68e78-128">Response</span></span>

<span data-ttu-id="68e78-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="68e78-129">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68e78-130">例</span><span class="sxs-lookup"><span data-stu-id="68e78-130">Example</span></span>

<span data-ttu-id="68e78-131">この例では、DriveItem リソースを「new-file-name.docx」という名前に変更します。</span><span class="sxs-lookup"><span data-stu-id="68e78-131">This example renames the DriveItem resource to "new-file-name.docx".</span></span>

<!-- { "blockType": "request", "name": "update-item", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```

### <a name="response"></a><span data-ttu-id="68e78-132">応答</span><span class="sxs-lookup"><span data-stu-id="68e78-132">Response</span></span>

<span data-ttu-id="68e78-133">成功した場合、このメソッドは応答本文で [driveItem][item-resource] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="68e78-133">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "01NKDM7HMOJTVYMDOSXFDK2QJDXCDI3WUK",
  "name": "new-file-name.docx",
  "file": { }
}
```

## <a name="error-responses"></a><span data-ttu-id="68e78-134">エラー応答</span><span class="sxs-lookup"><span data-stu-id="68e78-134">Error responses</span></span>

<span data-ttu-id="68e78-135">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68e78-135">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update"
} -->
