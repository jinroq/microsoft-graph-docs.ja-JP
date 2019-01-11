---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: SharePoint リストに新しいエントリを作成する
localization_priority: Priority
ms.openlocfilehash: 9456a8d7a8cb7561487a5a6bf08e5fd08082cf05
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876413"
---
# <a name="create-a-new-item-in-a-list"></a><span data-ttu-id="49a68-102">リストに新しいアイテムを作成する</span><span class="sxs-lookup"><span data-stu-id="49a68-102">Create a new item in a list</span></span>

<span data-ttu-id="49a68-103">[list][] に新しい [listItem][] を作成します。</span><span class="sxs-lookup"><span data-stu-id="49a68-103">Create a new [listItem][] in a [list][].</span></span>

## <a name="permissions"></a><span data-ttu-id="49a68-104">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="49a68-104">Permissions</span></span>

<span data-ttu-id="49a68-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49a68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49a68-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="49a68-107">Permission type</span></span>      | <span data-ttu-id="49a68-108">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="49a68-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49a68-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="49a68-109">Delegated (work or school account)</span></span> | <span data-ttu-id="49a68-110">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49a68-110">Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="49a68-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="49a68-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49a68-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="49a68-112">Not supported.</span></span>    |
|<span data-ttu-id="49a68-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="49a68-113">Application</span></span> | <span data-ttu-id="49a68-114">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="49a68-114">Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49a68-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="49a68-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
```

## <a name="request-body"></a><span data-ttu-id="49a68-116">要求本文</span><span class="sxs-lookup"><span data-stu-id="49a68-116">Request body</span></span>

<span data-ttu-id="49a68-117">要求本文で、作成する [listItem][] リソースの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="49a68-117">In the request body, supply a JSON representation of the [listItem][] resource to create.</span></span>

## <a name="example"></a><span data-ttu-id="49a68-118">例</span><span class="sxs-lookup"><span data-stu-id="49a68-118">Example</span></span>

<span data-ttu-id="49a68-119">新しい汎用リスト アイテムを作成する方法の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="49a68-119">Here is an example of how to create a new generic list item.</span></span>

<!-- { "blockType": "request", "name": "create-listitem", "scopes": "sites.readwrite.all" } -->

```json
POST https://graph.microsoft.com/v1.0/sites/{site-id}/lists/{list-id}/items
Content-Type: application/json

{
  "fields": {
    "Title": "Widget",
    "Color": "Purple",
    "Weight": 32
  }
}
```

## <a name="response"></a><span data-ttu-id="49a68-120">応答</span><span class="sxs-lookup"><span data-stu-id="49a68-120">Response</span></span>

<span data-ttu-id="49a68-121">成功した場合、このメソッドは作成されたリスト アイテムの応答本文で [listItem][] を返します。</span><span class="sxs-lookup"><span data-stu-id="49a68-121">If successful, this method returns a [listItem][] in the response body for the created list item.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.listItem", "truncated": true } -->

```json
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "20",
  "createdDateTime": "2016-08-30T08:26:00Z",
  "createdBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  },
  "lastModifiedDateTime": "2016-08-30T08:26:00Z",
  "lastModifiedBy": {
    "user": {
      "displayName": "Ryan Gregg",
      "id": "8606e4d5-d582-4f5f-aeba-7d7c18b20cfd"
    }
  }
}
```

<span data-ttu-id="49a68-122">**注:** 応答オブジェクトは、わかりやすくするために切り詰められています。</span><span class="sxs-lookup"><span data-stu-id="49a68-122">**Note:** The response object is truncated for clarity.</span></span> <span data-ttu-id="49a68-123">実際の呼び出しでは、既定のプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="49a68-123">Default properties will be returned from the actual call.</span></span>

[list]: ../resources/list.md
[listItem]: ../resources/listitem.md

<!-- {
  "type": "#page.annotation",
  "description": "Add a new item to a SharePoint list.",
  "keywords": "",
  "section": "documentation",
  "tocPath": "ListItem/Create"
} -->
