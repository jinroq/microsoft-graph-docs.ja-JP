---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リスト内のレコードを更新する
ms.openlocfilehash: fdd43cebf83e802441552be5476659677e41e8e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021296"
---
# <a name="update-an-item-in-a-list"></a><span data-ttu-id="e5e55-102">リスト内のアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="e5e55-102">Update an item in a list</span></span>

<span data-ttu-id="e5e55-103">**[listItem][]** のプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e5e55-103">Update the properties on a **[listItem][]**.</span></span>

## <a name="permissions"></a><span data-ttu-id="e5e55-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="e5e55-104">Permissions</span></span>

<span data-ttu-id="e5e55-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e5e55-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5e55-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e5e55-107">Permission type</span></span>      | <span data-ttu-id="e5e55-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="e5e55-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e5e55-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e5e55-109">Delegated (work or school account)</span></span> | <span data-ttu-id="e5e55-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5e55-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e5e55-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e5e55-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e5e55-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5e55-112">Not supported.</span></span>    |
|<span data-ttu-id="e5e55-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e5e55-113">Application</span></span> | <span data-ttu-id="e5e55-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5e55-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e5e55-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e5e55-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
```

## <a name="optional-request-headers"></a><span data-ttu-id="e5e55-116">オプションの要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e5e55-116">Optional request headers</span></span>

| <span data-ttu-id="e5e55-117">名前</span><span class="sxs-lookup"><span data-stu-id="e5e55-117">Name</span></span>       | <span data-ttu-id="e5e55-118">値</span><span class="sxs-lookup"><span data-stu-id="e5e55-118">Value</span></span> | <span data-ttu-id="e5e55-119">説明</span><span class="sxs-lookup"><span data-stu-id="e5e55-119">Description</span></span>
|:-----------|:------|:--------------------------------------------------------
| <span data-ttu-id="e5e55-120">_if-match_</span><span class="sxs-lookup"><span data-stu-id="e5e55-120">_if-match_</span></span> | <span data-ttu-id="e5e55-121">etag</span><span class="sxs-lookup"><span data-stu-id="e5e55-121">etag</span></span>  | <span data-ttu-id="e5e55-122">この要求ヘッダーが含まれていて、指定された eTag がアイテムの現在の eTag に一致しない場合には、`412 Precondition Failed` 応答が返され、アイテムは更新されません。</span><span class="sxs-lookup"><span data-stu-id="e5e55-122">If this request header is included and the eTag provided does not match the current eTag on the item, a `412 Precondition Failed` response is returned and the item will not be updated.</span></span>


## <a name="request-body"></a><span data-ttu-id="e5e55-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e5e55-123">Request body</span></span>

<span data-ttu-id="e5e55-124">要求本文に、更新するフィールドを指定する [fieldValueSet][] の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e5e55-124">In the request body, supply a JSON representation of a [fieldValueSet][] specifying the fields to update.</span></span>

## <a name="example"></a><span data-ttu-id="e5e55-125">例</span><span class="sxs-lookup"><span data-stu-id="e5e55-125">Example</span></span>

<span data-ttu-id="e5e55-126">ここでは、リスト アイテムの Color フィールドと Quantity フィールドを新しい値で更新する例を示します。</span><span class="sxs-lookup"><span data-stu-id="e5e55-126">Here is an example that updates the Color and Quantity fields of the list item with new values.</span></span>
<span data-ttu-id="e5e55-127">listItem の他の値はすべてそのままです。</span><span class="sxs-lookup"><span data-stu-id="e5e55-127">All other values on the listItem are left alone.</span></span> 

<!-- { "blockType": "request", "name": "update-listitem", "scopes": "sites.readwrite.all" } -->

```json
PATCH https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items/{item-id}/fields
Content-Type: application/json

{
    "Color": "Fuchsia",
    "Quantity": 934
}
```

## <a name="response"></a><span data-ttu-id="e5e55-128">応答</span><span class="sxs-lookup"><span data-stu-id="e5e55-128">Response</span></span>

<span data-ttu-id="e5e55-129">成功した場合、このメソッドは更新されたリスト アイテムの応答本文で [fieldValueSet][] を返します。</span><span class="sxs-lookup"><span data-stu-id="e5e55-129">If successful, this method returns a [fieldValueSet][] in the response body for the updated list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.fieldValueSet", "truncated": true } -->

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