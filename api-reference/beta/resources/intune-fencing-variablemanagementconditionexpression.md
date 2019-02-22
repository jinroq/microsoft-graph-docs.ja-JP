---
title: variableManagementConditionExpression リソースの種類
description: 管理条件の状態をブール式として評価します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fab070cc9d2c51fbe1dc4b33c82fb823a849b7cc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168230"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="41060-103">variableManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41060-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="41060-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41060-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41060-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="41060-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41060-106">管理条件の状態をブール式として評価します。</span><span class="sxs-lookup"><span data-stu-id="41060-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="41060-107">[managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="41060-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="41060-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41060-108">Properties</span></span>
|<span data-ttu-id="41060-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41060-109">Property</span></span>|<span data-ttu-id="41060-110">型</span><span class="sxs-lookup"><span data-stu-id="41060-110">Type</span></span>|<span data-ttu-id="41060-111">説明</span><span class="sxs-lookup"><span data-stu-id="41060-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="41060-112">managementconditionid</span><span class="sxs-lookup"><span data-stu-id="41060-112">managementConditionId</span></span>|<span data-ttu-id="41060-113">String</span><span class="sxs-lookup"><span data-stu-id="41060-113">String</span></span>|<span data-ttu-id="41060-114">式の評価に使用される管理条件 id。</span><span class="sxs-lookup"><span data-stu-id="41060-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="41060-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="41060-115">Relationships</span></span>
<span data-ttu-id="41060-116">なし</span><span class="sxs-lookup"><span data-stu-id="41060-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="41060-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41060-117">JSON Representation</span></span>
<span data-ttu-id="41060-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="41060-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.variableManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.variableManagementConditionExpression",
  "managementConditionId": "String"
}
```




