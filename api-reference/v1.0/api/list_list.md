---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: "サイト内の SharePoint リストを一覧表示する"
ms.openlocfilehash: 4be4c4aefc29cdcd684bc11ad086b5c0572dbe2b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="enumerate-lists-in-a-site"></a><span data-ttu-id="5f5c2-102">サイト内のリストを列挙する</span><span class="sxs-lookup"><span data-stu-id="5f5c2-102">Enumerate lists in a site</span></span>

<span data-ttu-id="5f5c2-103">[サイト][]の[リスト][]のコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="5f5c2-103">Get the collection of [lists][] for a [site][].</span></span>

[lists]: ../resources/list.md
[site]: ../resources/site.md

## <a name="permissions"></a><span data-ttu-id="5f5c2-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="5f5c2-106">Permissions</span></span>

<span data-ttu-id="5f5c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f5c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5f5c2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f5c2-109">Permission type</span></span>      | <span data-ttu-id="5f5c2-110">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f5c2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5f5c2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f5c2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5f5c2-112">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f5c2-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="5f5c2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f5c2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5f5c2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f5c2-114">Not supported.</span></span>    |
|<span data-ttu-id="5f5c2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f5c2-115">Application</span></span> | <span data-ttu-id="5f5c2-116">Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f5c2-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5f5c2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f5c2-117">HTTP request</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

## <a name="example"></a><span data-ttu-id="5f5c2-118">例</span><span class="sxs-lookup"><span data-stu-id="5f5c2-118">Example</span></span>

#### <a name="request"></a><span data-ttu-id="5f5c2-119">要求</span><span class="sxs-lookup"><span data-stu-id="5f5c2-119">Request</span></span>

<!-- { "blockType": "request", "name": "enum-lists", "scopes": "sites.read.all service.sharepoint" } -->

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists
```

##### <a name="response"></a><span data-ttu-id="5f5c2-120">応答</span><span class="sxs-lookup"><span data-stu-id="5f5c2-120">Response</span></span>

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

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Lists/Enumerate"
} -->
