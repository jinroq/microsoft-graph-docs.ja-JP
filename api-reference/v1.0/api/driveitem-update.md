---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーを更新する
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 7ec2ff2c438588074783e953598509eed1730f90
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35881614"
---
# <a name="update-driveitem-properties"></a><span data-ttu-id="ec0e1-102">DriveItem プロパティを更新する</span><span class="sxs-lookup"><span data-stu-id="ec0e1-102">Update DriveItem properties</span></span>

<span data-ttu-id="ec0e1-103">[DriveItem](../resources/driveitem.md) のメタデータを、ID またはパスで更新します。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-103">Update the metadata for a [DriveItem](../resources/driveitem.md) by ID or path.</span></span>

<span data-ttu-id="ec0e1-104">別の親に[アイテムを移動](driveitem-move.md)するために更新を使用することもできます。その場合は、アイテムの **parentReference** プロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-104">You can also use update to [move an item](driveitem-move.md) to another parent by updating the item's **parentReference** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="ec0e1-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ec0e1-105">Permissions</span></span>

<span data-ttu-id="ec0e1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec0e1-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec0e1-108">Permission type</span></span>      | <span data-ttu-id="ec0e1-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec0e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ec0e1-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec0e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ec0e1-111">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec0e1-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ec0e1-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec0e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ec0e1-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec0e1-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="ec0e1-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec0e1-114">Application</span></span> | <span data-ttu-id="ec0e1-115">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec0e1-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ec0e1-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec0e1-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/items/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="ec0e1-117">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec0e1-117">Optional request headers</span></span>

| <span data-ttu-id="ec0e1-118">名前</span><span class="sxs-lookup"><span data-stu-id="ec0e1-118">Name</span></span>          | <span data-ttu-id="ec0e1-119">型</span><span class="sxs-lookup"><span data-stu-id="ec0e1-119">Type</span></span>   | <span data-ttu-id="ec0e1-120">説明</span><span class="sxs-lookup"><span data-stu-id="ec0e1-120">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ec0e1-121">if-match</span><span class="sxs-lookup"><span data-stu-id="ec0e1-121">if-match</span></span>      | <span data-ttu-id="ec0e1-122">String</span><span class="sxs-lookup"><span data-stu-id="ec0e1-122">String</span></span> | <span data-ttu-id="ec0e1-123">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-123">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ec0e1-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec0e1-124">Request body</span></span>

<span data-ttu-id="ec0e1-125">要求本文で、更新すべきプロパティの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-125">In the request body, supply the values for properties that should be updated.</span></span>

<span data-ttu-id="ec0e1-126">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-126">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span>
<span data-ttu-id="ec0e1-127">最高のパフォーマンスのためには、変更されていないプロパティをアプリケーションに含めないでください。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-127">For best performance your app should not include properties that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="ec0e1-128">応答</span><span class="sxs-lookup"><span data-stu-id="ec0e1-128">Response</span></span>

<span data-ttu-id="ec0e1-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-129">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec0e1-130">例</span><span class="sxs-lookup"><span data-stu-id="ec0e1-130">Example</span></span>

<span data-ttu-id="ec0e1-131">この例では、DriveItem リソースを「new-file-name.docx」という名前に変更します。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-131">This example renames the DriveItem resource to "new-file-name.docx".</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="ec0e1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ec0e1-132">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "update-item", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "name": "new-file-name.docx"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ec0e1-133">C#</span><span class="sxs-lookup"><span data-stu-id="ec0e1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ec0e1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="ec0e1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ec0e1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ec0e1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ec0e1-136">Java</span><span class="sxs-lookup"><span data-stu-id="ec0e1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ec0e1-137">応答</span><span class="sxs-lookup"><span data-stu-id="ec0e1-137">Response</span></span>

<span data-ttu-id="ec0e1-138">成功した場合、このメソッドでは応答本文の [driveItem][item-resource] リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-138">If successful, this method returns an [driveItem][item-resource] resource in the response body.</span></span>

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

## <a name="error-responses"></a><span data-ttu-id="ec0e1-139">エラー応答</span><span class="sxs-lookup"><span data-stu-id="ec0e1-139">Error responses</span></span>

<span data-ttu-id="ec0e1-140">エラーがどのように返されるかの詳細については、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec0e1-140">See [Error Responses][error-response] for details about how errors are returned.</span></span>

[error-response]: /graph/errors
[item-resource]: ../resources/driveitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of an item.",
  "keywords": "update,replace,contents,item",
  "section": "documentation",
  "tocPath": "Items/Update",
  "suppressions": [
  ]
} -->
