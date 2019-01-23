---
title: binaryManagementConditionExpression リソースの種類
description: 二項演算を使用して評価される管理条件式です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 722387492e6167c3bd74d306fa03e4835bc12dbe
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402728"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="84321-103">binaryManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="84321-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="84321-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84321-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84321-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84321-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84321-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="84321-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84321-107">二項演算を使用して評価される管理条件式です。</span><span class="sxs-lookup"><span data-stu-id="84321-107">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="84321-108">[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="84321-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="84321-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84321-109">Properties</span></span>
|<span data-ttu-id="84321-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="84321-110">Property</span></span>|<span data-ttu-id="84321-111">型</span><span class="sxs-lookup"><span data-stu-id="84321-111">Type</span></span>|<span data-ttu-id="84321-112">説明</span><span class="sxs-lookup"><span data-stu-id="84321-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84321-113">operator</span><span class="sxs-lookup"><span data-stu-id="84321-113">operator</span></span>|[<span data-ttu-id="84321-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="84321-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="84321-115">二項演算の評価に使用する演算子です。</span><span class="sxs-lookup"><span data-stu-id="84321-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="84321-116">使用可能な値は、`or`、`and` です。</span><span class="sxs-lookup"><span data-stu-id="84321-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="84321-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="84321-117">firstOperand</span></span>|[<span data-ttu-id="84321-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="84321-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="84321-119">二項演算の 1 番目のオペランド。</span><span class="sxs-lookup"><span data-stu-id="84321-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="84321-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="84321-120">secondOperand</span></span>|[<span data-ttu-id="84321-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="84321-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="84321-122">二項演算の 2 番目のオペランド。</span><span class="sxs-lookup"><span data-stu-id="84321-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84321-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="84321-123">Relationships</span></span>
<span data-ttu-id="84321-124">なし</span><span class="sxs-lookup"><span data-stu-id="84321-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84321-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="84321-125">JSON Representation</span></span>
<span data-ttu-id="84321-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="84321-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.binaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.binaryManagementConditionExpression",
  "operator": "String",
  "firstOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  },
  "secondOperand": {
    "@odata.type": "microsoft.graph.managementConditionExpressionModel"
  }
}
```




