---
author: JeremyKelley
description: columnDefinition リソースの choiceColumn は、選択肢のリストから列の値を選択できることを示します。
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 72ef8adb96614fc32b9aee8141eb19248e963639
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973501"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="90eb9-103">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90eb9-103">ChoiceColumn resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="90eb9-104">[columnDefinition ](columndefinition.md)リソースの\*\* choiceColumn \*\*は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="90eb9-104">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90eb9-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90eb9-105">JSON representation</span></span>

<span data-ttu-id="90eb9-106">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="90eb9-106">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="90eb9-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90eb9-107">Properties</span></span>

| <span data-ttu-id="90eb9-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="90eb9-108">Property name</span></span>      | <span data-ttu-id="90eb9-109">種類</span><span class="sxs-lookup"><span data-stu-id="90eb9-109">Type</span></span>               | <span data-ttu-id="90eb9-110">説明</span><span class="sxs-lookup"><span data-stu-id="90eb9-110">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="90eb9-111">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="90eb9-111">**allowTextEntry**</span></span> | <span data-ttu-id="90eb9-112">boolean</span><span class="sxs-lookup"><span data-stu-id="90eb9-112">boolean</span></span>            | <span data-ttu-id="90eb9-113">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="90eb9-113">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="90eb9-114">**choices**</span><span class="sxs-lookup"><span data-stu-id="90eb9-114">**choices**</span></span>        | <span data-ttu-id="90eb9-115">collection(string)</span><span class="sxs-lookup"><span data-stu-id="90eb9-115">collection(string)</span></span> | <span data-ttu-id="90eb9-116">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="90eb9-116">The list of values available for this column.</span></span>
| <span data-ttu-id="90eb9-117">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="90eb9-117">**displayAs**</span></span>      | <span data-ttu-id="90eb9-118">string</span><span class="sxs-lookup"><span data-stu-id="90eb9-118">string</span></span>             | <span data-ttu-id="90eb9-119">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="90eb9-119">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="90eb9-120">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="90eb9-120">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn",
  "suppressions": []
}
-->
