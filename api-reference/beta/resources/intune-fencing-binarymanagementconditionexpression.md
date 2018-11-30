---
title: binaryManagementConditionExpression リソースの種類
description: 二項演算を使用して評価される管理条件式です。
ms.openlocfilehash: e675a5696d545ba48fc676d1716ed49c7c0b7c65
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073448"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="2e830-103">binaryManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e830-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="2e830-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2e830-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e830-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e830-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e830-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e830-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e830-107">二項演算を使用して評価される管理条件式です。</span><span class="sxs-lookup"><span data-stu-id="2e830-107">A management condition expression that is evaluated using a binary operation.</span></span>

<span data-ttu-id="2e830-108">[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="2e830-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="2e830-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e830-109">Properties</span></span>
|<span data-ttu-id="2e830-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e830-110">Property</span></span>|<span data-ttu-id="2e830-111">型</span><span class="sxs-lookup"><span data-stu-id="2e830-111">Type</span></span>|<span data-ttu-id="2e830-112">説明</span><span class="sxs-lookup"><span data-stu-id="2e830-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e830-113">operator</span><span class="sxs-lookup"><span data-stu-id="2e830-113">operator</span></span>|[<span data-ttu-id="2e830-114">binaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="2e830-114">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="2e830-115">二項演算の評価に使用する演算子です。</span><span class="sxs-lookup"><span data-stu-id="2e830-115">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="2e830-116">使用可能な値は、`or`、`and` です。</span><span class="sxs-lookup"><span data-stu-id="2e830-116">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="2e830-117">firstOperand</span><span class="sxs-lookup"><span data-stu-id="2e830-117">firstOperand</span></span>|[<span data-ttu-id="2e830-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="2e830-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="2e830-119">二項演算の 1 番目のオペランド。</span><span class="sxs-lookup"><span data-stu-id="2e830-119">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="2e830-120">secondOperand</span><span class="sxs-lookup"><span data-stu-id="2e830-120">secondOperand</span></span>|[<span data-ttu-id="2e830-121">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="2e830-121">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="2e830-122">二項演算の 2 番目のオペランド。</span><span class="sxs-lookup"><span data-stu-id="2e830-122">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e830-123">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e830-123">Relationships</span></span>
<span data-ttu-id="2e830-124">なし</span><span class="sxs-lookup"><span data-stu-id="2e830-124">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2e830-125">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e830-125">JSON Representation</span></span>
<span data-ttu-id="2e830-126">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e830-126">Here is a JSON representation of the resource.</span></span>
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





