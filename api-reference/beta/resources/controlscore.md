---
title: " controlScore リソースの種類"
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 89e448d828f1f7caef73b14586b06d1df238f100
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973934"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="bb078-103">controlScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb078-103">controlScore resource type</span></span>

<span data-ttu-id="bb078-104">このリソースには、各コントロールのテナントのスコアと説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb078-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="bb078-105">名前</span><span class="sxs-lookup"><span data-stu-id="bb078-105">Name</span></span> |<span data-ttu-id="bb078-106">型</span><span class="sxs-lookup"><span data-stu-id="bb078-106">Type</span></span> |<span data-ttu-id="bb078-107">説明</span><span class="sxs-lookup"><span data-stu-id="bb078-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="bb078-108">controlName</span><span class="sxs-lookup"><span data-stu-id="bb078-108">controlName</span></span> |   <span data-ttu-id="bb078-109">String</span><span class="sxs-lookup"><span data-stu-id="bb078-109">String</span></span>  |   <span data-ttu-id="bb078-110">コントロールの一意の名前</span><span class="sxs-lookup"><span data-stu-id="bb078-110">Control unique name</span></span> |
|   <span data-ttu-id="bb078-111">score</span><span class="sxs-lookup"><span data-stu-id="bb078-111">score</span></span>   |   <span data-ttu-id="bb078-112">2 行分</span><span class="sxs-lookup"><span data-stu-id="bb078-112">Double</span></span>  |  <span data-ttu-id="bb078-113">コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。</span><span class="sxs-lookup"><span data-stu-id="bb078-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="bb078-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="bb078-114">controlCategory</span></span> |   <span data-ttu-id="bb078-115">String</span><span class="sxs-lookup"><span data-stu-id="bb078-115">String</span></span>  |  <span data-ttu-id="bb078-116">コントロールアクションカテゴリ (Id、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="bb078-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="bb078-117">description</span><span class="sxs-lookup"><span data-stu-id="bb078-117">description</span></span> |   <span data-ttu-id="bb078-118">String</span><span class="sxs-lookup"><span data-stu-id="bb078-118">String</span></span>  |  <span data-ttu-id="bb078-119">コントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="bb078-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="bb078-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb078-120">JSON representation</span></span>

<span data-ttu-id="bb078-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bb078-121">The following is a JSON representation of the resource.</span></span>

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
