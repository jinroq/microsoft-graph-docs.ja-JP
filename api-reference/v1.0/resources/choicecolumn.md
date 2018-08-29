---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 9feb49fc9c581a4518f63a0367087d54de32cff4
ms.sourcegitcommit: abf4b739257e3ffd9d045f783ec595d846172590
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/21/2018
ms.locfileid: "23264071"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="3a8e3-102">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3a8e3-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="3a8e3-103">[columnDefinition ](columnDefinition.md)リソースの** choiceColumn **は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="3a8e3-103">The **choiceColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a8e3-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3a8e3-104">JSON representation</span></span>

<span data-ttu-id="3a8e3-105">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3a8e3-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="3a8e3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3a8e3-106">Properties</span></span>

| <span data-ttu-id="3a8e3-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="3a8e3-107">Property name</span></span>      | <span data-ttu-id="3a8e3-108">型</span><span class="sxs-lookup"><span data-stu-id="3a8e3-108">Type</span></span>               | <span data-ttu-id="3a8e3-109">説明</span><span class="sxs-lookup"><span data-stu-id="3a8e3-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="3a8e3-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="3a8e3-110">**allowTextEntry**</span></span> | <span data-ttu-id="3a8e3-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="3a8e3-111">boolean</span></span>            | <span data-ttu-id="3a8e3-112">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="3a8e3-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="3a8e3-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="3a8e3-113">**choices**</span></span>        | <span data-ttu-id="3a8e3-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="3a8e3-114">collection(string)</span></span> | <span data-ttu-id="3a8e3-115">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="3a8e3-115">The list of values available for this column.</span></span>
| <span data-ttu-id="3a8e3-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="3a8e3-116">**displayAs**</span></span>      | <span data-ttu-id="3a8e3-117">文字列</span><span class="sxs-lookup"><span data-stu-id="3a8e3-117">string</span></span>             | <span data-ttu-id="3a8e3-118">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="3a8e3-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="3a8e3-119">、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。 `radioButtons`</span><span class="sxs-lookup"><span data-stu-id="3a8e3-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
