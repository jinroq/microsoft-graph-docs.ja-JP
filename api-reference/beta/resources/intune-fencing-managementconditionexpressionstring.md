---
title: managementcondition式 string リソースの種類
description: 管理条件式文字列は、管理条件式の文字列表現です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3dac405c71e4e85cc29bb36d335a57bb51fbe0f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31783739"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="0c860-103">managementcondition式 string リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c860-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="0c860-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c860-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c860-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0c860-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c860-106">管理条件式文字列は、管理条件式の文字列表現です。</span><span class="sxs-lookup"><span data-stu-id="0c860-106">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="0c860-107">[managementconditionexpression](../resources/intune-fencing-managementconditionexpression.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="0c860-107">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c860-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c860-108">Properties</span></span>
|<span data-ttu-id="0c860-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c860-109">Property</span></span>|<span data-ttu-id="0c860-110">型</span><span class="sxs-lookup"><span data-stu-id="0c860-110">Type</span></span>|<span data-ttu-id="0c860-111">説明</span><span class="sxs-lookup"><span data-stu-id="0c860-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c860-112">value</span><span class="sxs-lookup"><span data-stu-id="0c860-112">value</span></span>|<span data-ttu-id="0c860-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0c860-113">String</span></span>|<span data-ttu-id="0c860-114">管理条件ステートメントの式文字列値。</span><span class="sxs-lookup"><span data-stu-id="0c860-114">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c860-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c860-115">Relationships</span></span>
<span data-ttu-id="0c860-116">なし</span><span class="sxs-lookup"><span data-stu-id="0c860-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c860-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c860-117">JSON Representation</span></span>
<span data-ttu-id="0c860-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c860-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpressionString"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpressionString",
  "value": "String"
}
```





