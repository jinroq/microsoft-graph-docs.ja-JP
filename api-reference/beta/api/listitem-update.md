---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リスト内のレコードを更新する
ms.openlocfilehash: a3d5ca140f56da1de5f4134fbe76f55b350e83a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066755"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="02a8d-102">リスト内のアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="02a8d-102">Update an item in a list</span></span>

> <span data-ttu-id="02a8d-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02a8d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02a8d-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02a8d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02a8d-105">**[listItem][]** のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="02a8d-105">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="02a8d-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="02a8d-106">Permissions</span></span>

<span data-ttu-id="02a8d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02a8d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02a8d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02a8d-109">Permission type</span></span>      | <span data-ttu-id="02a8d-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="02a8d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02a8d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02a8d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="02a8d-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a8d-112">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="02a8d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02a8d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02a8d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02a8d-114">Not supported.</span></span>    |
|<span data-ttu-id="02a8d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02a8d-115">Application</span></span> | <span data-ttu-id="02a8d-116">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02a8d-116">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="02a8d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02a8d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="02a8d-118">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02a8d-118">Optional request headers</span></span>

| <span data-ttu-id="02a8d-119">名前</span><span class="sxs-lookup"><span data-stu-id="02a8d-119">Name</span></span>       | <span data-ttu-id="02a8d-120">値</span><span class="sxs-lookup"><span data-stu-id="02a8d-120">Value</span></span> | <span data-ttu-id="02a8d-121">説明</span><span class="sxs-lookup"><span data-stu-id="02a8d-121">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="02a8d-122">_if-match_</span><span class="sxs-lookup"><span data-stu-id="02a8d-122">_if-match_</span></span> | <span data-ttu-id="02a8d-123">etag</span><span class="sxs-lookup"><span data-stu-id="02a8d-123">etag</span></span>  | <span data-ttu-id="02a8d-124">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは更新されません。</span><span class="sxs-lookup"><span data-stu-id="02a8d-124">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="02a8d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="02a8d-125">Request body</span></span>

<span data-ttu-id="02a8d-126">要求本文に、更新するフィールドを指定する [fieldValueSet][] の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="02a8d-126">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="02a8d-127">例</span><span class="sxs-lookup"><span data-stu-id="02a8d-127">Example</span></span>

<span data-ttu-id="02a8d-128">ここでは、リスト アイテムの Color フィールドと Quantity フィールドを新しい値で更新する例を示します。</span><span class="sxs-lookup"><span data-stu-id="02a8d-128">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="02a8d-129">listItem の他の値はすべてそのままです。</span><span class="sxs-lookup"><span data-stu-id="02a8d-129">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="02a8d-130">応答</span><span class="sxs-lookup"><span data-stu-id="02a8d-130">Response</span></span>

<span data-ttu-id="02a8d-131">成功した場合、このメソッドは更新されたリスト アイテムの応答本文で [fieldValueSet][] を返します。</span><span class="sxs-lookup"><span data-stu-id="02a8d-131">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "Name": "Widget",
  "Color": "Fuchsia",
  "Quantity": 934
}
```

[fieldValueSet]: ../resources/fieldvalueset.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Update"
} -->
