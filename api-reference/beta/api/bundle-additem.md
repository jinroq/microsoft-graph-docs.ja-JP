---
author: JeremyKelley
ms.author: jeremyke
title: バンドルにアイテムを追加する
description: ドライブ項目のバンドルにアイテムを追加する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 63c7dafb5f3787148b8c5775a83e2a381b64947a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36318020"
---
# <a name="add-item-to-a-bundle"></a><span data-ttu-id="2ebb3-103">バンドルにアイテムを追加する</span><span class="sxs-lookup"><span data-stu-id="2ebb3-103">Add item to a bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ebb3-104">ドライブから[バンドル][]に、追加のドライブ[項目][]を追加します。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-104">Add an additional [driveItem][] from a drive to a [bundle][].</span></span>

[バンドル]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md

## <a name="permissions"></a><span data-ttu-id="2ebb3-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="2ebb3-107">Permissions</span></span>

<span data-ttu-id="2ebb3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ebb3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2ebb3-110">Permission type</span></span>      | <span data-ttu-id="2ebb3-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="2ebb3-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2ebb3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2ebb3-112">Delegated (work or school account)</span></span> | <span data-ttu-id="2ebb3-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-113">Not supported.</span></span>                             |
|<span data-ttu-id="2ebb3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2ebb3-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ebb3-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ebb3-115">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="2ebb3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2ebb3-116">Application</span></span>          | <span data-ttu-id="2ebb3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-117">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="2ebb3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2ebb3-118">HTTP request</span></span>

```http
POST /drive/bundles/{bundle-id}/children
```

## <a name="request-headers"></a><span data-ttu-id="2ebb3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2ebb3-119">Request headers</span></span>

| <span data-ttu-id="2ebb3-120">名前</span><span class="sxs-lookup"><span data-stu-id="2ebb3-120">Name</span></span>          | <span data-ttu-id="2ebb3-121">説明</span><span class="sxs-lookup"><span data-stu-id="2ebb3-121">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="2ebb3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ebb3-122">Authorization</span></span> | <span data-ttu-id="2ebb3-123">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-123">Bearer \{token\}.</span></span> <span data-ttu-id="2ebb3-124">必須です。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-124">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ebb3-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2ebb3-125">Request body</span></span>

<span data-ttu-id="2ebb3-126">要求本文には、バンドルの子コレクションに追加する必要があるアイテムの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-126">The request body includes the identifier for an item that should be added to the bundle's children collection.</span></span>

## <a name="response"></a><span data-ttu-id="2ebb3-127">応答</span><span class="sxs-lookup"><span data-stu-id="2ebb3-127">Response</span></span>

<span data-ttu-id="2ebb3-128">成功した場合、応答`204 No Content`はになります。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-128">If successful, the response is `204 No Content`.</span></span>

<span data-ttu-id="2ebb3-129">エラーがどのような形で返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-129">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="2ebb3-130">例</span><span class="sxs-lookup"><span data-stu-id="2ebb3-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ebb3-131">要求</span><span class="sxs-lookup"><span data-stu-id="2ebb3-131">Request</span></span>

<span data-ttu-id="2ebb3-132">この要求は、指定したバンドルに既存のアイテムを追加します。</span><span class="sxs-lookup"><span data-stu-id="2ebb3-132">This request will add an existing item to the specified bundle.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2ebb3-133">プロトコル</span><span class="sxs-lookup"><span data-stu-id="2ebb3-133">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "add-to-bundle", "isCollection": true, "@odata.type": "microsoft.graph.driveItem", "tags": "onedrive.only" } -->

```http
POST https://graph.microsoft.com/beta/drive/bundles/{bundle-id}/children
Content-Type: application/json

{
  "id": "123456!87"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2ebb3-134">C#</span><span class="sxs-lookup"><span data-stu-id="2ebb3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/add-to-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2ebb3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ebb3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/add-to-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2ebb3-136">目的-C</span><span class="sxs-lookup"><span data-stu-id="2ebb3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/add-to-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2ebb3-137">Java</span><span class="sxs-lookup"><span data-stu-id="2ebb3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/add-to-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ebb3-138">応答</span><span class="sxs-lookup"><span data-stu-id="2ebb3-138">Response</span></span>

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add items to an existing bundle.",
  "keywords": "",
  "section": "documentation"
} -->
