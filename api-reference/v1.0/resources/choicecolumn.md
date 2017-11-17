---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: c266550e8918603c3ee6104818c0aa721f1281d9
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="64de2-102">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64de2-102">ChoiceColumn resource type</span></span>

<span data-ttu-id="64de2-103">[columnDefinition](columnDefinition.md) リソースの **choiceColumn** は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="64de2-103">The **choiceColumn** on a [columnDefinition](columnDefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64de2-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64de2-104">JSON representation</span></span>

<span data-ttu-id="64de2-105">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64de2-105">Here is a JSON representation of a **driveItem** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="64de2-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64de2-106">Properties</span></span>

| <span data-ttu-id="64de2-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="64de2-107">Property name</span></span>      | <span data-ttu-id="64de2-108">種類</span><span class="sxs-lookup"><span data-stu-id="64de2-108">Type</span></span>               | <span data-ttu-id="64de2-109">説明</span><span class="sxs-lookup"><span data-stu-id="64de2-109">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="64de2-110">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="64de2-110">**allowTextEntry**</span></span> | <span data-ttu-id="64de2-111">boolean</span><span class="sxs-lookup"><span data-stu-id="64de2-111">boolean</span></span>            | <span data-ttu-id="64de2-112">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="64de2-112">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="64de2-113">**choices**</span><span class="sxs-lookup"><span data-stu-id="64de2-113">**CHOICES**</span></span>        | <span data-ttu-id="64de2-114">collection(string)</span><span class="sxs-lookup"><span data-stu-id="64de2-114">Collection(String)</span></span> | <span data-ttu-id="64de2-115">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="64de2-115">The list of values available for this column.</span></span>
| <span data-ttu-id="64de2-116">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="64de2-116">**displayAs**</span></span>      | <span data-ttu-id="64de2-117">string</span><span class="sxs-lookup"><span data-stu-id="64de2-117">string</span></span>             | <span data-ttu-id="64de2-118">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="64de2-118">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="64de2-119">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません</span><span class="sxs-lookup"><span data-stu-id="64de2-119">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
