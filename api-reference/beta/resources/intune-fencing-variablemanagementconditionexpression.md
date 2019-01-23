---
title: variableManagementConditionExpression リソースの種類
description: 管理条件の状態は、ブール式として評価されます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6a5e7efd0c8213f40d1dfb5f86d2f86c999069d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399627"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="f25b6-103">variableManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f25b6-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="f25b6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f25b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f25b6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f25b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f25b6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f25b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f25b6-107">管理条件の状態は、ブール式として評価されます。</span><span class="sxs-lookup"><span data-stu-id="f25b6-107">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="f25b6-108">[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="f25b6-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f25b6-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f25b6-109">Properties</span></span>
|<span data-ttu-id="f25b6-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f25b6-110">Property</span></span>|<span data-ttu-id="f25b6-111">型</span><span class="sxs-lookup"><span data-stu-id="f25b6-111">Type</span></span>|<span data-ttu-id="f25b6-112">説明</span><span class="sxs-lookup"><span data-stu-id="f25b6-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f25b6-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="f25b6-113">managementConditionId</span></span>|<span data-ttu-id="f25b6-114">String</span><span class="sxs-lookup"><span data-stu-id="f25b6-114">String</span></span>|<span data-ttu-id="f25b6-115">式を評価するために使用される管理条件の id です。</span><span class="sxs-lookup"><span data-stu-id="f25b6-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f25b6-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f25b6-116">Relationships</span></span>
<span data-ttu-id="f25b6-117">なし</span><span class="sxs-lookup"><span data-stu-id="f25b6-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f25b6-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f25b6-118">JSON Representation</span></span>
<span data-ttu-id="f25b6-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f25b6-119">Here is a JSON representation of the resource.</span></span>
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




