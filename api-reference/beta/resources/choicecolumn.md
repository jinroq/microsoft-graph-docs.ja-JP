---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 21405fe3aa28e0eef1233cd6f27e63568fb4b00e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543779"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="a47f0-102">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a47f0-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="a47f0-103">[columnDefinition ](columndefinition.md)リソースの\*\* choiceColumn \*\*は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="a47f0-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a47f0-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a47f0-104">JSON representation</span></span>

<span data-ttu-id="a47f0-105">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a47f0-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="a47f0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a47f0-106">Properties</span></span>

| <span data-ttu-id="a47f0-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="a47f0-107">Property name</span></span>      | <span data-ttu-id="a47f0-108">種類</span><span class="sxs-lookup"><span data-stu-id="a47f0-108">Type</span></span>               | <span data-ttu-id="a47f0-109">説明</span><span class="sxs-lookup"><span data-stu-id="a47f0-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="a47f0-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="a47f0-110">**allowTextEntry**</span></span> | <span data-ttu-id="a47f0-111">boolean</span><span class="sxs-lookup"><span data-stu-id="a47f0-111">boolean</span></span>            | <span data-ttu-id="a47f0-112">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="a47f0-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="a47f0-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="a47f0-113">**choices**</span></span>        | <span data-ttu-id="a47f0-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="a47f0-114">collection(string)</span></span> | <span data-ttu-id="a47f0-115">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="a47f0-115">The list of values available for this column.</span></span>
| <span data-ttu-id="a47f0-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="a47f0-116">**displayAs**</span></span>      | <span data-ttu-id="a47f0-117">string</span><span class="sxs-lookup"><span data-stu-id="a47f0-117">string</span></span>             | <span data-ttu-id="a47f0-118">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="a47f0-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="a47f0-119">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="a47f0-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
