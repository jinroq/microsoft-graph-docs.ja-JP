---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: FieldValueSet
ms.openlocfilehash: f1cc8d4d61d53b30c1da3e86f614895eb9d10833
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071283"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="3f18b-102">FieldValueSet リソース</span><span class="sxs-lookup"><span data-stu-id="3f18b-102">FieldValueSet resource</span></span>

> <span data-ttu-id="3f18b-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3f18b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3f18b-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3f18b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3f18b-105">[listItem](listitem.md) リソースでの列の値を表します。</span><span class="sxs-lookup"><span data-stu-id="3f18b-105">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f18b-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3f18b-106">JSON representation</span></span>

<span data-ttu-id="3f18b-107">以下は、**fieldValueSet** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3f18b-107">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
       "keyProperty": "id", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a><span data-ttu-id="3f18b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f18b-108">Properties</span></span>

<span data-ttu-id="3f18b-109">**listItem** の各ユーザーに表示されるフィールドは、**fieldValueSet** の名前と値のペアとして返されます。</span><span class="sxs-lookup"><span data-stu-id="3f18b-109">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="3f18b-110">上記の例は、**Author**、**Name**、**Color**、**Quantity** の 4 つの列を含むリストを示しています。</span><span class="sxs-lookup"><span data-stu-id="3f18b-110">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="3f18b-111">既定では、ルックアップ フィールド (上記の `Author` など) は返されません。</span><span class="sxs-lookup"><span data-stu-id="3f18b-111">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="3f18b-112">代わりにサーバーは、ルックアップの対象となる listItem を参照する 'LookupId' フィールド (上記の `AuthorLookupId` など) を返します。</span><span class="sxs-lookup"><span data-stu-id="3f18b-112">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="3f18b-113">'LookupId' フィールドの名前は元のフィールド名の末尾に `LookupId` を付けたものです。</span><span class="sxs-lookup"><span data-stu-id="3f18b-113">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="3f18b-114">1 つのクエリでは、ルックアップ フィールドを最大 12 個まで要求できます。</span><span class="sxs-lookup"><span data-stu-id="3f18b-114">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="3f18b-115">サーバーは、要求に `select` ステートメントと必要なフィールドが含まれていると、ルックアップ値を返します。</span><span class="sxs-lookup"><span data-stu-id="3f18b-115">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="3f18b-116">例:</span><span class="sxs-lookup"><span data-stu-id="3f18b-116">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="3f18b-117">1 つのクエリでは、最大 12 個のルックアップ フィールドと、任意の数の通常のフィールドを要求できます。</span><span class="sxs-lookup"><span data-stu-id="3f18b-117">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->