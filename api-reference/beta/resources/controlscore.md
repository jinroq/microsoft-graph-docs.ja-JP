---
title: " controlscore リソースの種類"
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
ms.openlocfilehash: 34e94128ff3993a01d37770bea1ad046f936405f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341184"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="f3963-103">controlscore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3963-103">controlScore resource type</span></span>

<span data-ttu-id="f3963-104">このリソースには、各コントロールのテナントのスコアと説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3963-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="f3963-105">名前</span><span class="sxs-lookup"><span data-stu-id="f3963-105">Name</span></span> |<span data-ttu-id="f3963-106">型</span><span class="sxs-lookup"><span data-stu-id="f3963-106">Type</span></span> |<span data-ttu-id="f3963-107">説明</span><span class="sxs-lookup"><span data-stu-id="f3963-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="f3963-108">controlName</span><span class="sxs-lookup"><span data-stu-id="f3963-108">controlName</span></span> |   <span data-ttu-id="f3963-109">String</span><span class="sxs-lookup"><span data-stu-id="f3963-109">String</span></span>  |   <span data-ttu-id="f3963-110">コントロールの一意の名前</span><span class="sxs-lookup"><span data-stu-id="f3963-110">Control unique name</span></span> |
|   <span data-ttu-id="f3963-111">score</span><span class="sxs-lookup"><span data-stu-id="f3963-111">score</span></span>   |   <span data-ttu-id="f3963-112">2 行分</span><span class="sxs-lookup"><span data-stu-id="f3963-112">Double</span></span>  |  <span data-ttu-id="f3963-113">コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。</span><span class="sxs-lookup"><span data-stu-id="f3963-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="f3963-114">controlcategory</span><span class="sxs-lookup"><span data-stu-id="f3963-114">controlCategory</span></span> |   <span data-ttu-id="f3963-115">String</span><span class="sxs-lookup"><span data-stu-id="f3963-115">String</span></span>  |  <span data-ttu-id="f3963-116">コントロールアクションカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="f3963-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="f3963-117">description</span><span class="sxs-lookup"><span data-stu-id="f3963-117">description</span></span> |   <span data-ttu-id="f3963-118">String</span><span class="sxs-lookup"><span data-stu-id="f3963-118">String</span></span>  |  <span data-ttu-id="f3963-119">コントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="f3963-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f3963-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3963-120">JSON representation</span></span>

<span data-ttu-id="f3963-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f3963-121">The following is a JSON representation of the resource.</span></span>

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
