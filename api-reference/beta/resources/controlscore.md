---
title: " controlScore リソースの種類"
description: このリソースには、テナントのスコアと個々 のコントロールの説明が含まれています。
ms.openlocfilehash: 67059c1a7382416411709f02c609c90b20a673b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067808"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="ba0e6-103">controlScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba0e6-103">controlScore resource type</span></span>

<span data-ttu-id="ba0e6-104">このリソースには、テナントのスコアと個々 のコントロールの説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ba0e6-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="ba0e6-105">名前</span><span class="sxs-lookup"><span data-stu-id="ba0e6-105">Name</span></span> |<span data-ttu-id="ba0e6-106">型</span><span class="sxs-lookup"><span data-stu-id="ba0e6-106">Type</span></span> |<span data-ttu-id="ba0e6-107">説明</span><span class="sxs-lookup"><span data-stu-id="ba0e6-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="ba0e6-108">controlName</span><span class="sxs-lookup"><span data-stu-id="ba0e6-108">controlName</span></span> |   <span data-ttu-id="ba0e6-109">String</span><span class="sxs-lookup"><span data-stu-id="ba0e6-109">String</span></span>  |   <span data-ttu-id="ba0e6-110">コントロールの一意の名前</span><span class="sxs-lookup"><span data-stu-id="ba0e6-110">Control unique name</span></span> |
|   <span data-ttu-id="ba0e6-111">score</span><span class="sxs-lookup"><span data-stu-id="ba0e6-111">score</span></span>   |   <span data-ttu-id="ba0e6-112">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="ba0e6-112">Double</span></span>  |  <span data-ttu-id="ba0e6-113">テナントは、コントロールの (日単位によって異なりますコントロール上のテナントの操作) のスコアを達成しました。</span><span class="sxs-lookup"><span data-stu-id="ba0e6-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="ba0e6-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="ba0e6-114">controlCategory</span></span> |   <span data-ttu-id="ba0e6-115">String</span><span class="sxs-lookup"><span data-stu-id="ba0e6-115">String</span></span>  |  <span data-ttu-id="ba0e6-116">コントロールのアクションのカテゴリ (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) です。</span><span class="sxs-lookup"><span data-stu-id="ba0e6-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="ba0e6-117">説明</span><span class="sxs-lookup"><span data-stu-id="ba0e6-117">description</span></span> |   <span data-ttu-id="ba0e6-118">String</span><span class="sxs-lookup"><span data-stu-id="ba0e6-118">String</span></span>  |  <span data-ttu-id="ba0e6-119">コントロールの説明です。</span><span class="sxs-lookup"><span data-stu-id="ba0e6-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ba0e6-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba0e6-120">JSON representation</span></span>

<span data-ttu-id="ba0e6-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ba0e6-121">The following is a JSON representation of the resource.</span></span>

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
