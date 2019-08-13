---
author: JeremyKelley
description: DriveItem を新しい親アイテムに移動する場合は、移動する DriveItem の parentReference をアプリで更新します。
ms.date: 09/10/2017
title: ファイルまたはフォルダーを移動する
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 163f53ada04154647fd886124644e48fbccec821
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36324329"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="fa129-103">DriveItem を新しいフォルダーに移動する</span><span class="sxs-lookup"><span data-stu-id="fa129-103">Move a DriveItem to a new folder</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa129-104">DriveItem を新しい親アイテムに移動する場合は、移動する DriveItem の **parentReference** をアプリで更新します。</span><span class="sxs-lookup"><span data-stu-id="fa129-104">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="fa129-105">これは、[Update](driveitem-update.md) メソッドの特殊なケースです。</span><span class="sxs-lookup"><span data-stu-id="fa129-105">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="fa129-106">アプリでは、新しいコンテナーへのアイテムの移動と、アイテムの別のプロパティの更新を単一の要求に組み合わせることができます。</span><span class="sxs-lookup"><span data-stu-id="fa129-106">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="fa129-107">この要求を使用して、アイテムを[ドライブ](../resources/drive.md)間で移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="fa129-107">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa129-108">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="fa129-108">Permissions</span></span>
<span data-ttu-id="fa129-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa129-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa129-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa129-111">Permission type</span></span>      | <span data-ttu-id="fa129-112">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa129-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa129-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa129-113">Delegated (work or school account)</span></span> | <span data-ttu-id="fa129-114">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa129-114">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa129-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa129-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa129-116">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa129-116">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fa129-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa129-117">Application</span></span> | <span data-ttu-id="fa129-118">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa129-118">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa129-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa129-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="fa129-120">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa129-120">Optional request headers</span></span>

| <span data-ttu-id="fa129-121">名前</span><span class="sxs-lookup"><span data-stu-id="fa129-121">Name</span></span>          | <span data-ttu-id="fa129-122">型</span><span class="sxs-lookup"><span data-stu-id="fa129-122">Type</span></span>   | <span data-ttu-id="fa129-123">説明</span><span class="sxs-lookup"><span data-stu-id="fa129-123">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="fa129-124">if-match</span><span class="sxs-lookup"><span data-stu-id="fa129-124">if-match</span></span>      | <span data-ttu-id="fa129-125">String</span><span class="sxs-lookup"><span data-stu-id="fa129-125">String</span></span> | <span data-ttu-id="fa129-126">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="fa129-126">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa129-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa129-127">Request body</span></span>

<span data-ttu-id="fa129-p103">要求の本文内に、**parentReference** プロパティの新しい値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="fa129-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="fa129-131">**注:** ドライブのルートにアイテムを移動するときは、`"id:" "root"` 構文はアプリでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="fa129-131">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="fa129-132">アプリは、親参照のためにルート フォルダーの実際の ID を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa129-132">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="fa129-133">応答</span><span class="sxs-lookup"><span data-stu-id="fa129-133">Response</span></span>

<span data-ttu-id="fa129-134">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="fa129-134">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa129-135">例</span><span class="sxs-lookup"><span data-stu-id="fa129-135">Example</span></span>

<span data-ttu-id="fa129-136">この例では、{item-id} で指定したアイテムを、ID を持つユーザーのドライブの `new-parent-folder-id` フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="fa129-136">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="fa129-137">プロトコル</span><span class="sxs-lookup"><span data-stu-id="fa129-137">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "move-item", "scopes": "files.readwrite" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "parentReference": {
    "id": "new-parent-folder-id"
  },
  "name": "new-item-name.txt"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fa129-138">C#</span><span class="sxs-lookup"><span data-stu-id="fa129-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/move-item-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fa129-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fa129-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/move-item-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fa129-140">目的-C</span><span class="sxs-lookup"><span data-stu-id="fa129-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/move-item-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="fa129-141">Java</span><span class="sxs-lookup"><span data-stu-id="fa129-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/move-item-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fa129-142">応答</span><span class="sxs-lookup"><span data-stu-id="fa129-142">Response</span></span>

<span data-ttu-id="fa129-143">次の例は、この移動要求への応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="fa129-143">The following example shows the response for this move request.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "0123456789abc",
  "name": "new-item-name.txt",
  "parentReference":
  {
    "driveId": "11231001",
    "path": "/drive/root:/Documents",
    "id": "1231203102!1011"
  }
}
```

## <a name="error-responses"></a><span data-ttu-id="fa129-144">エラー応答</span><span class="sxs-lookup"><span data-stu-id="fa129-144">Error responses</span></span>

<span data-ttu-id="fa129-145">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa129-145">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!--
{
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move",
  "suppressions": [
  ]
}
-->
