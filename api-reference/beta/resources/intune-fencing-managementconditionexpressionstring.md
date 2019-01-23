---
title: managementConditionExpressionString リソースの種類
description: 管理条件の式の文字列は、管理条件式の文字列表現です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8b8abc3492690afe6709070decbfe050356fd614
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419192"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="3b9a1-103">managementConditionExpressionString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3b9a1-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="3b9a1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3b9a1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3b9a1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b9a1-107">管理条件の式の文字列は、管理条件式の文字列表現です。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-107">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="3b9a1-108">[ManagementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3b9a1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b9a1-109">Properties</span></span>
|<span data-ttu-id="3b9a1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b9a1-110">Property</span></span>|<span data-ttu-id="3b9a1-111">型</span><span class="sxs-lookup"><span data-stu-id="3b9a1-111">Type</span></span>|<span data-ttu-id="3b9a1-112">説明</span><span class="sxs-lookup"><span data-stu-id="3b9a1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b9a1-113">value</span><span class="sxs-lookup"><span data-stu-id="3b9a1-113">value</span></span>|<span data-ttu-id="3b9a1-114">文字列</span><span class="sxs-lookup"><span data-stu-id="3b9a1-114">String</span></span>|<span data-ttu-id="3b9a1-115">管理条件ステートメント式の文字列値。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3b9a1-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3b9a1-116">Relationships</span></span>
<span data-ttu-id="3b9a1-117">なし</span><span class="sxs-lookup"><span data-stu-id="3b9a1-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3b9a1-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3b9a1-118">JSON Representation</span></span>
<span data-ttu-id="3b9a1-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3b9a1-119">Here is a JSON representation of the resource.</span></span>
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




