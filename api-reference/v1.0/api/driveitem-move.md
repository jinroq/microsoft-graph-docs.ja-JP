---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: ファイルまたはフォルダーを移動する
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 04ae380f69831f398699dcc3dcc50eb6921468e9
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33616365"
---
# <a name="move-a-driveitem-to-a-new-folder"></a><span data-ttu-id="1b997-102">DriveItem を新しいフォルダーに移動する</span><span class="sxs-lookup"><span data-stu-id="1b997-102">Move a DriveItem to a new folder</span></span>

<span data-ttu-id="1b997-103">DriveItem を新しい親アイテムに移動する場合は、移動する DriveItem の **parentReference** をアプリで更新します。</span><span class="sxs-lookup"><span data-stu-id="1b997-103">To move a DriveItem to a new parent item, your app requests to update the **parentReference** of the DriveItem to move.</span></span>

<span data-ttu-id="1b997-104">これは、[Update](driveitem-update.md) メソッドの特殊なケースです。</span><span class="sxs-lookup"><span data-stu-id="1b997-104">This is a special case of the [Update](driveitem-update.md) method.</span></span>
<span data-ttu-id="1b997-105">アプリでは、新しいコンテナーへのアイテムの移動と、アイテムの別のプロパティの更新を単一の要求に組み合わせることができます。</span><span class="sxs-lookup"><span data-stu-id="1b997-105">Your app can combine moving an item to a new container and updating other properties of the item into a single request.</span></span>

<span data-ttu-id="1b997-106">この要求を使用して、アイテムを[ドライブ](../resources/drive.md)間で移動することはできません。</span><span class="sxs-lookup"><span data-stu-id="1b997-106">Items cannot be moved between [Drives](../resources/drive.md) using this request.</span></span>

## <a name="permissions"></a><span data-ttu-id="1b997-107">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="1b997-107">Permissions</span></span>
<span data-ttu-id="1b997-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b997-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b997-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1b997-110">Permission type</span></span>      | <span data-ttu-id="1b997-111">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="1b997-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1b997-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1b997-112">Delegated (work or school account)</span></span> | <span data-ttu-id="1b997-113">Files.ReadWrite、Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b997-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b997-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1b997-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1b997-115">Files.ReadWrite、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b997-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="1b997-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1b997-116">Application</span></span> | <span data-ttu-id="1b997-117">Files.ReadWrite.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b997-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1b997-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1b997-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /drives/{drive-id}/items/{item-id}
PATCH /groups/{group-id}/drive/{item-id}
PATCH /me/drive/items/{item-id}
PATCH /sites/{site-id}/drive/items/{item-id}
PATCH /users/{user-id}/drive/items/{item-id}
```

## <a name="optional-request-headers"></a><span data-ttu-id="1b997-119">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b997-119">Optional request headers</span></span>

| <span data-ttu-id="1b997-120">名前</span><span class="sxs-lookup"><span data-stu-id="1b997-120">Name</span></span>          | <span data-ttu-id="1b997-121">型</span><span class="sxs-lookup"><span data-stu-id="1b997-121">Type</span></span>   | <span data-ttu-id="1b997-122">説明</span><span class="sxs-lookup"><span data-stu-id="1b997-122">Description</span></span>                                                                                                                                                         |
|:--------------|:-------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="1b997-123">if-match</span><span class="sxs-lookup"><span data-stu-id="1b997-123">if-match</span></span>      | <span data-ttu-id="1b997-124">String</span><span class="sxs-lookup"><span data-stu-id="1b997-124">String</span></span> | <span data-ttu-id="1b997-125">この要求ヘッダーが含まれていて、指定された eTag (または cTag) がフォルダーの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返されます。</span><span class="sxs-lookup"><span data-stu-id="1b997-125">If this request header is included and the eTag (or cTag) provided does not match the current eTag on the folder, a `412 Precondition Failed` response is returned.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1b997-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1b997-126">Request body</span></span>

<span data-ttu-id="1b997-p103">要求の本文内に、**parentReference** プロパティの新しい値を指定します。要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="1b997-p103">In the request body, supply the new value for the **parentReference** property. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

<span data-ttu-id="1b997-130">**注:** ドライブのルートにアイテムを移動するときは、`"id:" "root"` 構文はアプリでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="1b997-130">**Note:** When moving items to the root of a drive your app cannot use the `"id:" "root"` syntax.</span></span>
<span data-ttu-id="1b997-131">アプリは、親参照のためにルート フォルダーの実際の ID を提供する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b997-131">Your app needs to provide the actual ID of the root folder for the parent reference.</span></span>

## <a name="response"></a><span data-ttu-id="1b997-132">応答</span><span class="sxs-lookup"><span data-stu-id="1b997-132">Response</span></span>

<span data-ttu-id="1b997-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [DriveItem](../resources/driveitem.md) リソースを返します。</span><span class="sxs-lookup"><span data-stu-id="1b997-133">If successful, this method returns a `200 OK` response code and updated [DriveItem](../resources/driveitem.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b997-134">例</span><span class="sxs-lookup"><span data-stu-id="1b997-134">Example</span></span>

<span data-ttu-id="1b997-135">この例では、{item-id} で指定したアイテムを、ID を持つユーザーのドライブの `new-parent-folder-id` フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="1b997-135">This example moves an item specified by {item-id} into a folder in the user's drive with the ID `new-parent-folder-id`.</span></span>

<!-- { "blockType": "request", "name": "move-item", "scopes": "files.readwrite", "tags": "service.graph" } -->

```http
PATCH /me/drive/items/{item-id}
Content-type: application/json

{
  "parentReference": {
    "id": "{new-parent-folder-id}"
  },
  "name": "new-item-name.txt"
}
```

### <a name="response"></a><span data-ttu-id="1b997-136">応答</span><span class="sxs-lookup"><span data-stu-id="1b997-136">Response</span></span>

<span data-ttu-id="1b997-137">次の例は、この移動要求への応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="1b997-137">The following example shows the response for this move request.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="1b997-138">SDK サンプルコード</span><span class="sxs-lookup"><span data-stu-id="1b997-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="1b997-139">Visual</span><span class="sxs-lookup"><span data-stu-id="1b997-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/move-item-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="1b997-140">Java</span><span class="sxs-lookup"><span data-stu-id="1b997-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/move-item-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="error-responses"></a><span data-ttu-id="1b997-141">エラー応答</span><span class="sxs-lookup"><span data-stu-id="1b997-141">Error responses</span></span>

<span data-ttu-id="1b997-142">エラーがどのように返されるかについては、「[エラー応答][error-response]」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b997-142">See [Error Responses][error-response] for more info about how errors are returned.</span></span>

[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Move an item to another location or rename the item.",
  "keywords": "move,rename,mv,change location",
  "section": "documentation",
  "tocPath": "Items/Move",
  "suppressions": [
    "Error: /api-reference/v1.0/api/driveitem-move.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/driveitem-move.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
} -->
