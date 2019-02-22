---
title: 非 arymanagementconditionexpression リソースの種類
description: 単項演算を使用して評価される管理条件式。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9802cb8162973ecdaa387a29c70d1baa7aec4b8b
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164219"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="7e388-103">非 arymanagementconditionexpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e388-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="7e388-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e388-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e388-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e388-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e388-106">単項演算を使用して評価される管理条件式。</span><span class="sxs-lookup"><span data-stu-id="7e388-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="7e388-107">[managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="7e388-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e388-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e388-108">Properties</span></span>
|<span data-ttu-id="7e388-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e388-109">Property</span></span>|<span data-ttu-id="7e388-110">型</span><span class="sxs-lookup"><span data-stu-id="7e388-110">Type</span></span>|<span data-ttu-id="7e388-111">説明</span><span class="sxs-lookup"><span data-stu-id="7e388-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e388-112">operator</span><span class="sxs-lookup"><span data-stu-id="7e388-112">operator</span></span>|[<span data-ttu-id="7e388-113">非 arymanagementconditionexpression 演算子の種類</span><span class="sxs-lookup"><span data-stu-id="7e388-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="7e388-114">単項演算の評価に使用する演算子。</span><span class="sxs-lookup"><span data-stu-id="7e388-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="7e388-115">可能な値は`not`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="7e388-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="7e388-116">左辺</span><span class="sxs-lookup"><span data-stu-id="7e388-116">operand</span></span>|[<span data-ttu-id="7e388-117">managementconditionexpression モデル</span><span class="sxs-lookup"><span data-stu-id="7e388-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7e388-118">単項演算のオペランド。</span><span class="sxs-lookup"><span data-stu-id="7e388-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e388-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e388-119">Relationships</span></span>
<span data-ttu-id="7e388-120">なし</span><span class="sxs-lookup"><span data-stu-id="7e388-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e388-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e388-121">JSON Representation</span></span>
<span data-ttu-id="7e388-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e388-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```




