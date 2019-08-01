---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
description: columnDefinition リソースの choiceColumn は、選択肢のリストから列の値を選択できることを示します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: a86cb783fb170c2b9528b47272fc214ea0010760
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029737"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="9e455-103">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9e455-103">ChoiceColumn resource type</span></span>

<span data-ttu-id="9e455-104">[columnDefinition ](columndefinition.md)リソースの\*\* choiceColumn \*\*は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="9e455-104">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e455-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9e455-105">JSON representation</span></span>

<span data-ttu-id="9e455-106">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9e455-106">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="9e455-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e455-107">Properties</span></span>

| <span data-ttu-id="9e455-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9e455-108">Property name</span></span>      | <span data-ttu-id="9e455-109">種類</span><span class="sxs-lookup"><span data-stu-id="9e455-109">Type</span></span>               | <span data-ttu-id="9e455-110">説明</span><span class="sxs-lookup"><span data-stu-id="9e455-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="9e455-111">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="9e455-111">**allowTextEntry**</span></span> | <span data-ttu-id="9e455-112">boolean</span><span class="sxs-lookup"><span data-stu-id="9e455-112">boolean</span></span>            | <span data-ttu-id="9e455-113">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="9e455-113">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="9e455-114">**choices**</span><span class="sxs-lookup"><span data-stu-id="9e455-114">**choices**</span></span>        | <span data-ttu-id="9e455-115">collection(string)</span><span class="sxs-lookup"><span data-stu-id="9e455-115">collection(string)</span></span> | <span data-ttu-id="9e455-116">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="9e455-116">The list of values available for this column.</span></span>
| <span data-ttu-id="9e455-117">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="9e455-117">**displayAs**</span></span>      | <span data-ttu-id="9e455-118">string</span><span class="sxs-lookup"><span data-stu-id="9e455-118">string</span></span>             | <span data-ttu-id="9e455-119">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="9e455-119">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="9e455-120">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9e455-120">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
