---
title: unaryManagementConditionExpression リソースの種類
description: 単項演算を使用して評価される管理条件式です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f1224a869ec2ec9cae2f38273f7a68b64d3d7333
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406781"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="82064-103">unaryManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="82064-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="82064-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="82064-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="82064-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82064-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82064-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82064-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82064-107">単項演算を使用して評価される管理条件式です。</span><span class="sxs-lookup"><span data-stu-id="82064-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="82064-108">[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="82064-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="82064-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82064-109">Properties</span></span>
|<span data-ttu-id="82064-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82064-110">Property</span></span>|<span data-ttu-id="82064-111">型</span><span class="sxs-lookup"><span data-stu-id="82064-111">Type</span></span>|<span data-ttu-id="82064-112">説明</span><span class="sxs-lookup"><span data-stu-id="82064-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82064-113">operator</span><span class="sxs-lookup"><span data-stu-id="82064-113">operator</span></span>|[<span data-ttu-id="82064-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="82064-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="82064-115">単項演算の評価に使用する演算子です。</span><span class="sxs-lookup"><span data-stu-id="82064-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="82064-116">使用可能な値: `not`。</span><span class="sxs-lookup"><span data-stu-id="82064-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="82064-117">オペランド</span><span class="sxs-lookup"><span data-stu-id="82064-117">operand</span></span>|[<span data-ttu-id="82064-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="82064-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="82064-119">単項演算のオペランドです。</span><span class="sxs-lookup"><span data-stu-id="82064-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82064-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82064-120">Relationships</span></span>
<span data-ttu-id="82064-121">なし</span><span class="sxs-lookup"><span data-stu-id="82064-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="82064-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82064-122">JSON Representation</span></span>
<span data-ttu-id="82064-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82064-123">Here is a JSON representation of the resource.</span></span>
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




