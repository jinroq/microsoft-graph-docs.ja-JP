---
title: unaryManagementConditionExpression リソースの種類
description: 単項演算を使用して評価される管理条件式です。
ms.openlocfilehash: 958c180e52a268f849eca1fe0d2a2b75ff81333b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070525"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="d1bf1-103">unaryManagementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d1bf1-103">unaryManagementConditionExpression resource type</span></span>

> <span data-ttu-id="d1bf1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1bf1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d1bf1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d1bf1-107">単項演算を使用して評価される管理条件式です。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-107">A management condition expression that is evaluated using a unary operation.</span></span>

<span data-ttu-id="d1bf1-108">[ManagementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d1bf1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1bf1-109">Properties</span></span>
|<span data-ttu-id="d1bf1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d1bf1-110">Property</span></span>|<span data-ttu-id="d1bf1-111">型</span><span class="sxs-lookup"><span data-stu-id="d1bf1-111">Type</span></span>|<span data-ttu-id="d1bf1-112">説明</span><span class="sxs-lookup"><span data-stu-id="d1bf1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1bf1-113">operator</span><span class="sxs-lookup"><span data-stu-id="d1bf1-113">operator</span></span>|[<span data-ttu-id="d1bf1-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="d1bf1-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="d1bf1-115">単項演算の評価に使用する演算子です。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="d1bf1-116">使用可能な値: `not`。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="d1bf1-117">オペランド</span><span class="sxs-lookup"><span data-stu-id="d1bf1-117">operand</span></span>|[<span data-ttu-id="d1bf1-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="d1bf1-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="d1bf1-119">単項演算のオペランドです。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1bf1-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d1bf1-120">Relationships</span></span>
<span data-ttu-id="d1bf1-121">なし</span><span class="sxs-lookup"><span data-stu-id="d1bf1-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d1bf1-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d1bf1-122">JSON Representation</span></span>
<span data-ttu-id="d1bf1-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d1bf1-123">Here is a JSON representation of the resource.</span></span>
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





