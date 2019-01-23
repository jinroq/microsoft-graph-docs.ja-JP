---
title: managementConditionExpression リソースの種類
description: 管理の条件式は、評価されるとき、つまり true または管理の条件付きステートメントがアクティブ/非アクティブであることを示す false のいずれかのブール値を生成する式です。 管理条件式は、式の変数とブール値の式の演算子の組み合わせで構成されます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e572cdae0104cf5bbb929286b4c3452dfd38eeea
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415510"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="6647b-104">managementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6647b-104">managementConditionExpression resource type</span></span>

> <span data-ttu-id="6647b-105">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6647b-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6647b-106">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6647b-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6647b-107">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6647b-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6647b-108">管理の条件式は、評価されるとき、つまり true または管理の条件付きステートメントがアクティブ/非アクティブであることを示す false のいずれかのブール値を生成する式です。</span><span class="sxs-lookup"><span data-stu-id="6647b-108">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="6647b-109">管理条件式は、式の変数とブール値の式の演算子の組み合わせで構成されます。</span><span class="sxs-lookup"><span data-stu-id="6647b-109">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>

## <a name="properties"></a><span data-ttu-id="6647b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6647b-110">Properties</span></span>
|<span data-ttu-id="6647b-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6647b-111">Property</span></span>|<span data-ttu-id="6647b-112">型</span><span class="sxs-lookup"><span data-stu-id="6647b-112">Type</span></span>|<span data-ttu-id="6647b-113">説明</span><span class="sxs-lookup"><span data-stu-id="6647b-113">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="6647b-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6647b-114">Relationships</span></span>
<span data-ttu-id="6647b-115">なし</span><span class="sxs-lookup"><span data-stu-id="6647b-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6647b-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6647b-116">JSON Representation</span></span>
<span data-ttu-id="6647b-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6647b-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementConditionExpression"
}
```




