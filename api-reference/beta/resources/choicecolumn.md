---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: ChoiceColumn
localization_priority: Normal
ms.openlocfilehash: 2e0798f558ace72f59a6acccc0cc8ce3eb6e2291
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27842547"
---
# <a name="choicecolumn-resource-type"></a><span data-ttu-id="646d0-102">ChoiceColumn リソースの種類</span><span class="sxs-lookup"><span data-stu-id="646d0-102">ChoiceColumn resource type</span></span>

> <span data-ttu-id="646d0-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="646d0-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="646d0-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="646d0-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="646d0-105">[columnDefinition ](columndefinition.md)リソースの\*\* choiceColumn \*\*は、選択肢のリストから列の値を選択できることを示します。</span><span class="sxs-lookup"><span data-stu-id="646d0-105">The **choiceColumn** on a [columnDefinition](columndefinition.md) resource indicates that the column's values can be selected from a list of choices.</span></span>

## <a name="json-representation"></a><span data-ttu-id="646d0-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="646d0-106">JSON representation</span></span>

<span data-ttu-id="646d0-107">以下は、**choiceColumn** リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="646d0-107">Here is a JSON representation of a **choiceColumn** resource.</span></span>
<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.choiceColumn" } -->

```json
{
  "allowTextEntry": true,
  "choices": ["red", "blue", "green"],
  "displayAs": "checkBoxes | dropDownMenu | radioButtons"
}
```

## <a name="properties"></a><span data-ttu-id="646d0-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="646d0-108">Properties</span></span>

| <span data-ttu-id="646d0-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="646d0-109">Property name</span></span>      | <span data-ttu-id="646d0-110">Type</span><span class="sxs-lookup"><span data-stu-id="646d0-110">Type</span></span>               | <span data-ttu-id="646d0-111">説明</span><span class="sxs-lookup"><span data-stu-id="646d0-111">Description</span></span>
|:-------------------|:-------------------|:----------------------------------------------
| <span data-ttu-id="646d0-112">**allowTextEntry**</span><span class="sxs-lookup"><span data-stu-id="646d0-112">**allowTextEntry**</span></span> | <span data-ttu-id="646d0-113">boolean</span><span class="sxs-lookup"><span data-stu-id="646d0-113">boolean</span></span>            | <span data-ttu-id="646d0-114">true の場合、設定された選択肢にないカスタム値を使用できます。</span><span class="sxs-lookup"><span data-stu-id="646d0-114">If true, allows custom values that aren't in the configured choices.</span></span>
| <span data-ttu-id="646d0-115">**choices**</span><span class="sxs-lookup"><span data-stu-id="646d0-115">**choices**</span></span>        | <span data-ttu-id="646d0-116">collection(string)</span><span class="sxs-lookup"><span data-stu-id="646d0-116">collection(string)</span></span> | <span data-ttu-id="646d0-117">この列に使用可能な値のリスト。</span><span class="sxs-lookup"><span data-stu-id="646d0-117">The list of values available for this column.</span></span>
| <span data-ttu-id="646d0-118">**displayAs**</span><span class="sxs-lookup"><span data-stu-id="646d0-118">**displayAs**</span></span>      | <span data-ttu-id="646d0-119">文字列</span><span class="sxs-lookup"><span data-stu-id="646d0-119">string</span></span>             | <span data-ttu-id="646d0-120">UX での選択肢の表示方法。</span><span class="sxs-lookup"><span data-stu-id="646d0-120">How the choices are to be presented in the UX.</span></span> <span data-ttu-id="646d0-121">`checkBoxes`、`dropDownMenu`、`radioButtons` のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="646d0-121">Must be one of `checkBoxes`, `dropDownMenu`, or `radioButtons`</span></span>


<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/ChoiceColumn"
} -->
