---
author: JeremyKelley
ms.author: jeremyke
title: バンドルからのアイテムの削除
description: ドライブ項目のバンドルから項目を削除する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ff7f292be35b59f17465e65517174746faddca1a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35944810"
---
# <a name="remove-item-from-bundle"></a><span data-ttu-id="69f72-103">バンドルからのアイテムの削除</span><span class="sxs-lookup"><span data-stu-id="69f72-103">Remove item from bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69f72-104">[バンドル][]からアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="69f72-104">Remove an item from a [bundle][].</span></span>

## <a name="permissions"></a><span data-ttu-id="69f72-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="69f72-105">Permissions</span></span>

<span data-ttu-id="69f72-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69f72-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69f72-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69f72-108">Permission type</span></span>      | <span data-ttu-id="69f72-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="69f72-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="69f72-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69f72-110">Delegated (work or school account)</span></span> | <span data-ttu-id="69f72-111">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69f72-111">Not supported.</span></span>                             |
|<span data-ttu-id="69f72-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69f72-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="69f72-113">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69f72-113">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="69f72-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69f72-114">Application</span></span>          | <span data-ttu-id="69f72-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69f72-115">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="69f72-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69f72-116">HTTP request</span></span>

```http
DELETE /drive/bundles/{bundle-id}/children/{item-id}
```

## <a name="request-headers"></a><span data-ttu-id="69f72-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69f72-117">Request headers</span></span>

| <span data-ttu-id="69f72-118">名前</span><span class="sxs-lookup"><span data-stu-id="69f72-118">Name</span></span>          | <span data-ttu-id="69f72-119">説明</span><span class="sxs-lookup"><span data-stu-id="69f72-119">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="69f72-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f72-120">Authorization</span></span> | <span data-ttu-id="69f72-121">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="69f72-121">Bearer \{token\}.</span></span> <span data-ttu-id="69f72-122">必須です。</span><span class="sxs-lookup"><span data-stu-id="69f72-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="69f72-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="69f72-123">Request body</span></span>

<span data-ttu-id="69f72-124">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="69f72-124">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f72-125">応答</span><span class="sxs-lookup"><span data-stu-id="69f72-125">Response</span></span>

<span data-ttu-id="69f72-126">成功した場合、応答`204 No Content`はになります。</span><span class="sxs-lookup"><span data-stu-id="69f72-126">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="69f72-127">エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="69f72-127">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="69f72-128">例</span><span class="sxs-lookup"><span data-stu-id="69f72-128">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f72-129">要求</span><span class="sxs-lookup"><span data-stu-id="69f72-129">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="69f72-130">プロトコル</span><span class="sxs-lookup"><span data-stu-id="69f72-130">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "remove-from-bundle" } -->

```http
DELETE https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children/{item-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="69f72-131">C#</span><span class="sxs-lookup"><span data-stu-id="69f72-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/remove-from-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="69f72-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="69f72-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/remove-from-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="69f72-133">目的-C</span><span class="sxs-lookup"><span data-stu-id="69f72-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/remove-from-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="69f72-134">Java</span><span class="sxs-lookup"><span data-stu-id="69f72-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/remove-from-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="69f72-135">応答</span><span class="sxs-lookup"><span data-stu-id="69f72-135">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


[バンドル]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Remove an item from a bundle.",
  "keywords": "",
  "section": "documentation"
} -->