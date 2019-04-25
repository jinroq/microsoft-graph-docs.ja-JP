---
title: variableManagementConditionExpression リソースの種類
description: 管理条件の状態をブール式として評価します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 548c0ffd27f76dacf5f88d9e783ce793e64cc434
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552890"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="d1237-103">variableManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1237-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="d1237-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1237-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1237-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d1237-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1237-106">管理条件の状態をブール式として評価します。</span><span class="sxs-lookup"><span data-stu-id="d1237-106">Evaluates the management condition state as a Boolean expression.</span></span>


<span data-ttu-id="d1237-107">[managementconditionexpression モデル](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="d1237-107">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1237-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1237-108">Properties</span></span>
|<span data-ttu-id="d1237-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1237-109">Property</span></span>|<span data-ttu-id="d1237-110">型</span><span class="sxs-lookup"><span data-stu-id="d1237-110">Type</span></span>|<span data-ttu-id="d1237-111">説明</span><span class="sxs-lookup"><span data-stu-id="d1237-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1237-112">managementconditionid</span><span class="sxs-lookup"><span data-stu-id="d1237-112">managementConditionId</span></span>|<span data-ttu-id="d1237-113">String</span><span class="sxs-lookup"><span data-stu-id="d1237-113">String</span></span>|<span data-ttu-id="d1237-114">式の評価に使用される管理条件 id。</span><span class="sxs-lookup"><span data-stu-id="d1237-114">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1237-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1237-115">Relationships</span></span>
<span data-ttu-id="d1237-116">なし</span><span class="sxs-lookup"><span data-stu-id="d1237-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1237-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1237-117">JSON Representation</span></span>
<span data-ttu-id="d1237-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1237-118">Here is a JSON representation of the resource.</span></span>
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





