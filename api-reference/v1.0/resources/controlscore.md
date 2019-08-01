---
title: controlScore リソースの種類
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 68e4bf278b7d1b6ea6f00f75192847abab1ae3a4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032845"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="f7c0c-103">controlScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7c0c-103">controlScore resource type</span></span>

<span data-ttu-id="f7c0c-104">各コントロールのテナントのスコアと説明が含まれます。</span><span class="sxs-lookup"><span data-stu-id="f7c0c-104">Contains a tenant score and description for an individual control.</span></span>

## <a name="properties"></a><span data-ttu-id="f7c0c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c0c-105">Properties</span></span>

|<span data-ttu-id="f7c0c-106">名前</span><span class="sxs-lookup"><span data-stu-id="f7c0c-106">Name</span></span> |<span data-ttu-id="f7c0c-107">型</span><span class="sxs-lookup"><span data-stu-id="f7c0c-107">Type</span></span> |<span data-ttu-id="f7c0c-108">説明</span><span class="sxs-lookup"><span data-stu-id="f7c0c-108">Description</span></span> |
|:--|:--|:--|
|<span data-ttu-id="f7c0c-109">controlName</span><span class="sxs-lookup"><span data-stu-id="f7c0c-109">controlName</span></span>|<span data-ttu-id="f7c0c-110">String</span><span class="sxs-lookup"><span data-stu-id="f7c0c-110">String</span></span>|<span data-ttu-id="f7c0c-111">一意の名前を制御します。</span><span class="sxs-lookup"><span data-stu-id="f7c0c-111">Control unique name.</span></span>|
|<span data-ttu-id="f7c0c-112">score</span><span class="sxs-lookup"><span data-stu-id="f7c0c-112">score</span></span>|<span data-ttu-id="f7c0c-113">2 行分</span><span class="sxs-lookup"><span data-stu-id="f7c0c-113">Double</span></span>|<span data-ttu-id="f7c0c-114">コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。</span><span class="sxs-lookup"><span data-stu-id="f7c0c-114">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span>|
|<span data-ttu-id="f7c0c-115">controlCategory</span><span class="sxs-lookup"><span data-stu-id="f7c0c-115">controlCategory</span></span>|<span data-ttu-id="f7c0c-116">String</span><span class="sxs-lookup"><span data-stu-id="f7c0c-116">String</span></span>|<span data-ttu-id="f7c0c-117">コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="f7c0c-117">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span>|
|<span data-ttu-id="f7c0c-118">description</span><span class="sxs-lookup"><span data-stu-id="f7c0c-118">description</span></span>|<span data-ttu-id="f7c0c-119">String</span><span class="sxs-lookup"><span data-stu-id="f7c0c-119">String</span></span>| <span data-ttu-id="f7c0c-120">コントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="f7c0c-120">Description of the control.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f7c0c-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7c0c-121">JSON representation</span></span>

<span data-ttu-id="f7c0c-122">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f7c0c-122">The following is a JSON representation of the resource.</span></span>

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
