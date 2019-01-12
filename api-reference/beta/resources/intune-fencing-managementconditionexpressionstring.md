---
title: managementConditionExpressionString リソースの種類
description: 管理条件の式の文字列は、管理条件式の文字列表現です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 872282914dc57be4e8e9bc7d476e7767907ec913
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968849"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="eefc1-103">managementConditionExpressionString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eefc1-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="eefc1-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eefc1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eefc1-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eefc1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eefc1-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eefc1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eefc1-107">管理条件の式の文字列は、管理条件式の文字列表現です。</span><span class="sxs-lookup"><span data-stu-id="eefc1-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="eefc1-108">[ManagementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="eefc1-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eefc1-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eefc1-109">Properties</span></span>
|<span data-ttu-id="eefc1-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eefc1-110">Property</span></span>|<span data-ttu-id="eefc1-111">種類</span><span class="sxs-lookup"><span data-stu-id="eefc1-111">Type</span></span>|<span data-ttu-id="eefc1-112">説明</span><span class="sxs-lookup"><span data-stu-id="eefc1-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eefc1-113">value</span><span class="sxs-lookup"><span data-stu-id="eefc1-113">value</span></span>|<span data-ttu-id="eefc1-114">文字列</span><span class="sxs-lookup"><span data-stu-id="eefc1-114">String</span></span>|<span data-ttu-id="eefc1-115">管理条件ステートメント式の文字列値。</span><span class="sxs-lookup"><span data-stu-id="eefc1-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eefc1-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eefc1-116">Relationships</span></span>
<span data-ttu-id="eefc1-117">なし</span><span class="sxs-lookup"><span data-stu-id="eefc1-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eefc1-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eefc1-118">JSON Representation</span></span>
<span data-ttu-id="eefc1-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eefc1-119">Here is a JSON representation of the resource.</span></span>
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





