---
title: " controlscore リソースの種類"
description: このリソースには、各コントロールのテナントのスコアと説明が含まれています。
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543379"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="6cdbf-103">controlscore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6cdbf-103">controlScore resource type</span></span>

<span data-ttu-id="6cdbf-104">このリソースには、各コントロールのテナントのスコアと説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6cdbf-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="6cdbf-105">名前</span><span class="sxs-lookup"><span data-stu-id="6cdbf-105">Name</span></span> |<span data-ttu-id="6cdbf-106">型</span><span class="sxs-lookup"><span data-stu-id="6cdbf-106">Type</span></span> |<span data-ttu-id="6cdbf-107">説明</span><span class="sxs-lookup"><span data-stu-id="6cdbf-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="6cdbf-108">controlName</span><span class="sxs-lookup"><span data-stu-id="6cdbf-108">controlName</span></span> |   <span data-ttu-id="6cdbf-109">String</span><span class="sxs-lookup"><span data-stu-id="6cdbf-109">String</span></span>  |   <span data-ttu-id="6cdbf-110">コントロールの一意の名前</span><span class="sxs-lookup"><span data-stu-id="6cdbf-110">Control unique name</span></span> |
|   <span data-ttu-id="6cdbf-111">score</span><span class="sxs-lookup"><span data-stu-id="6cdbf-111">score</span></span>   |   <span data-ttu-id="6cdbf-112">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="6cdbf-112">Double</span></span>  |  <span data-ttu-id="6cdbf-113">コントロールのテナントが獲得したスコア (コントロールのテナント操作に応じて日によって日付が変化します)。</span><span class="sxs-lookup"><span data-stu-id="6cdbf-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="6cdbf-114">controlcategory</span><span class="sxs-lookup"><span data-stu-id="6cdbf-114">controlCategory</span></span> |   <span data-ttu-id="6cdbf-115">String</span><span class="sxs-lookup"><span data-stu-id="6cdbf-115">String</span></span>  |  <span data-ttu-id="6cdbf-116">コントロールアクションカテゴリ (id、データ、デバイス、アプリ、インフラストラクチャ)。</span><span class="sxs-lookup"><span data-stu-id="6cdbf-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="6cdbf-117">description</span><span class="sxs-lookup"><span data-stu-id="6cdbf-117">description</span></span> |   <span data-ttu-id="6cdbf-118">String</span><span class="sxs-lookup"><span data-stu-id="6cdbf-118">String</span></span>  |  <span data-ttu-id="6cdbf-119">コントロールの説明。</span><span class="sxs-lookup"><span data-stu-id="6cdbf-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="6cdbf-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6cdbf-120">JSON representation</span></span>

<span data-ttu-id="6cdbf-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6cdbf-121">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.controlScore"
}-->

```json
{
  "controlName": "String",
  "score": "String",
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
