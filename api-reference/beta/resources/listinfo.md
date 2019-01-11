---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ListInfo
localization_priority: Normal
ms.openlocfilehash: c1a29099264c46f32e09b375a97ff49c13c99c6f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858458"
---
# <a name="listinfo-resource"></a><span data-ttu-id="a814e-102">ListInfo リソース</span><span class="sxs-lookup"><span data-stu-id="a814e-102">ListInfo resource</span></span>

> <span data-ttu-id="a814e-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a814e-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a814e-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a814e-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a814e-105">**listInfo** 複合型は、[list][] に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a814e-105">The **listInfo** complex type provides additional information about a [list][].</span></span>

[list]: list.md

## <a name="json-representation"></a><span data-ttu-id="a814e-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a814e-107">JSON representation</span></span>

<span data-ttu-id="a814e-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a814e-108">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="a814e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a814e-109">Properties</span></span>

| <span data-ttu-id="a814e-110">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a814e-110">Property name</span></span>           | <span data-ttu-id="a814e-111">Type</span><span class="sxs-lookup"><span data-stu-id="a814e-111">Type</span></span>    | <span data-ttu-id="a814e-112">説明</span><span class="sxs-lookup"><span data-stu-id="a814e-112">Description</span></span>
|:------------------------|:--------|:------------------------------------------------
| <span data-ttu-id="a814e-113">**contentTypesEnabled**</span><span class="sxs-lookup"><span data-stu-id="a814e-113">**contentTypesEnabled**</span></span> | <span data-ttu-id="a814e-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="a814e-114">Boolean</span></span> | <span data-ttu-id="a814e-115">`true` である場合、このリストのコンテンツ タイプが有効であることを示します。</span><span class="sxs-lookup"><span data-stu-id="a814e-115">If `true`, indicates that content types are enabled for this list.</span></span>
| <span data-ttu-id="a814e-116">**hidden**</span><span class="sxs-lookup"><span data-stu-id="a814e-116">**hidden**</span></span>              | <span data-ttu-id="a814e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a814e-117">Boolean</span></span> | <span data-ttu-id="a814e-118">`true` である場合、リストが通常 SharePoint ユーザー エクスペリエンスに表示されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a814e-118">If `true`, indicates that the list is not normally visible in the SharePoint user experience.</span></span>
| <span data-ttu-id="a814e-119">**template**</span><span class="sxs-lookup"><span data-stu-id="a814e-119">**template**</span></span>            | <span data-ttu-id="a814e-120">String</span><span class="sxs-lookup"><span data-stu-id="a814e-120">String</span></span>  | <span data-ttu-id="a814e-121">リストの作成に使用される基本リスト テンプレートを表す列挙値。</span><span class="sxs-lookup"><span data-stu-id="a814e-121">An enumerated value that represents the base list template used in creating the list.</span></span> <span data-ttu-id="a814e-122">代入可能な値は `documentLibrary`、`genericList`、`task`、`survey`、`announcements`、`contacts` などです。</span><span class="sxs-lookup"><span data-stu-id="a814e-122">Possible values include `documentLibrary`, `genericList`, `task`, `survey`, `announcements`, `contacts`, and more.</span></span>

### <a name="remarks"></a><span data-ttu-id="a814e-123">備考</span><span class="sxs-lookup"><span data-stu-id="a814e-123">Remarks</span></span>

<span data-ttu-id="a814e-124">ユーザーによって作成されたほとんどのリストには、上記の値のいずれかが含まれますが、それ以外の値を含めることも可能です。</span><span class="sxs-lookup"><span data-stu-id="a814e-124">While most lists created by users will have one of the values listed above, other values are possible as well.</span></span>
<span data-ttu-id="a814e-125">アプリは、ここに記載されていない任意の値も処理できるようになっている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a814e-125">Your app should be prepared to handle any values that are not listed here.</span></span>
<span data-ttu-id="a814e-126">SharePoint の CSOM API に詳しい開発者へ: `template` の値は `SPListTemplateType` 列挙体に相当します。</span><span class="sxs-lookup"><span data-stu-id="a814e-126">For developers familiar with SharePoint's CSOM APIs, the `template` value corresponds to the `SPListTemplateType` enumeration.</span></span>

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
