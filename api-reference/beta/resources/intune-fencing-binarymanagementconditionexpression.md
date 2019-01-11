---
title: binaryManagementConditionExpression リソースの種類
description: 二項演算を使用して評価される管理条件式です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 509e03e7d492289fc9615f7f8ad47bf13d5bead4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27857051"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="3b061-103">binaryManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b061-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="3b061-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b061-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3b061-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b061-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b061-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b061-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b061-107">二項演算を使用して評価される管理条件式です。</span><span class="sxs-lookup"><span data-stu-id="3b061-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="3b061-108">[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3b061-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b061-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b061-109">Properties</span></span>
|<span data-ttu-id="3b061-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b061-110">Property</span></span>|<span data-ttu-id="3b061-111">種類</span><span class="sxs-lookup"><span data-stu-id="3b061-111">Type</span></span>|<span data-ttu-id="3b061-112">説明</span><span class="sxs-lookup"><span data-stu-id="3b061-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b061-113">operator</span><span class="sxs-lookup"><span data-stu-id="3b061-113">operator</span></span>|[<span data-ttu-id="3b061-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="3b061-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="3b061-115">二項演算の評価に使用する演算子です。</span><span class="sxs-lookup"><span data-stu-id="3b061-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="3b061-116">使用可能な値は、`or`、`and` です。</span><span class="sxs-lookup"><span data-stu-id="3b061-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="3b061-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="3b061-117">firstOperand</span></span>|[<span data-ttu-id="3b061-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="3b061-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="3b061-119">二項演算の 1 番目のオペランド。</span><span class="sxs-lookup"><span data-stu-id="3b061-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="3b061-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="3b061-120">secondOperand</span></span>|[<span data-ttu-id="3b061-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="3b061-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="3b061-122">二項演算の 2 番目のオペランド。</span><span class="sxs-lookup"><span data-stu-id="3b061-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b061-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b061-123">Relationships</span></span>
<span data-ttu-id="3b061-124">なし</span><span class="sxs-lookup"><span data-stu-id="3b061-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3b061-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b061-125">JSON Representation</span></span>
<span data-ttu-id="3b061-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3b061-126">Here is a JSON representation of the resource.</span></span>
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





