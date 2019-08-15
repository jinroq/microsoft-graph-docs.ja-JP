---
author: JeremyKelley
ms.author: jeremyke
title: バンドルを更新する
description: ドライブ項目のバンドルを更新する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: a68aedbec838b0c74c1750acdee73a0f20880933
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36419198"
---
# <a name="update-bundle"></a><span data-ttu-id="16492-103">バンドルの更新</span><span class="sxs-lookup"><span data-stu-id="16492-103">Update bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="16492-104">ID を使用して、[ドライブ項目]の[ドライブ項目]の[バンドル][]のメタデータを更新します。</span><span class="sxs-lookup"><span data-stu-id="16492-104">Update the metadata for a [bundle][] of [driveItems][driveItem] by ID.</span></span>
<span data-ttu-id="16492-105">次のメタデータのみを更新できます。</span><span class="sxs-lookup"><span data-stu-id="16492-105">You can only update the following metadata:</span></span>

* <span data-ttu-id="16492-106">バンドル名</span><span class="sxs-lookup"><span data-stu-id="16492-106">Bundle name</span></span>
* <span data-ttu-id="16492-107">アルバム`coverImageItemId` (該当する場合)</span><span class="sxs-lookup"><span data-stu-id="16492-107">Album `coverImageItemId` (if applicable)</span></span>

<span data-ttu-id="16492-108">その他の変更要求は無視されます。</span><span class="sxs-lookup"><span data-stu-id="16492-108">Any other change requests will be ignored.</span></span>

## <a name="permissions"></a><span data-ttu-id="16492-109">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="16492-109">Permissions</span></span>

<span data-ttu-id="16492-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16492-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16492-112">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16492-112">Permission type</span></span>      | <span data-ttu-id="16492-113">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="16492-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="16492-114">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16492-114">Delegated (work or school account)</span></span> | <span data-ttu-id="16492-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16492-115">Not supported.</span></span>                             |
|<span data-ttu-id="16492-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16492-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="16492-117">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16492-117">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="16492-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16492-118">Application</span></span>          | <span data-ttu-id="16492-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16492-119">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="16492-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16492-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drive/items/{bundle-id}
```

## <a name="request-headers"></a><span data-ttu-id="16492-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16492-121">Request headers</span></span>

| <span data-ttu-id="16492-122">名前</span><span class="sxs-lookup"><span data-stu-id="16492-122">Name</span></span>          | <span data-ttu-id="16492-123">説明</span><span class="sxs-lookup"><span data-stu-id="16492-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="16492-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="16492-124">Authorization</span></span> | <span data-ttu-id="16492-125">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="16492-125">Bearer \{token\}.</span></span> <span data-ttu-id="16492-126">必須。</span><span class="sxs-lookup"><span data-stu-id="16492-126">Required.</span></span> |
| <span data-ttu-id="16492-127">if-match</span><span class="sxs-lookup"><span data-stu-id="16492-127">if-match</span></span>      | <span data-ttu-id="16492-128">eTag.</span><span class="sxs-lookup"><span data-stu-id="16492-128">eTag.</span></span> <span data-ttu-id="16492-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="16492-129">Optional.</span></span> <span data-ttu-id="16492-130">この要求ヘッダーが含まれており、指定された eTag が buncle の現在の eTag と`412 Precondition Failed`一致しない場合は、応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="16492-130">If this request header is included and the eTag provided does not match the current eTag on the buncle, a `412 Precondition Failed` response is returned.</span></span>

## <a name="request-body"></a><span data-ttu-id="16492-131">要求本文</span><span class="sxs-lookup"><span data-stu-id="16492-131">Request body</span></span>

<span data-ttu-id="16492-132">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="16492-132">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="16492-133">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="16492-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="16492-134">最適なパフォーマンスを得るために、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="16492-134">For best performance, don't include existing values that haven't changed.</span></span>

## <a name="response"></a><span data-ttu-id="16492-135">応答</span><span class="sxs-lookup"><span data-stu-id="16492-135">Response</span></span>

<span data-ttu-id="16492-136">成功した場合、このメソッドは、応答本文で更新されたバンドルを表す、[ドライブ項目][]リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="16492-136">If successful, this method returns a [driveItem][] resource that represents the updated bundle in the response body.</span></span>

<span data-ttu-id="16492-137">エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="16492-137">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="example"></a><span data-ttu-id="16492-138">例</span><span class="sxs-lookup"><span data-stu-id="16492-138">Example</span></span>

<span data-ttu-id="16492-139">この例では、バンドルの名前を変更します。</span><span class="sxs-lookup"><span data-stu-id="16492-139">This example renames a bundle.</span></span>

### <a name="request"></a><span data-ttu-id="16492-140">要求</span><span class="sxs-lookup"><span data-stu-id="16492-140">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="16492-141">プロトコル</span><span class="sxs-lookup"><span data-stu-id="16492-141">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "rename-bundle" } -->

```json
PATCH https://graph.microsoft.com/beta/drive/items/{bundle-id}
Content-Type: application/json

{
  "name": "Shared legal agreements"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="16492-142">C#</span><span class="sxs-lookup"><span data-stu-id="16492-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/rename-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="16492-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="16492-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/rename-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="16492-144">目的-C</span><span class="sxs-lookup"><span data-stu-id="16492-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/rename-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="16492-145">応答</span><span class="sxs-lookup"><span data-stu-id="16492-145">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "0123456789abc",
  "name": "Shared legal agreements",
  "bundle": {
    "childCount": 3
  }
}
```

<span data-ttu-id="16492-146">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="16492-146">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="16492-147">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="16492-147">All the properties will be returned from an actual call.</span></span>


[バンドル]: ../resources/bundle.md
[bundle]: ../resources/bundle.md
[driveItem]: ../resources/driveItem.md
[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Update or replace the contents or properties of a bundle.",
  "keywords": "update,replace,contents,bundle",
  "section": "documentation",
    "tocPath": "Bundles/Update"
} -->
