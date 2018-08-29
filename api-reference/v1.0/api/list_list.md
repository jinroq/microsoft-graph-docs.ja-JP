---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: サイト内の SharePoint リストを一覧表示する
ms.openlocfilehash: 5d88720ecf3d183f806526364130dd2812874f3c
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23267648"
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="200be-102">サイト内のリストを列挙する</span><span class="sxs-lookup"><span data-stu-id="200be-102">Enumerate lists in a site</span></span>

<span data-ttu-id="200be-103">[サイト][]の[リスト][]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="200be-103">Get the collection of [lists][] for a [site][].</span></span>

[サイト]: ../resources/list.md
[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="200be-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="200be-106">Permissions</span></span>

<span data-ttu-id="200be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="200be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="200be-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="200be-109">Permission type</span></span>      | <span data-ttu-id="200be-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="200be-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="200be-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="200be-111">Delegated (work or school account)</span></span> | <span data-ttu-id="200be-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="200be-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="200be-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="200be-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="200be-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="200be-114">Not supported.</span></span>    |
|<span data-ttu-id="200be-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="200be-115">Application</span></span> | <span data-ttu-id="200be-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="200be-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="200be-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="200be-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="200be-118">例</span><span class="sxs-lookup"><span data-stu-id="200be-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="200be-119">要求</span><span class="sxs-lookup"><span data-stu-id="200be-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all", "tags": "service.sharepoint" } -->

```http
GET https://graph.microsoft.com/v1.0/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="200be-120">応答</span><span class="sxs-lookup"><span data-stu-id="200be-120">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.list", "isCollection": true, "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b57af081-936c-4803-a120-d94887b03864",
      "name": "Documents",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "documentLibrary"
       }
    },
    {
      "id": "1234-112-112-4",
      "name": "MicroFeed",
      "createdDateTime": "2016-08-30T08:32:00Z",
      "lastModifiedDateTime": "2016-08-30T08:32:00Z",
      "list": {
        "hidden": false,
        "template": "genericList"
       }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="200be-121">注釈</span><span class="sxs-lookup"><span data-stu-id="200be-121">Remarks</span></span>

<span data-ttu-id="200be-122">[system][] ファセットのあるリストは既定では非表示です。</span><span class="sxs-lookup"><span data-stu-id="200be-122">Lists with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="200be-123">それらを一覧表示するには、`$select` ステートメントに `system` を含めます。</span><span class="sxs-lookup"><span data-stu-id="200be-123">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemFacet.md

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
