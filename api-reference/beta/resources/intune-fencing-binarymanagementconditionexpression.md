---
title: binaryManagementConditionExpression リソースの種類
description: バイナリ演算を使用して評価される管理条件式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 97c812c3a26af0401bbdea87997167bcada05a37
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994819"
---
# <a name="binarymanagementconditionexpression-resource-type"></a><span data-ttu-id="ec250-103">binaryManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ec250-103">binaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="ec250-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec250-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec250-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ec250-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec250-106">バイナリ演算を使用して評価される管理条件式。</span><span class="sxs-lookup"><span data-stu-id="ec250-106">A management condition expression that is evaluated using a binary operation.</span></span>


<span data-ttu-id="ec250-107">[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="ec250-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ec250-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec250-108">Properties</span></span>
|<span data-ttu-id="ec250-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec250-109">Property</span></span>|<span data-ttu-id="ec250-110">型</span><span class="sxs-lookup"><span data-stu-id="ec250-110">Type</span></span>|<span data-ttu-id="ec250-111">説明</span><span class="sxs-lookup"><span data-stu-id="ec250-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec250-112">operator</span><span class="sxs-lookup"><span data-stu-id="ec250-112">operator</span></span>|[<span data-ttu-id="ec250-113">Binarymanagementconditionexpression 演算子の種類</span><span class="sxs-lookup"><span data-stu-id="ec250-113">binaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-binarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="ec250-114">二項演算の評価で使用される演算子です。</span><span class="sxs-lookup"><span data-stu-id="ec250-114">The operator used in the evaluation of the binary operation.</span></span> <span data-ttu-id="ec250-115">可能な値は、`or`、`and` です。</span><span class="sxs-lookup"><span data-stu-id="ec250-115">Possible values are: `or`, `and`.</span></span>|
|<span data-ttu-id="ec250-116">firstOperand</span><span class="sxs-lookup"><span data-stu-id="ec250-116">firstOperand</span></span>|[<span data-ttu-id="ec250-117">Managementconditionexpression モデル</span><span class="sxs-lookup"><span data-stu-id="ec250-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="ec250-118">二項演算の最初のオペランド。</span><span class="sxs-lookup"><span data-stu-id="ec250-118">The first operand of the binary operation.</span></span>|
|<span data-ttu-id="ec250-119">この</span><span class="sxs-lookup"><span data-stu-id="ec250-119">secondOperand</span></span>|[<span data-ttu-id="ec250-120">Managementconditionexpression モデル</span><span class="sxs-lookup"><span data-stu-id="ec250-120">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="ec250-121">二項演算の2番目のオペランド。</span><span class="sxs-lookup"><span data-stu-id="ec250-121">The second operand of the binary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ec250-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ec250-122">Relationships</span></span>
<span data-ttu-id="ec250-123">なし</span><span class="sxs-lookup"><span data-stu-id="ec250-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ec250-124">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ec250-124">JSON Representation</span></span>
<span data-ttu-id="ec250-125">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ec250-125">Here is a JSON representation of the resource.</span></span>
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





