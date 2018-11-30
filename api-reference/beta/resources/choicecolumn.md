---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
ms.openlocfilehash: 659ece2eab255fe7b55a258b0980eda4e7bde5b2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066492"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="ba62b-102">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba62b-102">ChoiceColumn resource type</span></span>

> <span data-ttu-id="ba62b-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ba62b-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ba62b-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba62b-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ba62b-105">[columnDefinition ](columndefinition.md)リソースの\*\* choiceColumn \*\*は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="ba62b-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba62b-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba62b-106">JSON representation</span></span>

<span data-ttu-id="ba62b-107">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba62b-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="ba62b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba62b-108">Properties</span></span>

| <span data-ttu-id="ba62b-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ba62b-109">Property name</span></span>      | <span data-ttu-id="ba62b-110">型</span><span class="sxs-lookup"><span data-stu-id="ba62b-110">Type</span></span>               | <span data-ttu-id="ba62b-111">説明</span><span class="sxs-lookup"><span data-stu-id="ba62b-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="ba62b-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="ba62b-112">**allowTextEntry**</span></span> | <span data-ttu-id="ba62b-113">boolean</span><span class="sxs-lookup"><span data-stu-id="ba62b-113">boolean</span></span>            | <span data-ttu-id="ba62b-114">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="ba62b-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="ba62b-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="ba62b-115">**choices**</span></span>        | <span data-ttu-id="ba62b-116">collection(string)</span><span class="sxs-lookup"><span data-stu-id="ba62b-116">collection(string)</span></span> | <span data-ttu-id="ba62b-117">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="ba62b-117">The list of values available for this column.</span></span>
| <span data-ttu-id="ba62b-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="ba62b-118">**displayAs**</span></span>      | <span data-ttu-id="ba62b-119">文字列</span><span class="sxs-lookup"><span data-stu-id="ba62b-119">string</span></span>             | <span data-ttu-id="ba62b-120">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="ba62b-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="ba62b-121">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="ba62b-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
