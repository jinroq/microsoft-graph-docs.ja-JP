---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ColumnDefinition
localization_priority: Normal
ms.openlocfilehash: ddd6b3c6d3048bf7a6d3ab2dbc8ff7259651ee2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32460624"
---
# <a name="columndefinition-resource-type"></a><span data-ttu-id="af779-102">columndefinition リソースの種類</span><span class="sxs-lookup"><span data-stu-id="af779-102">columnDefinition resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

## <a name="json-representation"></a><span data-ttu-id="af779-103">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="af779-103">JSON representation</span></span>

<span data-ttu-id="af779-104">以下は、columndefinition リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="af779-104">Here is a JSON representation of a columnDefinition resource.</span></span>

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
  "geolocation": { "@odata.type": "microsoft.graph.geolocationColumn" },
  "lookup": { "@odata.type": "microsoft.graph.lookupColumn" },
  "number": { "@odata.type": "microsoft.graph.numberColumn" },
  "personOrGroup": { "@odata.type": "microsoft.graph.personOrGroupColumn" },
  "text": { "@odata.type": "microsoft.graph.textColumn" }
}
```

## <a name="properties"></a><span data-ttu-id="af779-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="af779-105">Properties</span></span>

<span data-ttu-id="af779-106">列には、さまざまな種類のデータを保持できます。</span><span class="sxs-lookup"><span data-stu-id="af779-106">Columns can hold data of various types.</span></span>
<span data-ttu-id="af779-107">次のプロパティは、列に保持されるデータの種類と、そのデータに関する追加の設定を示します。</span><span class="sxs-lookup"><span data-stu-id="af779-107">The following properties indicate what type of data a column stores, as well as additional settings for that data.</span></span>
<span data-ttu-id="af779-108">型に関連するプロパティ (boolean、演算、choice、currency、dateTime、lookup、number、個人、グループ、テキスト) は相互に排他的です。1つの列に指定できるのは1つだけです。</span><span class="sxs-lookup"><span data-stu-id="af779-108">The type-related properties (boolean, calculated, choice, currency, dateTime, lookup, number, personOrGroup, text) are mutually exclusive -- a column can only have one of them specified.</span></span>

| <span data-ttu-id="af779-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="af779-109">Property name</span></span>           | <span data-ttu-id="af779-110">種類</span><span class="sxs-lookup"><span data-stu-id="af779-110">Type</span></span>    | <span data-ttu-id="af779-111">説明</span><span class="sxs-lookup"><span data-stu-id="af779-111">Description</span></span>
|:------------------------|:--------|:-----------------------------------------
| <span data-ttu-id="af779-112">**columnGroup**</span><span class="sxs-lookup"><span data-stu-id="af779-112">**columnGroup**</span></span>         | <span data-ttu-id="af779-113">string</span><span class="sxs-lookup"><span data-stu-id="af779-113">string</span></span>  | <span data-ttu-id="af779-114">サイト列の場合、この列が属するグループの名前。</span><span class="sxs-lookup"><span data-stu-id="af779-114">For site columns, the name of the group this column belongs to.</span></span> <span data-ttu-id="af779-115">関連する列を整理するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="af779-115">Helps organize related columns.</span></span>
| <span data-ttu-id="af779-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="af779-116">**description**</span></span>         | <span data-ttu-id="af779-117">string</span><span class="sxs-lookup"><span data-stu-id="af779-117">string</span></span>  | <span data-ttu-id="af779-118">列に関するユーザー向けの説明。</span><span class="sxs-lookup"><span data-stu-id="af779-118">The user-facing description of the column.</span></span>
| <span data-ttu-id="af779-119">**displayName**</span><span class="sxs-lookup"><span data-stu-id="af779-119">**displayName**</span></span>         | <span data-ttu-id="af779-120">string</span><span class="sxs-lookup"><span data-stu-id="af779-120">string</span></span>  | <span data-ttu-id="af779-121">列を示すユーザー向けの名前。</span><span class="sxs-lookup"><span data-stu-id="af779-121">The user-facing name of the column.</span></span>
| <span data-ttu-id="af779-122">**enforceUniqueValues**</span><span class="sxs-lookup"><span data-stu-id="af779-122">**enforceUniqueValues**</span></span> | <span data-ttu-id="af779-123">ブール値</span><span class="sxs-lookup"><span data-stu-id="af779-123">boolean</span></span> | <span data-ttu-id="af779-124">True の場合、この列で 2 つのリスト アイテムの値を同じにすることはできません。</span><span class="sxs-lookup"><span data-stu-id="af779-124">If true, no two list items may have the same value for this column.</span></span>
| <span data-ttu-id="af779-125">**hidden**</span><span class="sxs-lookup"><span data-stu-id="af779-125">**hidden**</span></span>              | <span data-ttu-id="af779-126">ブール値</span><span class="sxs-lookup"><span data-stu-id="af779-126">boolean</span></span> | <span data-ttu-id="af779-127">この列がユーザー インターフェイスに表示されるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="af779-127">Specifies whether the column is displayed in the user interface.</span></span>
| <span data-ttu-id="af779-128">**id**</span><span class="sxs-lookup"><span data-stu-id="af779-128">**id**</span></span>                  | <span data-ttu-id="af779-129">string</span><span class="sxs-lookup"><span data-stu-id="af779-129">string</span></span>  | <span data-ttu-id="af779-130">列の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="af779-130">The unique identifier for the column.</span></span>
| <span data-ttu-id="af779-131">**indexed**</span><span class="sxs-lookup"><span data-stu-id="af779-131">**indexed**</span></span>             | <span data-ttu-id="af779-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="af779-132">boolean</span></span> | <span data-ttu-id="af779-133">列の値を、並べ替えと検索に使用できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="af779-133">Specifies whether the column values can used for sorting and searching.</span></span>
| <span data-ttu-id="af779-134">**name**</span><span class="sxs-lookup"><span data-stu-id="af779-134">**name**</span></span>                | <span data-ttu-id="af779-135">string</span><span class="sxs-lookup"><span data-stu-id="af779-135">string</span></span>  | <span data-ttu-id="af779-136">[listItem][] の [fields][] に表示される、列を示す API 向けの名前。</span><span class="sxs-lookup"><span data-stu-id="af779-136">The API-facing name of the column as it appears in the [fields][] on a [listItem][].</span></span> <span data-ttu-id="af779-137">ユーザー向けの名前については **displayName** をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="af779-137">For the user-facing name, see **displayName**.</span></span>
| <span data-ttu-id="af779-138">**readOnly**</span><span class="sxs-lookup"><span data-stu-id="af779-138">**readOnly**</span></span>            | <span data-ttu-id="af779-139">bool</span><span class="sxs-lookup"><span data-stu-id="af779-139">bool</span></span>    | <span data-ttu-id="af779-140">列の値を変更できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="af779-140">Specifies whether the column values can be modified.</span></span>
| <span data-ttu-id="af779-141">**required**</span><span class="sxs-lookup"><span data-stu-id="af779-141">**required**</span></span>            | <span data-ttu-id="af779-142">boolean</span><span class="sxs-lookup"><span data-stu-id="af779-142">boolean</span></span> | <span data-ttu-id="af779-143">列の値が省略不可であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="af779-143">Specifies whether the column value is not optional.</span></span>
| <span data-ttu-id="af779-144">**boolean**</span><span class="sxs-lookup"><span data-stu-id="af779-144">**boolean**</span></span>       | <span data-ttu-id="af779-145">[booleanColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-145">[booleanColumn][]</span></span>       | <span data-ttu-id="af779-146">この列にはブール値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="af779-146">This column stores boolean values.</span></span>
| <span data-ttu-id="af779-147">**calculated**</span><span class="sxs-lookup"><span data-stu-id="af779-147">**calculated**</span></span>    | <span data-ttu-id="af779-148">[calculatedColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-148">[calculatedColumn][]</span></span>    | <span data-ttu-id="af779-149">この列のデータは、他の列に基づいて計算されます。</span><span class="sxs-lookup"><span data-stu-id="af779-149">This column's data is calculated based on other columns.</span></span>
| <span data-ttu-id="af779-150">**choice**</span><span class="sxs-lookup"><span data-stu-id="af779-150">**choice**</span></span>        | <span data-ttu-id="af779-151">[choiceColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-151">[choiceColumn][]</span></span>        | <span data-ttu-id="af779-152">この列には、選択肢リストからのデータが格納されます。</span><span class="sxs-lookup"><span data-stu-id="af779-152">This column stores data from a list of choices.</span></span>
| <span data-ttu-id="af779-153">**currency**</span><span class="sxs-lookup"><span data-stu-id="af779-153">**currency**</span></span>      | <span data-ttu-id="af779-154">[currencyColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-154">[currencyColumn][]</span></span>      | <span data-ttu-id="af779-155">この列には通貨値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="af779-155">This column stores currency values.</span></span>
| <span data-ttu-id="af779-156">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="af779-156">**dateTime**</span></span>      | <span data-ttu-id="af779-157">[dateTimeColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-157">[dateTimeColumn][]</span></span>      | <span data-ttu-id="af779-158">この列には日時の値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="af779-158">This column stores DateTime values.</span></span>
| <span data-ttu-id="af779-159">**defaultValue**</span><span class="sxs-lookup"><span data-stu-id="af779-159">**defaultValue**</span></span>  | <span data-ttu-id="af779-160">[defaultColumnValue][]</span><span class="sxs-lookup"><span data-stu-id="af779-160">[defaultColumnValue][]</span></span>  | <span data-ttu-id="af779-161">この列の既定値です。</span><span class="sxs-lookup"><span data-stu-id="af779-161">The default value for this column.</span></span>
| <span data-ttu-id="af779-162">**地理位置情報**</span><span class="sxs-lookup"><span data-stu-id="af779-162">**geolocation**</span></span>   | <span data-ttu-id="af779-163">[geolocationcolumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-163">[geolocationColumn][]</span></span>   | <span data-ttu-id="af779-164">この列には、地理位置情報が格納されます。</span><span class="sxs-lookup"><span data-stu-id="af779-164">This column stores a geolocation.</span></span>
| <span data-ttu-id="af779-165">**lookup**</span><span class="sxs-lookup"><span data-stu-id="af779-165">**lookup**</span></span>        | <span data-ttu-id="af779-166">[lookupColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-166">[lookupColumn][]</span></span>        | <span data-ttu-id="af779-167">この列のデータは、サイト内の別のソースから検索されます。</span><span class="sxs-lookup"><span data-stu-id="af779-167">This column's data is looked up from another source in the site.</span></span>
| <span data-ttu-id="af779-168">**number**</span><span class="sxs-lookup"><span data-stu-id="af779-168">**number**</span></span>        | <span data-ttu-id="af779-169">[numberColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-169">[numberColumn][]</span></span>        | <span data-ttu-id="af779-170">この列には数値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="af779-170">This column stores number values.</span></span>
| <span data-ttu-id="af779-171">**personOrGroup**</span><span class="sxs-lookup"><span data-stu-id="af779-171">**personOrGroup**</span></span> | <span data-ttu-id="af779-172">[personOrGroupColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-172">[personOrGroupColumn][]</span></span> | <span data-ttu-id="af779-173">この列にはユーザーまたはグループの値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="af779-173">This column stores Person or Group values.</span></span>
| <span data-ttu-id="af779-174">**text**</span><span class="sxs-lookup"><span data-stu-id="af779-174">**text**</span></span>          | <span data-ttu-id="af779-175">[textColumn][]</span><span class="sxs-lookup"><span data-stu-id="af779-175">[textColumn][]</span></span>          | <span data-ttu-id="af779-176">この列にはテキスト値が格納されます。</span><span class="sxs-lookup"><span data-stu-id="af779-176">This column stores text values.</span></span>

><span data-ttu-id="af779-177">**注:** これらのプロパティは、SharePoint の[SPFieldType][]列挙に対応しています。</span><span class="sxs-lookup"><span data-stu-id="af779-177">**Note:** These properties correspond to SharePoint's [SPFieldType][] enumeration.</span></span>
<span data-ttu-id="af779-178">最も一般的なフィールドの種類は上記の表で表されていますが、このベータ版 API にはまだ不足しています。</span><span class="sxs-lookup"><span data-stu-id="af779-178">While the most common field types are represented in the previous table, this beta API is still missing some.</span></span>
<span data-ttu-id="af779-179">そのような場合、どの列タイプ ファセットも入力されず、基本的なプロパティだけが列に含まれます。</span><span class="sxs-lookup"><span data-stu-id="af779-179">In those cases, none of the column type facets will be populated, and the column will only have its basic properties.</span></span>

## <a name="remarks"></a><span data-ttu-id="af779-180">備考</span><span class="sxs-lookup"><span data-stu-id="af779-180">Remarks</span></span>

<span data-ttu-id="af779-181">`hidden` 列の ColumnDefinitions とフィールドの値は、既定では表示されません。</span><span class="sxs-lookup"><span data-stu-id="af779-181">ColumnDefinitions and field values for `hidden` columns are not shown by default.</span></span>
<span data-ttu-id="af779-182">**columnDefinitions** を一覧表示するときにこれらが表示されるようにするには、`$select` ステートメントに `hidden` を含めます。</span><span class="sxs-lookup"><span data-stu-id="af779-182">To see them when listing **columnDefinitions**, include `hidden` in your `$select` statement.</span></span>
<span data-ttu-id="af779-183">[listItems][listItem] の**フィールド**値を表示するときにこれらが表示されるようにするには、`$select` ステートメントに目的の列の名前を含めます。</span><span class="sxs-lookup"><span data-stu-id="af779-183">To see them when showing **field** values on [listItems][listItem], include the desired columns by name in your `$select` statement.</span></span>

[booleanColumn]: booleancolumn.md
[calculatedColumn]: calculatedcolumn.md
[choiceColumn]: choicecolumn.md
[currencyColumn]: currencycolumn.md
[dateTimeColumn]: datetimecolumn.md
[defaultColumnValue]: defaultcolumnvalue.md
[geolocationcolumn]: geolocationcolumn.md
[geolocationColumn]: geolocationcolumn.md
[lookupColumn]: lookupcolumn.md
[numberColumn]: numbercolumn.md
[personOrGroupColumn]: personorgroupcolumn.md
[textColumn]: textcolumn.md
[fieldValueSet]: fieldvalueset.md
[fields]: fieldvalueset.md
[listItem]: listitem.md

[SPFieldType]: https://msdn.microsoft.com/library/microsoft.sharepoint.spfieldtype.aspx

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ColumnDefinition",
  "suppressions": [
    "Error: /api-reference/beta/resources/columndefinition.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
