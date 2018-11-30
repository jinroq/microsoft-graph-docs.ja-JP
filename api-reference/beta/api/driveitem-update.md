---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: ファイルまたはフォルダーを更新する
ms.openlocfilehash: 90fab8a4cfafdbff888e53f968a67fa34c0599d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071397"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="82c01-102">DriveItem プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="82c01-102">Update DriveItem properties</span></span>

> <span data-ttu-id="82c01-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="82c01-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82c01-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82c01-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="82c01-105">[DriveItem](../resources/driveitem.md) のメタデータを、ID またはパスで更新します。</span><span class="sxs-lookup"><span data-stu-id="82c01-105">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="82c01-106">別の親に[アイテムを移動](driveitem-move.md)するために更新を使用することもできます。その場合は、アイテムの **parentReference** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="82c01-106">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="82c01-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="82c01-107">Permissions</span></span>

<span data-ttu-id="82c01-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82c01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82c01-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82c01-110">Permission type</span></span>      | <span data-ttu-id="82c01-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="82c01-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="82c01-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82c01-112">Delegated (work or school account)</span></span> | <span data-ttu-id="82c01-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c01-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="82c01-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82c01-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="82c01-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c01-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="82c01-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82c01-116">Application</span></span> | <span data-ttu-id="82c01-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82c01-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="82c01-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82c01-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="82c01-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82c01-119">Optional request headers</span></span>

| <span data-ttu-id="82c01-120">名前</span><span class="sxs-lookup"><span data-stu-id="82c01-120">Name</span></span>          | <span data-ttu-id="82c01-121">型</span><span class="sxs-lookup"><span data-stu-id="82c01-121">Type</span></span>   | <span data-ttu-id="82c01-122">説明</span><span class="sxs-lookup"><span data-stu-id="82c01-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="82c01-123">if-match</span><span class="sxs-lookup"><span data-stu-id="82c01-123">if-match</span></span>      | <span data-ttu-id="82c01-124">String</span><span class="sxs-lookup"><span data-stu-id="82c01-124">String</span></span> | <span data-ttu-id="82c01-125">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="82c01-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="82c01-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="82c01-126">Request body</span></span>

<span data-ttu-id="82c01-127">要求本文で、更新すべきプロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="82c01-127">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="82c01-128">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="82c01-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="82c01-129">最高のパフォーマンスのためには、変更されていないプロパティをアプリケーションに含めないでください。</span><span class="sxs-lookup"><span data-stu-id="82c01-129">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="82c01-130">応答</span><span class="sxs-lookup"><span data-stu-id="82c01-130">Response</span></span>

<span data-ttu-id="82c01-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="82c01-131">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82c01-132">例</span><span class="sxs-lookup"><span data-stu-id="82c01-132">Example</span></span>

<span data-ttu-id="82c01-133">この例では、DriveItem リソースを「new-file-name.docx」という名前に変更します。</span><span class="sxs-lookup"><span data-stu-id="82c01-133">This example renames the DriveItem resource to "new-file-name.docx".</span></span>

<!-- { "blockType": "request", "name": "update-item" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```

### <a name="response"></a><span data-ttu-id="82c01-134">応答</span><span class="sxs-lookup"><span data-stu-id="82c01-134">Response</span></span>

<span data-ttu-id="82c01-135">成功した場合、このメソッドは応答本文で [driveItem][item-resource] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="82c01-135">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="82c01-136">エラー応答</span><span class="sxs-lookup"><span data-stu-id="82c01-136">Error responses</span></span>

<span data-ttu-id="82c01-137">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82c01-137">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update"
} -->
