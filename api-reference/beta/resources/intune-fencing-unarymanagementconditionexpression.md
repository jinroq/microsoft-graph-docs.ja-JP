---
title: 非 Arymanagementconditionexpression リソースの種類
description: 単項演算を使用して評価される管理条件式。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 155386e63a5d1f28a3cbe0ed35b9c5f659389bc6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36011065"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="7499e-103">非 Arymanagementconditionexpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7499e-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="7499e-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7499e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7499e-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7499e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7499e-106">単項演算を使用して評価される管理条件式。</span><span class="sxs-lookup"><span data-stu-id="7499e-106">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="7499e-107">[Managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="7499e-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7499e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7499e-108">Properties</span></span>
|<span data-ttu-id="7499e-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7499e-109">Property</span></span>|<span data-ttu-id="7499e-110">型</span><span class="sxs-lookup"><span data-stu-id="7499e-110">Type</span></span>|<span data-ttu-id="7499e-111">説明</span><span class="sxs-lookup"><span data-stu-id="7499e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7499e-112">operator</span><span class="sxs-lookup"><span data-stu-id="7499e-112">operator</span></span>|[<span data-ttu-id="7499e-113">非 Arymanagementconditionexpression 演算子の種類</span><span class="sxs-lookup"><span data-stu-id="7499e-113">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="7499e-114">単項演算の評価に使用する演算子。</span><span class="sxs-lookup"><span data-stu-id="7499e-114">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="7499e-115">可能な値は`not`次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="7499e-115">Possible values are: `not`.</span></span>|
|<span data-ttu-id="7499e-116">左辺</span><span class="sxs-lookup"><span data-stu-id="7499e-116">operand</span></span>|[<span data-ttu-id="7499e-117">Managementconditionexpression モデル</span><span class="sxs-lookup"><span data-stu-id="7499e-117">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="7499e-118">単項演算のオペランド。</span><span class="sxs-lookup"><span data-stu-id="7499e-118">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7499e-119">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7499e-119">Relationships</span></span>
<span data-ttu-id="7499e-120">なし</span><span class="sxs-lookup"><span data-stu-id="7499e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7499e-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7499e-121">JSON Representation</span></span>
<span data-ttu-id="7499e-122">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7499e-122">Here is a JSON representation of the resource.</span></span>
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





