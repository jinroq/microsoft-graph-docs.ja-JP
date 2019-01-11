---
title: managementConditionExpressionString リソースの種類
description: 管理条件の式の文字列は、管理条件式の文字列表現です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 815d799bc37328062a717097fd27bc0870a315f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811579"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="eae51-103">managementConditionExpressionString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="eae51-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="eae51-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="eae51-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="eae51-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eae51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eae51-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eae51-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eae51-107">管理条件の式の文字列は、管理条件式の文字列表現です。</span><span class="sxs-lookup"><span data-stu-id="eae51-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="eae51-108">[ManagementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="eae51-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="eae51-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eae51-109">Properties</span></span>
|<span data-ttu-id="eae51-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eae51-110">Property</span></span>|<span data-ttu-id="eae51-111">種類</span><span class="sxs-lookup"><span data-stu-id="eae51-111">Type</span></span>|<span data-ttu-id="eae51-112">説明</span><span class="sxs-lookup"><span data-stu-id="eae51-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eae51-113">value</span><span class="sxs-lookup"><span data-stu-id="eae51-113">value</span></span>|<span data-ttu-id="eae51-114">文字列</span><span class="sxs-lookup"><span data-stu-id="eae51-114">String</span></span>|<span data-ttu-id="eae51-115">管理条件ステートメント式の文字列値。</span><span class="sxs-lookup"><span data-stu-id="eae51-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eae51-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="eae51-116">Relationships</span></span>
<span data-ttu-id="eae51-117">なし</span><span class="sxs-lookup"><span data-stu-id="eae51-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="eae51-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="eae51-118">JSON Representation</span></span>
<span data-ttu-id="eae51-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="eae51-119">Here is a JSON representation of the resource.</span></span>
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





