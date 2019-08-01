---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: FieldValueSet
localization_priority: Normal
description: listItem リソースでの列の値を表します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a1a308bfcda1bf913455ca6689dbaca308daecbb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032523"
---
# <a name="fieldvalueset-resource"></a><span data-ttu-id="bf417-103">FieldValueSet リソース</span><span class="sxs-lookup"><span data-stu-id="bf417-103">FieldValueSet resource</span></span>

<span data-ttu-id="bf417-104">[listItem](listitem.md) リソースでの列の値を表します。</span><span class="sxs-lookup"><span data-stu-id="bf417-104">Represents the column values in a [listItem](listitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf417-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bf417-105">JSON representation</span></span>

<span data-ttu-id="bf417-106">以下は、**fieldValueSet** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bf417-106">Here is a JSON representation of a **fieldValueSet** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.fieldValueSet",
      "optionalProperties": ["Author", "AuthorLookupId", "Name", "Color", "Quantity" ],
       "baseType": "microsoft.graph.entity", "openType": true } -->

```json
{
    "Author": "Brad Cleaver",
    "AuthorLookupId": "13",
    "Name": "Kangaroos and Wallabies: A Deep Dive",
    "Color": "Red",
    "Quantity": 350,
}
```

## <a name="properties"></a><span data-ttu-id="bf417-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bf417-107">Properties</span></span>

<span data-ttu-id="bf417-108">**listItem** の各ユーザーに表示されるフィールドは、**fieldValueSet** の名前と値のペアとして返されます。</span><span class="sxs-lookup"><span data-stu-id="bf417-108">Each user-visible field in the **listItem** is returned as a name-value pair in the **fieldValueSet**.</span></span>
<span data-ttu-id="bf417-109">上記の例は、**Author**、**Name**、**Color**、**Quantity** の 4 つの列を含むリストを示しています。</span><span class="sxs-lookup"><span data-stu-id="bf417-109">The example above is for a list that contains four columns, **Author**, **Name**, **Color**, and **Quantity**.</span></span>

<span data-ttu-id="bf417-110">既定では、ルックアップ フィールド (上記の `Author` など) は返されません。</span><span class="sxs-lookup"><span data-stu-id="bf417-110">Lookup fields (like `Author` above) are not returned by default.</span></span>
<span data-ttu-id="bf417-111">代わりにサーバーは、ルックアップの対象となる listItem を参照する 'LookupId' フィールド (上記の `AuthorLookupId` など) を返します。</span><span class="sxs-lookup"><span data-stu-id="bf417-111">Instead, the server returns a 'LookupId' field (like `AuthorLookupId` above) referencing the listItem targeted in the lookup.</span></span>
<span data-ttu-id="bf417-112">'LookupId' フィールドの名前は元のフィールド名の末尾に `LookupId` を付けたものです。</span><span class="sxs-lookup"><span data-stu-id="bf417-112">The name of the 'LookupId' field is the original field name followed by `LookupId`.</span></span>

<span data-ttu-id="bf417-113">1 つのクエリでは、ルックアップ フィールドを最大 12 個まで要求できます。</span><span class="sxs-lookup"><span data-stu-id="bf417-113">Up to 12 lookup fields may be requested in a single query.</span></span>
<span data-ttu-id="bf417-114">サーバーは、要求に `select` ステートメントと必要なフィールドが含まれていると、ルックアップ値を返します。</span><span class="sxs-lookup"><span data-stu-id="bf417-114">The server will return lookup values if your request includes a `select` statement with the fields you need.</span></span>
<span data-ttu-id="bf417-115">例:</span><span class="sxs-lookup"><span data-stu-id="bf417-115">Example:</span></span>

```http
GET https://graph.microsoft.com/beta/sites/{site-id}/lists/{list-id}/items?expand=fields(select=Author,BookTitle,PageCount)
```

<span data-ttu-id="bf417-116">1 つのクエリでは、最大 12 個のルックアップ フィールドと、任意の数の通常のフィールドを要求できます。</span><span class="sxs-lookup"><span data-stu-id="bf417-116">You may request up to 12 lookup fields in a single query, plus any number of regular fields.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/FieldValueSet"
} -->
