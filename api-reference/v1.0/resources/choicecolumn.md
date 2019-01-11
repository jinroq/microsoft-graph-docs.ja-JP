---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 3640e68902485215dda575cc93407f019007ee18
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826580"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="20ae8-102">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20ae8-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="20ae8-103">[columnDefinition ](columndefinition.md)リソースの\*\* choiceColumn \*\*は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="20ae8-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20ae8-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20ae8-104">JSON representation</span></span>

<span data-ttu-id="20ae8-105">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20ae8-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="20ae8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20ae8-106">Properties</span></span>

| <span data-ttu-id="20ae8-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="20ae8-107">Property name</span></span>      | <span data-ttu-id="20ae8-108">種類</span><span class="sxs-lookup"><span data-stu-id="20ae8-108">Type</span></span>               | <span data-ttu-id="20ae8-109">説明</span><span class="sxs-lookup"><span data-stu-id="20ae8-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="20ae8-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="20ae8-110">**allowTextEntry**</span></span> | <span data-ttu-id="20ae8-111">boolean</span><span class="sxs-lookup"><span data-stu-id="20ae8-111">boolean</span></span>            | <span data-ttu-id="20ae8-112">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="20ae8-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="20ae8-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="20ae8-113">**choices**</span></span>        | <span data-ttu-id="20ae8-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="20ae8-114">collection(string)</span></span> | <span data-ttu-id="20ae8-115">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="20ae8-115">The list of values available for this column.</span></span>
| <span data-ttu-id="20ae8-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="20ae8-116">**displayAs**</span></span>      | <span data-ttu-id="20ae8-117">string</span><span class="sxs-lookup"><span data-stu-id="20ae8-117">string</span></span>             | <span data-ttu-id="20ae8-118">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="20ae8-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="20ae8-119">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="20ae8-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/choicecolumn.md:
      Found potential enums in resource example that weren't defined in a table:(checkBoxes,dropDownMenu,radioButtons) are in resource, but () are in table"
  ],
  "tocPath": "Resources/ChoiceColumn"
} -->
