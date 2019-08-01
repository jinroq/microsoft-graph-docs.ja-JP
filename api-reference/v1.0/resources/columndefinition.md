---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
description: 以下は、ColumnDefinition リソースの JSON 表記です。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3a02721c5289b1d49077e1b2d9fa1017f0c53021
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032873"
---
# <a name="columndefinition-resource"></a><span data-ttu-id="45cc6-103">ColumnDefinition リソース</span><span class="sxs-lookup"><span data-stu-id="45cc6-103">ColumnDefinition resource</span></span>

## <a name="json-representation"></a><span data-ttu-id="45cc6-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="45cc6-104">JSON representation</span></span>

<span data-ttu-id="45cc6-105">以下は、ColumnDefinition リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="45cc6-105">Here is a JSON representation of a ColumnDefinition resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.columnDefinition"
}-->

```json
{
  "columnGroup": "string",
  "description": "description",
  "displayName": "friendly name",
  "enforceUniqueValues": "true",
  "hidden": false,
  "id": "string",
  "indexed": true,
  "name": "staticNameForApi",
  "readOnly": false,
  "required": false,
  "boolean": { "@odata.type": "microsoft.graph.booleanColumn" },
  "calculated": { "@odata.type": "microsoft.graph.calculatedColumn" },
  "choice": { "@odata.type": "microsoft.graph.choiceColumn" },
  "currency": { "@odata.type": "microsoft.graph.currencyColumn" },
  "dateTime": { "@odata.type": "microsoft.graph.dateTimeColumn" },
  "defaultValue": { "@odata.type": "microsoft.graph.defaultColumnValue" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="45cc6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45cc6-106">Properties</span></span>

<span data-ttu-id="45cc6-107">**columnDefinition** リソースには以下のプロパティがあります。</span><span class="sxs-lookup"><span data-stu-id="45cc6-107">The **columnDefinition** resource has the following properties.</span></span>

| <span data-ttu-id="45cc6-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="45cc6-108">Property name</span></span>           | <span data-ttu-id="45cc6-109">種類</span><span class="sxs-lookup"><span data-stu-id="45cc6-109">Type</span></span>    | <span data-ttu-id="45cc6-110">説明</span><span class="sxs-lookup"><span data-stu-id="45cc6-110">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="45cc6-111">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="45cc6-111">**columnGroup**</span></span>         | <span data-ttu-id="45cc6-112">string</span><span class="sxs-lookup"><span data-stu-id="45cc6-112">string</span></span>  | <span data-ttu-id="45cc6-113">サイト列の場合、この列が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="45cc6-113">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="45cc6-114">関連する列を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-114">Helps organize related columns.</span></span>
| <span data-ttu-id="45cc6-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="45cc6-115">**description**</span></span>         | <span data-ttu-id="45cc6-116">string</span><span class="sxs-lookup"><span data-stu-id="45cc6-116">string</span></span>  | <span data-ttu-id="45cc6-117">列に関するユーザー向けの説明。</span><span class="sxs-lookup"><span data-stu-id="45cc6-117">The user-facing description of the column.</span></span>
| <span data-ttu-id="45cc6-118">**displayName**</span><span class="sxs-lookup"><span data-stu-id="45cc6-118">**displayName**</span></span>         | <span data-ttu-id="45cc6-119">string</span><span class="sxs-lookup"><span data-stu-id="45cc6-119">string</span></span>  | <span data-ttu-id="45cc6-120">列を示すユーザー向けの名前。</span><span class="sxs-lookup"><span data-stu-id="45cc6-120">The user-facing name of the column.</span></span>
| <span data-ttu-id="45cc6-121">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="45cc6-121">**enforceUniqueValues**</span></span> | <span data-ttu-id="45cc6-122">ブール値</span><span class="sxs-lookup"><span data-stu-id="45cc6-122">boolean</span></span> | <span data-ttu-id="45cc6-123">True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="45cc6-123">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="45cc6-124">**hidden**</span><span class="sxs-lookup"><span data-stu-id="45cc6-124">**hidden**</span></span>              | <span data-ttu-id="45cc6-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="45cc6-125">boolean</span></span> | <span data-ttu-id="45cc6-126">この列がユーザー インターフェイスに表示されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="45cc6-126">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="45cc6-127">**id**</span><span class="sxs-lookup"><span data-stu-id="45cc6-127">**id**</span></span>                  | <span data-ttu-id="45cc6-128">string</span><span class="sxs-lookup"><span data-stu-id="45cc6-128">string</span></span>  | <span data-ttu-id="45cc6-129">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="45cc6-129">The unique identifier for the column.</span></span>
| <span data-ttu-id="45cc6-130">**indexed**</span><span class="sxs-lookup"><span data-stu-id="45cc6-130">**indexed**</span></span>             | <span data-ttu-id="45cc6-131">ブール値</span><span class="sxs-lookup"><span data-stu-id="45cc6-131">boolean</span></span> | <span data-ttu-id="45cc6-132">列の値を、並べ替えと検索に使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="45cc6-132">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="45cc6-133">**name**</span><span class="sxs-lookup"><span data-stu-id="45cc6-133">**name**</span></span>                | <span data-ttu-id="45cc6-134">string</span><span class="sxs-lookup"><span data-stu-id="45cc6-134">string</span></span>  | <span data-ttu-id="45cc6-135">[listItem][] の [fields][] に表示される、列を示す API 向けの名前。</span><span class="sxs-lookup"><span data-stu-id="45cc6-135">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="45cc6-136">ユーザー向けの名前については **displayName** をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="45cc6-136">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="45cc6-137">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="45cc6-137">**readOnly**</span></span>            | <span data-ttu-id="45cc6-138">bool</span><span class="sxs-lookup"><span data-stu-id="45cc6-138">bool</span></span>    | <span data-ttu-id="45cc6-139">列の値を変更できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="45cc6-139">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="45cc6-140">**required**</span><span class="sxs-lookup"><span data-stu-id="45cc6-140">**required**</span></span>            | <span data-ttu-id="45cc6-141">boolean</span><span class="sxs-lookup"><span data-stu-id="45cc6-141">boolean</span></span> | <span data-ttu-id="45cc6-142">列の値が省略不可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="45cc6-142">Specifies whether the column value is not optional.</span></span>

<span data-ttu-id="45cc6-143">列には、さまざまな種類のデータを保持できます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-143">Columns can hold data of various types.</span></span>
<span data-ttu-id="45cc6-144">次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="45cc6-144">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="45cc6-145">これらのプロパティは相互に排他的で、各列でいずれか 1 つだけを指定できます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-145">These properties are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="45cc6-146">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="45cc6-146">Property name</span></span>     | <span data-ttu-id="45cc6-147">種類</span><span class="sxs-lookup"><span data-stu-id="45cc6-147">Type</span></span>                    | <span data-ttu-id="45cc6-148">説明</span><span class="sxs-lookup"><span data-stu-id="45cc6-148">Description</span></span>
|:------------------|:------------------------|:-------------------------------
| <span data-ttu-id="45cc6-149">**boolean**</span><span class="sxs-lookup"><span data-stu-id="45cc6-149">**boolean**</span></span>       | <span data-ttu-id="45cc6-150">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-150">[booleanColumn][]</span></span>       | <span data-ttu-id="45cc6-151">この列にはブール値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-151">This column stores boolean values.</span></span>
| <span data-ttu-id="45cc6-152">**calculated**</span><span class="sxs-lookup"><span data-stu-id="45cc6-152">**calculated**</span></span>    | <span data-ttu-id="45cc6-153">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-153">[calculatedColumn][]</span></span>    | <span data-ttu-id="45cc6-154">この列のデータは、他の列に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-154">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="45cc6-155">**choice**</span><span class="sxs-lookup"><span data-stu-id="45cc6-155">**choice**</span></span>        | <span data-ttu-id="45cc6-156">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-156">[choiceColumn][]</span></span>        | <span data-ttu-id="45cc6-157">この列には、選択肢リストからのデータが格納されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-157">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="45cc6-158">**currency**</span><span class="sxs-lookup"><span data-stu-id="45cc6-158">**currency**</span></span>      | <span data-ttu-id="45cc6-159">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-159">[currencyColumn][]</span></span>      | <span data-ttu-id="45cc6-160">この列には通貨値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-160">This column stores currency values.</span></span>
| <span data-ttu-id="45cc6-161">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="45cc6-161">**dateTime**</span></span>      | <span data-ttu-id="45cc6-162">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-162">[dateTimeColumn][]</span></span>      | <span data-ttu-id="45cc6-163">この列には日時の値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-163">This column stores DateTime values.</span></span>
| <span data-ttu-id="45cc6-164">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="45cc6-164">**defaultValue**</span></span>  | <span data-ttu-id="45cc6-165">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-165">[defaultColumnValue][]</span></span>  | <span data-ttu-id="45cc6-166">この列の既定値です。</span><span class="sxs-lookup"><span data-stu-id="45cc6-166">The default value for this column.</span></span>
| <span data-ttu-id="45cc6-167">**lookup**</span><span class="sxs-lookup"><span data-stu-id="45cc6-167">**lookup**</span></span>        | <span data-ttu-id="45cc6-168">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-168">[lookupColumn][]</span></span>        | <span data-ttu-id="45cc6-169">この列のデータは、サイト内の別のソースから検索されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-169">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="45cc6-170">**number**</span><span class="sxs-lookup"><span data-stu-id="45cc6-170">**number**</span></span>        | <span data-ttu-id="45cc6-171">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-171">[numberColumn][]</span></span>        | <span data-ttu-id="45cc6-172">この列には数値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-172">This column stores number values.</span></span>
| <span data-ttu-id="45cc6-173">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="45cc6-173">**personOrGroup**</span></span> | <span data-ttu-id="45cc6-174">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-174">[personOrGroupColumn][]</span></span> | <span data-ttu-id="45cc6-175">この列にはユーザーまたはグループの値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-175">This column stores Person or Group values.</span></span>
| <span data-ttu-id="45cc6-176">**text**</span><span class="sxs-lookup"><span data-stu-id="45cc6-176">**text**</span></span>          | <span data-ttu-id="45cc6-177">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="45cc6-177">[textColumn][]</span></span>          | <span data-ttu-id="45cc6-178">この列にはテキスト値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-178">This column stores text values.</span></span>

<span data-ttu-id="45cc6-179">注: これらのプロパティは SharePoint の [SPFieldType][] 列挙体に対応しています。</span><span class="sxs-lookup"><span data-stu-id="45cc6-179">Note: These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="45cc6-180">最も一般的なフィールドの種類は上記のとおりですが、この API はまだ一部不足しています。</span><span class="sxs-lookup"><span data-stu-id="45cc6-180">While the most common field types are represented above, this API is still missing some.</span></span>
<span data-ttu-id="45cc6-181">そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-181">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="45cc6-182">備考</span><span class="sxs-lookup"><span data-stu-id="45cc6-182">Remarks</span></span>

<span data-ttu-id="45cc6-183">`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。</span><span class="sxs-lookup"><span data-stu-id="45cc6-183">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="45cc6-184">**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-184">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="45cc6-185">[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。</span><span class="sxs-lookup"><span data-stu-id="45cc6-185">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition"
} -->
