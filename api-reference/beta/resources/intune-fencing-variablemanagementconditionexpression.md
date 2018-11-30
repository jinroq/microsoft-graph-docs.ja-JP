---
title: variableManagementConditionExpression リソースの種類
description: 管理条件の状態は、ブール式として評価されます。
ms.openlocfilehash: 220cb54680755461edb9dab6edf076f8ae0c6a68
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070810"
---
# <a name="variablemanagementconditionexpression-resource-type"></a><span data-ttu-id="1567d-103">variableManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1567d-103">variableManagementConditionExpression resource type</span></span>

> <span data-ttu-id="1567d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1567d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1567d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1567d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1567d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1567d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1567d-107">管理条件の状態は、ブール式として評価されます。</span><span class="sxs-lookup"><span data-stu-id="1567d-107">Evaluates the management condition state as a Boolean expression.</span></span>

<span data-ttu-id="1567d-108">[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1567d-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1567d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1567d-109">Properties</span></span>
|<span data-ttu-id="1567d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1567d-110">Property</span></span>|<span data-ttu-id="1567d-111">型</span><span class="sxs-lookup"><span data-stu-id="1567d-111">Type</span></span>|<span data-ttu-id="1567d-112">説明</span><span class="sxs-lookup"><span data-stu-id="1567d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1567d-113">managementConditionId</span><span class="sxs-lookup"><span data-stu-id="1567d-113">managementConditionId</span></span>|<span data-ttu-id="1567d-114">String</span><span class="sxs-lookup"><span data-stu-id="1567d-114">String</span></span>|<span data-ttu-id="1567d-115">式を評価するために使用される管理条件の id です。</span><span class="sxs-lookup"><span data-stu-id="1567d-115">The management condition id that is used to evaluate the expression.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1567d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1567d-116">Relationships</span></span>
<span data-ttu-id="1567d-117">なし</span><span class="sxs-lookup"><span data-stu-id="1567d-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1567d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1567d-118">JSON Representation</span></span>
<span data-ttu-id="1567d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1567d-119">Here is a JSON representation of the resource.</span></span>
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





