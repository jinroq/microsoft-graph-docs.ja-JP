---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 21405fe3aa28e0eef1233cd6f27e63568fb4b00e
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482218"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="0fd89-102">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0fd89-102">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0fd89-103">[columnDefinition ](columndefinition.md)リソースの\*\* choiceColumn \*\*は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="0fd89-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0fd89-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0fd89-104">JSON representation</span></span>

<span data-ttu-id="0fd89-105">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0fd89-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="0fd89-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0fd89-106">Properties</span></span>

| <span data-ttu-id="0fd89-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0fd89-107">Property name</span></span>      | <span data-ttu-id="0fd89-108">種類</span><span class="sxs-lookup"><span data-stu-id="0fd89-108">Type</span></span>               | <span data-ttu-id="0fd89-109">説明</span><span class="sxs-lookup"><span data-stu-id="0fd89-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="0fd89-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="0fd89-110">**allowTextEntry**</span></span> | <span data-ttu-id="0fd89-111">boolean</span><span class="sxs-lookup"><span data-stu-id="0fd89-111">boolean</span></span>            | <span data-ttu-id="0fd89-112">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="0fd89-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="0fd89-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="0fd89-113">**choices**</span></span>        | <span data-ttu-id="0fd89-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="0fd89-114">collection(string)</span></span> | <span data-ttu-id="0fd89-115">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="0fd89-115">The list of values available for this column.</span></span>
| <span data-ttu-id="0fd89-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="0fd89-116">**displayAs**</span></span>      | <span data-ttu-id="0fd89-117">string</span><span class="sxs-lookup"><span data-stu-id="0fd89-117">string</span></span>             | <span data-ttu-id="0fd89-118">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="0fd89-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="0fd89-119">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="0fd89-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": [
    "Error: /api-reference/beta/resources/choicecolumn.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
