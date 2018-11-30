---
title: NamedItem リソースの種類
description: セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。
ms.openlocfilehash: 11ca12e0ae094f0e682cfde5fb1fe1feecabdb9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070164"
---
# <a name="nameditem-resource-type"></a><span data-ttu-id="bcaf1-105">NamedItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bcaf1-105">NamedItem resource type</span></span>

<span data-ttu-id="bcaf1-p102">セルまたは値の範囲の定義済みの名前を表します。名前には、(以下の型に見られるような) プリミティブ名前付きオブジェクト、範囲オブジェクト、範囲への参照を設定できます。このオブジェクトを使用して、名前に関連付けられた範囲オブジェクトを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-p102">Represents a defined name for a range of cells or value. Names can be primitive named objects (as seen in the type below), range object, reference to a range. This object can be used to obtain range object associated with names.</span></span>


## <a name="methods"></a><span data-ttu-id="bcaf1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcaf1-109">Methods</span></span>

| <span data-ttu-id="bcaf1-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="bcaf1-110">Method</span></span>           | <span data-ttu-id="bcaf1-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bcaf1-111">Return Type</span></span>    |<span data-ttu-id="bcaf1-112">説明</span><span class="sxs-lookup"><span data-stu-id="bcaf1-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bcaf1-113">追加</span><span class="sxs-lookup"><span data-stu-id="bcaf1-113">Add</span></span>](../api/nameditem-add.md)|[<span data-ttu-id="bcaf1-114">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bcaf1-114">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="bcaf1-115">新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-115">Adds a new name to the collection of the given scope.</span></span>|
|[<span data-ttu-id="bcaf1-116">AddFormulaLocal</span><span class="sxs-lookup"><span data-stu-id="bcaf1-116">AddFormulaLocal</span></span>](../api/nameditem-addformulalocal.md)|[<span data-ttu-id="bcaf1-117">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bcaf1-117">NamedItem</span></span>](nameditem.md)|<span data-ttu-id="bcaf1-118">ユーザーのロケールを数式に使用して、新しい名前を指定したスコープのコレクションに追加します。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-118">Adds a new name to the collection of the given scope using the user's locale for the formula.</span></span>|
|[<span data-ttu-id="bcaf1-119">NamedItem を取得する</span><span class="sxs-lookup"><span data-stu-id="bcaf1-119">Get NamedItem</span></span>](../api/nameditem-get.md) | [<span data-ttu-id="bcaf1-120">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bcaf1-120">NamedItem</span></span>](nameditem.md) |<span data-ttu-id="bcaf1-121">namedItem オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-121">Read properties and relationships of namedItem object.</span></span>|
|[<span data-ttu-id="bcaf1-122">Update</span><span class="sxs-lookup"><span data-stu-id="bcaf1-122">Update</span></span>](../api/nameditem-update.md) | [<span data-ttu-id="bcaf1-123">NamedItem</span><span class="sxs-lookup"><span data-stu-id="bcaf1-123">NamedItem</span></span>](nameditem.md)   |<span data-ttu-id="bcaf1-124">NamedItem オブジェクトを更新します。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-124">Update NamedItem object.</span></span> |
|[<span data-ttu-id="bcaf1-125">Range</span><span class="sxs-lookup"><span data-stu-id="bcaf1-125">Range</span></span>](../api/nameditem-range.md)|[<span data-ttu-id="bcaf1-126">Range</span><span class="sxs-lookup"><span data-stu-id="bcaf1-126">Range</span></span>](range.md)|<span data-ttu-id="bcaf1-p103">名前に関連付けられている範囲オブジェクトを返します。名前付き項目の型が範囲でない場合、例外をスローします。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-p103">Returns the range object that is associated with the name. Throws an exception if the named item's type is not a range.</span></span>|
|[<span data-ttu-id="bcaf1-129">List</span><span class="sxs-lookup"><span data-stu-id="bcaf1-129">List</span></span>](../api/nameditem-list.md) | <span data-ttu-id="bcaf1-130">[NamedItem](nameditem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bcaf1-130">[NamedItem](nameditem.md) collection</span></span> |<span data-ttu-id="bcaf1-131">namedItem オブジェクトのコレクションを取得します。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-131">Get namedItem object collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="bcaf1-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcaf1-132">Properties</span></span>
| <span data-ttu-id="bcaf1-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bcaf1-133">Property</span></span>     | <span data-ttu-id="bcaf1-134">型</span><span class="sxs-lookup"><span data-stu-id="bcaf1-134">Type</span></span>   |<span data-ttu-id="bcaf1-135">説明</span><span class="sxs-lookup"><span data-stu-id="bcaf1-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcaf1-136">name</span><span class="sxs-lookup"><span data-stu-id="bcaf1-136">name</span></span>|<span data-ttu-id="bcaf1-137">string</span><span class="sxs-lookup"><span data-stu-id="bcaf1-137">string</span></span>|<span data-ttu-id="bcaf1-p104">オブジェクトの名前。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-p104">The name of the object. Read-only.</span></span>|
|<span data-ttu-id="bcaf1-140">comment</span><span class="sxs-lookup"><span data-stu-id="bcaf1-140">comment</span></span>|<span data-ttu-id="bcaf1-141">文字列</span><span class="sxs-lookup"><span data-stu-id="bcaf1-141">string</span></span>|<span data-ttu-id="bcaf1-142">この名前に関連付けられているコメントを表します。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-142">Represents the comment associated with this name.</span></span>|
|<span data-ttu-id="bcaf1-143">scope</span><span class="sxs-lookup"><span data-stu-id="bcaf1-143">scope</span></span>|<span data-ttu-id="bcaf1-144">string</span><span class="sxs-lookup"><span data-stu-id="bcaf1-144">string</span></span>|<span data-ttu-id="bcaf1-p105">名前がブックを対象にしているのか、特定のワークシートを対象にしているのかを示します。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-p105">Indicates whether the name is scoped to the workbook or to a specific worksheet. Read-only.</span></span>|
|<span data-ttu-id="bcaf1-147">type</span><span class="sxs-lookup"><span data-stu-id="bcaf1-147">type</span></span>|<span data-ttu-id="bcaf1-148">文字列</span><span class="sxs-lookup"><span data-stu-id="bcaf1-148">string</span></span>|<span data-ttu-id="bcaf1-p106">名前に関連付けられている参照の型を示します。可能な値は、`String`、`Integer`、`Double`、`Boolean`、`Range` です。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-p106">Indicates what type of reference is associated with the name. Possible values are: `String`, `Integer`, `Double`, `Boolean`, `Range`. Read-only.</span></span>|
|<span data-ttu-id="bcaf1-152">value</span><span class="sxs-lookup"><span data-stu-id="bcaf1-152">value</span></span>|<span data-ttu-id="bcaf1-153">文字列</span><span class="sxs-lookup"><span data-stu-id="bcaf1-153">string</span></span>|<span data-ttu-id="bcaf1-p107">定義されている名前が参照する数式を表します。例: =Sheet14!$B$2:$H$12、=4.75, など。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-p107">Represents the formula that the name is defined to refer to. E.g. =Sheet14!$B$2:$H$12, =4.75, etc. Read-only.</span></span>|
|<span data-ttu-id="bcaf1-157">visible</span><span class="sxs-lookup"><span data-stu-id="bcaf1-157">visible</span></span>|<span data-ttu-id="bcaf1-158">ブール値</span><span class="sxs-lookup"><span data-stu-id="bcaf1-158">boolean</span></span>|<span data-ttu-id="bcaf1-159">オブジェクトを表示するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-159">Specifies whether the object is visible or not.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bcaf1-160">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcaf1-160">Relationships</span></span>
| <span data-ttu-id="bcaf1-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bcaf1-161">Relationship</span></span>     | <span data-ttu-id="bcaf1-162">型</span><span class="sxs-lookup"><span data-stu-id="bcaf1-162">Type</span></span>   |<span data-ttu-id="bcaf1-163">説明</span><span class="sxs-lookup"><span data-stu-id="bcaf1-163">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bcaf1-164">ワークシート</span><span class="sxs-lookup"><span data-stu-id="bcaf1-164">worksheet</span></span>|[<span data-ttu-id="bcaf1-165">worksheet</span><span class="sxs-lookup"><span data-stu-id="bcaf1-165">worksheet</span></span>](worksheet.md)|<span data-ttu-id="bcaf1-p108">名前付きのアイテムの対象になるワークシートを返します。アイテムの対象がワークシートの場合にのみ使用できます。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-p108">Returns the worksheet on which the named item is scoped to. Available only if the item is scoped to the worksheet. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bcaf1-169">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bcaf1-169">JSON representation</span></span>

<span data-ttu-id="bcaf1-170">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bcaf1-170">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.namedItem"
}-->

```json
{
  "name": "string",
  "comment": "string",
  "scope": "string",
  "type": "string",
  "value": "string",
  "visible": true
  
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "NamedItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->