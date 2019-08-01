---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.prod: sharepoint
description: listInfo 複合型は、list に関する追加情報を提供します。
doc_type: resourcePageType
ms.openlocfilehash: dd6b2d892746c5aafc599b988113aefaa0b9973d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036415"
---
# <a name="listinfo-resource"></a><span data-ttu-id="6ba9a-103">ListInfo リソース</span><span class="sxs-lookup"><span data-stu-id="6ba9a-103">ListInfo resource</span></span>

<span data-ttu-id="6ba9a-104">**listInfo** 複合型は、[list][] に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-104">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="6ba9a-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ba9a-106">JSON representation</span></span>

<span data-ttu-id="6ba9a-107">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.listInfo"
}-->

```json
{
  "contentTypesEnabled": false,
  "hidden": false,
  "template": "documentLibrary | genericList | tasks | survey | links | announcements | contacts | ..."
}
```

## <a name="properties"></a><span data-ttu-id="6ba9a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ba9a-108">Properties</span></span>

| <span data-ttu-id="6ba9a-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6ba9a-109">Property name</span></span>           | <span data-ttu-id="6ba9a-110">種類</span><span class="sxs-lookup"><span data-stu-id="6ba9a-110">Type</span></span>    | <span data-ttu-id="6ba9a-111">説明</span><span class="sxs-lookup"><span data-stu-id="6ba9a-111">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="6ba9a-112">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="6ba9a-112">**contentTypesEnabled**</span></span> | <span data-ttu-id="6ba9a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ba9a-113">Boolean</span></span> | <span data-ttu-id="6ba9a-114">`true` である場合、このリストのコンテンツ タイプが有効であることを示します。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-114">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="6ba9a-115">**hidden**</span><span class="sxs-lookup"><span data-stu-id="6ba9a-115">**hidden**</span></span>              | <span data-ttu-id="6ba9a-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ba9a-116">Boolean</span></span> | <span data-ttu-id="6ba9a-117">`true` である場合、リストが通常 SharePoint ユーザー エクスペリエンスに表示されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-117">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="6ba9a-118">**template**</span><span class="sxs-lookup"><span data-stu-id="6ba9a-118">**template**</span></span>            | <span data-ttu-id="6ba9a-119">String</span><span class="sxs-lookup"><span data-stu-id="6ba9a-119">String</span></span>  | <span data-ttu-id="6ba9a-120">リストの作成に使用される基本リスト テンプレートを表す列挙値。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-120">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="6ba9a-121">代入可能な値は `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` などです。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-121">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="6ba9a-122">備考</span><span class="sxs-lookup"><span data-stu-id="6ba9a-122">Remarks</span></span>

<span data-ttu-id="6ba9a-123">ユーザーによって作成されたほとんどのリストには、上記の値のいずれかが含まれますが、それ以外の値を含めることも可能です。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-123">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="6ba9a-124">アプリは、ここに記載されていない任意の値も処理できるようになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-124">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="6ba9a-125">SharePoint の CSOM API に詳しい開発者へ: `template` の値は `SPListTemplateType` 列挙体に相当します。</span><span class="sxs-lookup"><span data-stu-id="6ba9a-125">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/listinfo.md:
      Found potential enums in resource example that weren't defined in a table:(documentLibrary,genericList,tasks,survey,links,announcements,contacts,...) are in resource, but () are in table"
  ],
  "tocPath": ""
}-->
