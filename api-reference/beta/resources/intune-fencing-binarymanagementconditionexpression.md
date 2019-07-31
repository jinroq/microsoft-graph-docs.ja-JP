---
title: binaryManagementConditionExpression リソースの種類
description: バイナリ演算を使用して評価される管理条件式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f4782fb9fc7f1af9110622d9714c6f67e59bd89e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011135"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="3457e-103">binaryManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3457e-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="3457e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3457e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3457e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3457e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3457e-106">バイナリ演算を使用して評価される管理条件式。</span><span class="sxs-lookup"><span data-stu-id="3457e-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="3457e-107">[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="3457e-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3457e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3457e-108">Properties</span></span>
|<span data-ttu-id="3457e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3457e-109">Property</span></span>|<span data-ttu-id="3457e-110">型</span><span class="sxs-lookup"><span data-stu-id="3457e-110">Type</span></span>|<span data-ttu-id="3457e-111">説明</span><span class="sxs-lookup"><span data-stu-id="3457e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3457e-112">operator</span><span class="sxs-lookup"><span data-stu-id="3457e-112">operator</span></span>|[<span data-ttu-id="3457e-113">Binarymanagementconditionexpression 演算子の種類</span><span class="sxs-lookup"><span data-stu-id="3457e-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="3457e-114">二項演算の評価で使用される演算子です。</span><span class="sxs-lookup"><span data-stu-id="3457e-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="3457e-115">可能な値は、`or`、`and` です。</span><span class="sxs-lookup"><span data-stu-id="3457e-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="3457e-116">firstOperand</span><span class="sxs-lookup"><span data-stu-id="3457e-116">firstOperand</span></span>|[<span data-ttu-id="3457e-117">Managementconditionexpression モデル</span><span class="sxs-lookup"><span data-stu-id="3457e-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="3457e-118">二項演算の最初のオペランド。</span><span class="sxs-lookup"><span data-stu-id="3457e-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="3457e-119">この</span><span class="sxs-lookup"><span data-stu-id="3457e-119">secondOperand</span></span>|[<span data-ttu-id="3457e-120">Managementconditionexpression モデル</span><span class="sxs-lookup"><span data-stu-id="3457e-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="3457e-121">二項演算の2番目のオペランド。</span><span class="sxs-lookup"><span data-stu-id="3457e-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3457e-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3457e-122">Relationships</span></span>
<span data-ttu-id="3457e-123">なし</span><span class="sxs-lookup"><span data-stu-id="3457e-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3457e-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3457e-124">JSON Representation</span></span>
<span data-ttu-id="3457e-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3457e-125">Here is a JSON representation of the resource.</span></span>
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





