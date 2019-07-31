---
title: Managementcondition式 String リソースの種類
description: 管理条件式文字列は、管理条件式の文字列表現です。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7a0ed3cd867592c5cf46e98ec8bde923effd8b02
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998717"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="f3468-103">Managementcondition式 String リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f3468-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="f3468-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f3468-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3468-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f3468-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3468-106">管理条件式文字列は、管理条件式の文字列表現です。</span><span class="sxs-lookup"><span data-stu-id="f3468-106">A management condition expression string is a string representation of a management condition expression.</span></span>


<span data-ttu-id="f3468-107">[Managementconditionexpression](../resources/intune-fencing-managementconditionexpression.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="f3468-107">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f3468-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3468-108">Properties</span></span>
|<span data-ttu-id="f3468-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f3468-109">Property</span></span>|<span data-ttu-id="f3468-110">型</span><span class="sxs-lookup"><span data-stu-id="f3468-110">Type</span></span>|<span data-ttu-id="f3468-111">説明</span><span class="sxs-lookup"><span data-stu-id="f3468-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3468-112">value</span><span class="sxs-lookup"><span data-stu-id="f3468-112">value</span></span>|<span data-ttu-id="f3468-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f3468-113">String</span></span>|<span data-ttu-id="f3468-114">管理条件ステートメントの式文字列値。</span><span class="sxs-lookup"><span data-stu-id="f3468-114">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3468-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f3468-115">Relationships</span></span>
<span data-ttu-id="f3468-116">なし</span><span class="sxs-lookup"><span data-stu-id="f3468-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3468-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f3468-117">JSON Representation</span></span>
<span data-ttu-id="f3468-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f3468-118">Here is a JSON representation of the resource.</span></span>
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





