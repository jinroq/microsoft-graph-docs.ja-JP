---
title: " controlScore リソースの種類"
description: このリソースには、テナントのスコアと個々 のコントロールの説明が含まれています。
localization_priority: Normal
ms.openlocfilehash: d8c2d73205f00a9dd5f2f28fcee3c33778bb3276
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891470"
---
#  <a name="controlscore-resource-type"></a><span data-ttu-id="065b0-103">controlScore リソースの種類</span><span class="sxs-lookup"><span data-stu-id="065b0-103">controlScore resource type</span></span>

<span data-ttu-id="065b0-104">このリソースには、テナントのスコアと個々 のコントロールの説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="065b0-104">This resource contains a tenant score and description for an individual control.</span></span>

|<span data-ttu-id="065b0-105">名前</span><span class="sxs-lookup"><span data-stu-id="065b0-105">Name</span></span> |<span data-ttu-id="065b0-106">種類</span><span class="sxs-lookup"><span data-stu-id="065b0-106">Type</span></span> |<span data-ttu-id="065b0-107">説明</span><span class="sxs-lookup"><span data-stu-id="065b0-107">Description</span></span> |
|:--|:--|:--|
|   <span data-ttu-id="065b0-108">controlName</span><span class="sxs-lookup"><span data-stu-id="065b0-108">controlName</span></span> |   <span data-ttu-id="065b0-109">String</span><span class="sxs-lookup"><span data-stu-id="065b0-109">String</span></span>  |   <span data-ttu-id="065b0-110">コントロールの一意の名前</span><span class="sxs-lookup"><span data-stu-id="065b0-110">Control unique name</span></span> |
|   <span data-ttu-id="065b0-111">score</span><span class="sxs-lookup"><span data-stu-id="065b0-111">score</span></span>   |   <span data-ttu-id="065b0-112">倍精度浮動小数点数</span><span class="sxs-lookup"><span data-stu-id="065b0-112">Double</span></span>  |  <span data-ttu-id="065b0-113">テナントは、コントロールの (日単位によって異なりますコントロール上のテナントの操作) のスコアを達成しました。</span><span class="sxs-lookup"><span data-stu-id="065b0-113">Tenant achieved score for the control (it varies day by day depending on tenant operations on the control).</span></span> |
|   <span data-ttu-id="065b0-114">controlCategory</span><span class="sxs-lookup"><span data-stu-id="065b0-114">controlCategory</span></span> |   <span data-ttu-id="065b0-115">String</span><span class="sxs-lookup"><span data-stu-id="065b0-115">String</span></span>  |  <span data-ttu-id="065b0-116">コントロールのアクションのカテゴリ (識別情報、データ、デバイス、アプリケーション、インフラストラクチャ) です。</span><span class="sxs-lookup"><span data-stu-id="065b0-116">Control action category (Identity, Data, Device, Apps, Infrastructure).</span></span> |
|   <span data-ttu-id="065b0-117">説明</span><span class="sxs-lookup"><span data-stu-id="065b0-117">description</span></span> |   <span data-ttu-id="065b0-118">String</span><span class="sxs-lookup"><span data-stu-id="065b0-118">String</span></span>  |  <span data-ttu-id="065b0-119">コントロールの説明です。</span><span class="sxs-lookup"><span data-stu-id="065b0-119">Description of the control.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="065b0-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="065b0-120">JSON representation</span></span>

<span data-ttu-id="065b0-121">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="065b0-121">The following is a JSON representation of the resource.</span></span>

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
