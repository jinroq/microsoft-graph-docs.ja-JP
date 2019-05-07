---
title: controlScore リソースの種類
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
author: preetikr
ms.openlocfilehash: 64b5377fce01273ab31d7ec293f5dc7a6e1342ff
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629286"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="0c420-103">controlScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c420-103">controlScore resource type</span></span>

<span data-ttu-id="0c420-104">各コントロールのテナントのスコアと説明が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0c420-104">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="0c420-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c420-105">Properties</span></span>

|<span data-ttu-id="0c420-106">名前</span><span class="sxs-lookup"><span data-stu-id="0c420-106">Name</span></span> |<span data-ttu-id="0c420-107">型</span><span class="sxs-lookup"><span data-stu-id="0c420-107">Type</span></span> |<span data-ttu-id="0c420-108">説明</span><span class="sxs-lookup"><span data-stu-id="0c420-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="0c420-109">controlName</span><span class="sxs-lookup"><span data-stu-id="0c420-109">controlName</span></span>|<span data-ttu-id="0c420-110">String</span><span class="sxs-lookup"><span data-stu-id="0c420-110">String</span></span>|<span data-ttu-id="0c420-111">一意の名前を制御します。</span><span class="sxs-lookup"><span data-stu-id="0c420-111">Control unique name.</span></span>|
|<span data-ttu-id="0c420-112">score</span><span class="sxs-lookup"><span data-stu-id="0c420-112">score</span></span>|<span data-ttu-id="0c420-113">2 行分</span><span class="sxs-lookup"><span data-stu-id="0c420-113">Double</span></span>|<span data-ttu-id="0c420-114">コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。</span><span class="sxs-lookup"><span data-stu-id="0c420-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="0c420-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="0c420-115">controlCategory</span></span>|<span data-ttu-id="0c420-116">String</span><span class="sxs-lookup"><span data-stu-id="0c420-116">String</span></span>|<span data-ttu-id="0c420-117">コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="0c420-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="0c420-118">説明</span><span class="sxs-lookup"><span data-stu-id="0c420-118">description</span></span>|<span data-ttu-id="0c420-119">String</span><span class="sxs-lookup"><span data-stu-id="0c420-119">String</span></span>| <span data-ttu-id="0c420-120">コントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="0c420-120">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0c420-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c420-121">JSON representation</span></span>

<span data-ttu-id="0c420-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0c420-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "Double",
  "controlCategory": "String",
  "description": "String"
}

```


<!-- {
  "type": "#page.annotation",
  "description": "controlScore resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
