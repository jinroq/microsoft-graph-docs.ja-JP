---
title: managementConditionExpression リソースの種類
description: 管理条件式は、評価時にブール値を生成する式です。つまり、true または false のいずれかで、管理条件ステートメントがアクティブ化/非アクティブ化されたことを示します。 管理条件式は、式の変数とブール値の式の演算子の組み合わせで構成できます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b2611bf91fb5b69601cad52820ac9492c42e8937
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941262"
---
# <a name="managementconditionexpression-resource-type"></a><span data-ttu-id="be3df-104">managementConditionExpression リソースの種類</span><span class="sxs-lookup"><span data-stu-id="be3df-104">managementConditionExpression resource type</span></span>

> <span data-ttu-id="be3df-105">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="be3df-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be3df-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="be3df-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be3df-107">管理条件式は、評価時にブール値を生成する式です。つまり、true または false のいずれかで、管理条件ステートメントがアクティブ化/非アクティブ化されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="be3df-107">A management condition expression is an expression that produces a boolean value when evaluated, i.e. one of true or false, indicating that a management condition statement is activated/deactivated.</span></span> <span data-ttu-id="be3df-108">管理条件式は、式の変数とブール値の式の演算子の組み合わせで構成できます。</span><span class="sxs-lookup"><span data-stu-id="be3df-108">A management condition expression may be composed of a combination of the expression variables and boolean-valued expression operators.</span></span>

## <a name="properties"></a><span data-ttu-id="be3df-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be3df-109">Properties</span></span>
|<span data-ttu-id="be3df-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="be3df-110">Property</span></span>|<span data-ttu-id="be3df-111">型</span><span class="sxs-lookup"><span data-stu-id="be3df-111">Type</span></span>|<span data-ttu-id="be3df-112">説明</span><span class="sxs-lookup"><span data-stu-id="be3df-112">Description</span></span>|
|:---|:---|:---|

## <a name="relationships"></a><span data-ttu-id="be3df-113">関係</span><span class="sxs-lookup"><span data-stu-id="be3df-113">Relationships</span></span>
<span data-ttu-id="be3df-114">なし</span><span class="sxs-lookup"><span data-stu-id="be3df-114">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be3df-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="be3df-115">JSON Representation</span></span>
<span data-ttu-id="be3df-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="be3df-116">Here is a JSON representation of the resource.</span></span>
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




