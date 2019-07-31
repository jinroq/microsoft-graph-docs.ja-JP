---
author: JeremyKelley
ms.author: jeremyke
title: バンドルの削除
description: ドライブ項目のバンドルを削除する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 5854daeabf14e69ec859fe04563e0ee68d76ed22
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944823"
---
# <a name="delete-bundle"></a><span data-ttu-id="c2360-103">バンドルの削除</span><span class="sxs-lookup"><span data-stu-id="c2360-103">Delete bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2360-104">**Id**を使用して、ドライブ項目の[バンドル][]を削除します。この方法を使用してバンドルを削除すると、そのバンドルが完全に削除され、ごみ箱に移動されないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="c2360-104">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="c2360-105">ただし、バンドルによって参照されていたアイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="c2360-105">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="c2360-106">それらは親フォルダーに残ります。</span><span class="sxs-lookup"><span data-stu-id="c2360-106">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2360-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="c2360-107">Permissions</span></span>

<span data-ttu-id="c2360-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2360-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2360-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c2360-110">Permission type</span></span>      | <span data-ttu-id="c2360-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="c2360-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2360-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c2360-112">Delegated (work or school account)</span></span> | <span data-ttu-id="c2360-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2360-113">Not supported.</span></span>                             |
|<span data-ttu-id="c2360-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c2360-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2360-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2360-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="c2360-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c2360-116">Application</span></span>          | <span data-ttu-id="c2360-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c2360-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="c2360-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c2360-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="c2360-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c2360-119">Request headers</span></span>

| <span data-ttu-id="c2360-120">名前</span><span class="sxs-lookup"><span data-stu-id="c2360-120">Name</span></span>          | <span data-ttu-id="c2360-121">説明</span><span class="sxs-lookup"><span data-stu-id="c2360-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="c2360-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2360-122">Authorization</span></span> | <span data-ttu-id="c2360-123">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="c2360-123">Bearer \{token\}.</span></span> <span data-ttu-id="c2360-124">必須。</span><span class="sxs-lookup"><span data-stu-id="c2360-124">Required.</span></span> |
| <span data-ttu-id="c2360-125">if-match</span><span class="sxs-lookup"><span data-stu-id="c2360-125">if-match</span></span>      | <span data-ttu-id="c2360-126">eTag.</span><span class="sxs-lookup"><span data-stu-id="c2360-126">eTag.</span></span> <span data-ttu-id="c2360-127">省略可能。</span><span class="sxs-lookup"><span data-stu-id="c2360-127">Optional.</span></span> <span data-ttu-id="c2360-128">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がバンドルの現在の`412 Precondition Failed`タグと一致しない場合は、応答が返され、バンドルは削除されません。</span><span class="sxs-lookup"><span data-stu-id="c2360-128">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="c2360-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="c2360-129">Request body</span></span>

<span data-ttu-id="c2360-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c2360-130">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="c2360-131">応答</span><span class="sxs-lookup"><span data-stu-id="c2360-131">Response</span></span>

<span data-ttu-id="c2360-132">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="c2360-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="c2360-133">エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2360-133">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="c2360-134">例</span><span class="sxs-lookup"><span data-stu-id="c2360-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2360-135">要求</span><span class="sxs-lookup"><span data-stu-id="c2360-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2360-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="c2360-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2360-137">C#</span><span class="sxs-lookup"><span data-stu-id="c2360-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2360-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="c2360-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2360-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="c2360-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="c2360-140">Java</span><span class="sxs-lookup"><span data-stu-id="c2360-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c2360-141">応答</span><span class="sxs-lookup"><span data-stu-id="c2360-141">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[バンドル]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Delete a bundle from OneDrive",
  "keywords": "delete,existing bundle,onedrive",
  "section": "documentation",
  "tocPath": "Bundles/Delete"
} -->
