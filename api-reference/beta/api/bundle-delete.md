---
author: JeremyKelley
ms.author: jeremyke
title: バンドルの削除
description: ドライブ項目のバンドルを削除する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 7556edc226f655af748facea1df6ea19820b7c9e
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419260"
---
# <a name="delete-bundle"></a><span data-ttu-id="3b569-103">バンドルの削除</span><span class="sxs-lookup"><span data-stu-id="3b569-103">Delete bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3b569-104">**Id**を使用して、ドライブ項目の[バンドル][]を削除します。この方法を使用してバンドルを削除すると、そのバンドルが完全に削除され、ごみ箱に移動されないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3b569-104">Delete a [bundle][] of driveItems by using its **id**. Note that deleting a bundle using this method permanently deletes the bundle and does not move it to the Recycle Bin.</span></span>
<span data-ttu-id="3b569-105">ただし、バンドルによって参照されていたアイテムは削除されません。</span><span class="sxs-lookup"><span data-stu-id="3b569-105">It does not, however, remove the items that were referenced by the bundle.</span></span>
<span data-ttu-id="3b569-106">それらは親フォルダーに残ります。</span><span class="sxs-lookup"><span data-stu-id="3b569-106">They will remain in their parent folders.</span></span>

## <a name="permissions"></a><span data-ttu-id="3b569-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="3b569-107">Permissions</span></span>

<span data-ttu-id="3b569-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b569-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b569-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b569-110">Permission type</span></span>      | <span data-ttu-id="3b569-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b569-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3b569-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b569-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3b569-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b569-113">Not supported.</span></span>                             |
|<span data-ttu-id="3b569-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b569-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3b569-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b569-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="3b569-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b569-116">Application</span></span>          | <span data-ttu-id="3b569-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b569-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="3b569-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b569-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="3b569-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b569-119">Request headers</span></span>

| <span data-ttu-id="3b569-120">名前</span><span class="sxs-lookup"><span data-stu-id="3b569-120">Name</span></span>          | <span data-ttu-id="3b569-121">説明</span><span class="sxs-lookup"><span data-stu-id="3b569-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="3b569-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b569-122">Authorization</span></span> | <span data-ttu-id="3b569-123">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="3b569-123">Bearer \{token\}.</span></span> <span data-ttu-id="3b569-124">必須。</span><span class="sxs-lookup"><span data-stu-id="3b569-124">Required.</span></span> |
| <span data-ttu-id="3b569-125">if-match</span><span class="sxs-lookup"><span data-stu-id="3b569-125">if-match</span></span>      | <span data-ttu-id="3b569-126">eTag.</span><span class="sxs-lookup"><span data-stu-id="3b569-126">eTag.</span></span> <span data-ttu-id="3b569-127">省略可能。</span><span class="sxs-lookup"><span data-stu-id="3b569-127">Optional.</span></span> <span data-ttu-id="3b569-128">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がバンドルの現在の`412 Precondition Failed`タグと一致しない場合は、応答が返され、バンドルは削除されません。</span><span class="sxs-lookup"><span data-stu-id="3b569-128">If this request header is included and the eTag (or cTag) provided does not match the current tag on the bundle, a `412 Precondition Failed` response is returned and the bundle will not be deleted.</span></span>

## <a name="request-body"></a><span data-ttu-id="3b569-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b569-129">Request body</span></span>

<span data-ttu-id="3b569-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="3b569-130">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="3b569-131">応答</span><span class="sxs-lookup"><span data-stu-id="3b569-131">Response</span></span>

<span data-ttu-id="3b569-132">成功した場合、この呼び出しはリソースが削除され返すものがなかったことを示す `204 No Content` 応答を返します。</span><span class="sxs-lookup"><span data-stu-id="3b569-132">If successful, this call returns a `204 No Content` response to indicate that resource was deleted and there was nothing to return.</span></span>

<span data-ttu-id="3b569-133">エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b569-133">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="3b569-134">例</span><span class="sxs-lookup"><span data-stu-id="3b569-134">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b569-135">要求</span><span class="sxs-lookup"><span data-stu-id="3b569-135">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="3b569-136">プロトコル</span><span class="sxs-lookup"><span data-stu-id="3b569-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "delete-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/items/{bundle-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="3b569-137">C#</span><span class="sxs-lookup"><span data-stu-id="3b569-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3b569-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3b569-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="3b569-139">目的-C</span><span class="sxs-lookup"><span data-stu-id="3b569-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3b569-140">応答</span><span class="sxs-lookup"><span data-stu-id="3b569-140">Response</span></span>

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
