---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
ms.openlocfilehash: da8398bbb87111648ea561e1799e062ed46b0ee6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021772"
---
# <a name="listinfo-resource"></a><span data-ttu-id="dd47f-102">ListInfo リソース</span><span class="sxs-lookup"><span data-stu-id="dd47f-102">ListInfo resource</span></span>

<span data-ttu-id="dd47f-103">**listInfo** 複合型は、[list][] に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="dd47f-103">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="dd47f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dd47f-105">JSON representation</span></span>

<span data-ttu-id="dd47f-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dd47f-106">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="dd47f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dd47f-107">Properties</span></span>

| <span data-ttu-id="dd47f-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="dd47f-108">Property name</span></span>           | <span data-ttu-id="dd47f-109">種類</span><span class="sxs-lookup"><span data-stu-id="dd47f-109">Type</span></span>    | <span data-ttu-id="dd47f-110">説明</span><span class="sxs-lookup"><span data-stu-id="dd47f-110">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="dd47f-111">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="dd47f-111">**contentTypesEnabled**</span></span> | <span data-ttu-id="dd47f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd47f-112">Boolean</span></span> | <span data-ttu-id="dd47f-113">`true` である場合、このリストのコンテンツ タイプが有効であることを示します。</span><span class="sxs-lookup"><span data-stu-id="dd47f-113">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="dd47f-114">**hidden**</span><span class="sxs-lookup"><span data-stu-id="dd47f-114">**hidden**</span></span>              | <span data-ttu-id="dd47f-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="dd47f-115">Boolean</span></span> | <span data-ttu-id="dd47f-116">`true` である場合、リストが通常 SharePoint ユーザー エクスペリエンスに表示されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="dd47f-116">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="dd47f-117">**template**</span><span class="sxs-lookup"><span data-stu-id="dd47f-117">**template**</span></span>            | <span data-ttu-id="dd47f-118">String</span><span class="sxs-lookup"><span data-stu-id="dd47f-118">String</span></span>  | <span data-ttu-id="dd47f-119">リストの作成に使用される基本リスト テンプレートを表す列挙値。</span><span class="sxs-lookup"><span data-stu-id="dd47f-119">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="dd47f-120">代入可能な値は `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` などです。</span><span class="sxs-lookup"><span data-stu-id="dd47f-120">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="dd47f-121">備考</span><span class="sxs-lookup"><span data-stu-id="dd47f-121">Remarks</span></span>

<span data-ttu-id="dd47f-122">ユーザーによって作成されたほとんどのリストには、上記の値のいずれかが含まれますが、それ以外の値を含めることも可能です。</span><span class="sxs-lookup"><span data-stu-id="dd47f-122">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="dd47f-123">アプリは、ここに記載されていない任意の値も処理できるようになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dd47f-123">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="dd47f-124">SharePoint の CSOM API に詳しい開発者へ: `template` の値は `SPListTemplateType` 列挙体に相当します。</span><span class="sxs-lookup"><span data-stu-id="dd47f-124">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

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
