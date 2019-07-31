---
author: JeremyKelley
ms.author: jeremyke
title: バンドルを作成する
description: ドライブ項目のバンドルを作成する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 34befe2badb842ca996821266b00731cfdd559d5
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932864"
---
# <a name="create-bundle"></a><span data-ttu-id="65511-103">バンドルを作成する</span><span class="sxs-lookup"><span data-stu-id="65511-103">Create bundle</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65511-104">ユーザーのドライブに新しい[バンドル][]を追加します。</span><span class="sxs-lookup"><span data-stu-id="65511-104">Add a new [bundle][] to the user's drive.</span></span>

[バンドル]: ../resources/bundle.md
[bundle]: ../resources/bundle.md

## <a name="permissions"></a><span data-ttu-id="65511-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="65511-106">Permissions</span></span>

<span data-ttu-id="65511-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="65511-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65511-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="65511-109">Permission type</span></span>      | <span data-ttu-id="65511-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="65511-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65511-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="65511-111">Delegated (work or school account)</span></span> | <span data-ttu-id="65511-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65511-112">Not supported.</span></span>                             |
|<span data-ttu-id="65511-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="65511-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65511-114">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65511-114">Files.ReadWrite, Files.ReadWrite.All</span></span>   |
|<span data-ttu-id="65511-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="65511-115">Application</span></span>          | <span data-ttu-id="65511-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="65511-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="65511-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="65511-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drive/bundles
```

## <a name="request-headers"></a><span data-ttu-id="65511-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="65511-118">Request headers</span></span>

| <span data-ttu-id="65511-119">名前</span><span class="sxs-lookup"><span data-stu-id="65511-119">Name</span></span>          | <span data-ttu-id="65511-120">説明</span><span class="sxs-lookup"><span data-stu-id="65511-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="65511-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="65511-121">Authorization</span></span> | <span data-ttu-id="65511-122">ベアラー \{トークン\}。</span><span class="sxs-lookup"><span data-stu-id="65511-122">Bearer \{token\}.</span></span> <span data-ttu-id="65511-123">必須です。</span><span class="sxs-lookup"><span data-stu-id="65511-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65511-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="65511-124">Request body</span></span>

<span data-ttu-id="65511-125">要求本文で、作成するバンドルの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="65511-125">In the request body, supply a JSON representation of the bundle to be created.</span></span>

## <a name="response"></a><span data-ttu-id="65511-126">応答</span><span class="sxs-lookup"><span data-stu-id="65511-126">Response</span></span>

<span data-ttu-id="65511-127">要求が成功すると、新しく作成されたバンドルを表す[Drive 項目](../resources/driveitem.md)が返されます。</span><span class="sxs-lookup"><span data-stu-id="65511-127">If the request is successful, the [driveItem](../resources/driveitem.md) representing the newly created bundle will be returned.</span></span>

<span data-ttu-id="65511-128">エラーがどのように返されるかに関する詳細については、「[エラー応答][error-response]」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="65511-128">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="65511-129">例</span><span class="sxs-lookup"><span data-stu-id="65511-129">Examples</span></span>

### <a name="example-1-create-a-bundle"></a><span data-ttu-id="65511-130">例 1: バンドルを作成する</span><span class="sxs-lookup"><span data-stu-id="65511-130">Example 1: Create a bundle</span></span>

<span data-ttu-id="65511-131">次の例は、基本的な新しいバンドルを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="65511-131">The following example shows how to create a basic new bundle.</span></span>
<span data-ttu-id="65511-132">この要求は、という名前`Just some files`の新しいバンドルを作成し、既存の2つのアイテムをバンドルに追加します。</span><span class="sxs-lookup"><span data-stu-id="65511-132">This request will create a new bundle named `Just some files` and add two existing items to the bundle.</span></span>
<span data-ttu-id="65511-133">このバンドルを使用すると、そのアイテムが保存されているフォルダーを共有することなく、他のユーザーとファイルのコレクションを共有できます。</span><span class="sxs-lookup"><span data-stu-id="65511-133">This bundle can be used to share a collection of files with other users without sharing the folder those items are stored in.</span></span>

#### <a name="request"></a><span data-ttu-id="65511-134">要求</span><span class="sxs-lookup"><span data-stu-id="65511-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65511-135">プロトコル</span><span class="sxs-lookup"><span data-stu-id="65511-135">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-bundle" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "Just some files",
  "@name.conflictBehavior" : "rename",
  "bundle": { },
  "children": [
    { "id": "1234asdf" },
    { "id": "1234qwerty" }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65511-136">C#</span><span class="sxs-lookup"><span data-stu-id="65511-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-bundle-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65511-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="65511-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-bundle-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65511-138">目的-C</span><span class="sxs-lookup"><span data-stu-id="65511-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-bundle-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65511-139">Java</span><span class="sxs-lookup"><span data-stu-id="65511-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-bundle-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65511-140">応答</span><span class="sxs-lookup"><span data-stu-id="65511-140">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2
  }
}
```

<span data-ttu-id="65511-141">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="65511-141">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="65511-142">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65511-142">All the properties will be returned from an actual call.</span></span>

### <a name="example-2-create-an-album"></a><span data-ttu-id="65511-143">例 2: アルバムを作成する</span><span class="sxs-lookup"><span data-stu-id="65511-143">Example 2: Create an album</span></span>

<span data-ttu-id="65511-144">新しいフォトアルバムの作成要求は似ていますが、バンドルファセット内では、アルバムプロパティは null 以外の値に設定されています。</span><span class="sxs-lookup"><span data-stu-id="65511-144">The request to create a new photo album is similar, although inside the bundle facet, the album property is set to a non-null value.</span></span>

#### <a name="request"></a><span data-ttu-id="65511-145">要求</span><span class="sxs-lookup"><span data-stu-id="65511-145">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="65511-146">プロトコル</span><span class="sxs-lookup"><span data-stu-id="65511-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "create-album" } -->

```json
POST https://graph.microsoft.com/beta/drive/bundles
Content-Type: application/json

{
  "name": "My Day at the Beach",
  "@name.conflictBehavior" : "rename",
  "bundle": { "album": {} },
  "children": [
    { "id": "1234asdf" }
  ]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="65511-147">C#</span><span class="sxs-lookup"><span data-stu-id="65511-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-album-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="65511-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="65511-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-album-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="65511-149">目的-C</span><span class="sxs-lookup"><span data-stu-id="65511-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-album-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="65511-150">Java</span><span class="sxs-lookup"><span data-stu-id="65511-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-album-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65511-151">応答</span><span class="sxs-lookup"><span data-stu-id="65511-151">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "1234321!abc",
  "name": "Just some files",
  "bundle": {
    "childCount": 2,
    "album": { }
 }
}
```

<span data-ttu-id="65511-152">ここに示す response オブジェクトは読みやすいように短縮される場合があります。</span><span class="sxs-lookup"><span data-stu-id="65511-152">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="65511-153">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="65511-153">All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="65511-154">ConflictBehavior が**名前変更**に設定されていて、同じ名前のバンドルが既に存在する _@microsoft_場合は、新しいバンドル名が一意になるように更新されます。</span><span class="sxs-lookup"><span data-stu-id="65511-154">If _@microsoft.graph.conflictBehavior_ is set to **rename** and a bundle with the same name already exists, the new bundle name will be updated to be unique.</span></span>
<span data-ttu-id="65511-155">OneDrive では、バンドル名の末尾に番号が追加されます。</span><span class="sxs-lookup"><span data-stu-id="65511-155">OneDrive will append a number to the end of the bundle name.</span></span>

<span data-ttu-id="65511-156">たとえば、`My Day at the Beach` は `My Day at the Beach 1` に名前が変更されます。</span><span class="sxs-lookup"><span data-stu-id="65511-156">For example, `My Day at the Beach` would be renamed `My Day at the Beach 1`.</span></span>
<span data-ttu-id="65511-157">`My Day at the Beach 1`が実行されると、一意のバンドル名が検出されるまで番号が再びインクリメントされます。</span><span class="sxs-lookup"><span data-stu-id="65511-157">If `My Day at the Beach 1` is taken, then the number would be incremented again until a unique bundle name is discovered.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Create a new bundle or photo album.",
  "keywords": "create,bundle",
  "section": "documentation",
  "tocPath": "Bundles/Create"
} -->