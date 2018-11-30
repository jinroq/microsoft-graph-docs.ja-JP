---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 6841f453cdfd423ead3edeea5895242a28b998f3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020829"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="52d9c-102">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="52d9c-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="52d9c-103">[columnDefinition ](columndefinition.md)リソースの\*\* choiceColumn \*\*は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="52d9c-103">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52d9c-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52d9c-104">JSON representation</span></span>

<span data-ttu-id="52d9c-105">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52d9c-105">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="52d9c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52d9c-106">Properties</span></span>

| <span data-ttu-id="52d9c-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="52d9c-107">Property name</span></span>      | <span data-ttu-id="52d9c-108">種類</span><span class="sxs-lookup"><span data-stu-id="52d9c-108">Type</span></span>               | <span data-ttu-id="52d9c-109">説明</span><span class="sxs-lookup"><span data-stu-id="52d9c-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="52d9c-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="52d9c-110">**allowTextEntry**</span></span> | <span data-ttu-id="52d9c-111">boolean</span><span class="sxs-lookup"><span data-stu-id="52d9c-111">boolean</span></span>            | <span data-ttu-id="52d9c-112">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="52d9c-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="52d9c-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="52d9c-113">**choices**</span></span>        | <span data-ttu-id="52d9c-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="52d9c-114">collection(string)</span></span> | <span data-ttu-id="52d9c-115">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="52d9c-115">The list of values available for this column.</span></span>
| <span data-ttu-id="52d9c-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="52d9c-116">**displayAs**</span></span>      | <span data-ttu-id="52d9c-117">string</span><span class="sxs-lookup"><span data-stu-id="52d9c-117">string</span></span>             | <span data-ttu-id="52d9c-118">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="52d9c-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="52d9c-119">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="52d9c-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


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
