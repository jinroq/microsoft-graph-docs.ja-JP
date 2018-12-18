---
title: managementConditionExpressionString リソースの種類
description: 管理条件の式の文字列は、管理条件式の文字列表現です。
author: tfitzmac
ms.openlocfilehash: eabcc730e86f74e2afc7c93874d47e787579c899
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27361041"
---
# <a name="managementconditionexpressionstring-resource-type"></a><span data-ttu-id="81fc4-103">managementConditionExpressionString リソースの種類</span><span class="sxs-lookup"><span data-stu-id="81fc4-103">managementConditionExpressionString resource type</span></span>

> <span data-ttu-id="81fc4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="81fc4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81fc4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81fc4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="81fc4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="81fc4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="81fc4-107">管理条件の式の文字列は、管理条件式の文字列表現です。</span><span class="sxs-lookup"><span data-stu-id="81fc4-107">A management condition expression string is a string representation of a management condition expression.</span></span>

<span data-ttu-id="81fc4-108">[ManagementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="81fc4-108">Inherits from [managementConditionExpression](../resources/intune-fencing-managementconditionexpression.md)</span></span>

## <a name="properties"></a><span data-ttu-id="81fc4-109">Properties</span><span class="sxs-lookup"><span data-stu-id="81fc4-109">Properties</span></span>
|<span data-ttu-id="81fc4-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81fc4-110">Property</span></span>|<span data-ttu-id="81fc4-111">種類</span><span class="sxs-lookup"><span data-stu-id="81fc4-111">Type</span></span>|<span data-ttu-id="81fc4-112">説明</span><span class="sxs-lookup"><span data-stu-id="81fc4-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81fc4-113">value</span><span class="sxs-lookup"><span data-stu-id="81fc4-113">value</span></span>|<span data-ttu-id="81fc4-114">文字列</span><span class="sxs-lookup"><span data-stu-id="81fc4-114">String</span></span>|<span data-ttu-id="81fc4-115">管理条件ステートメント式の文字列値。</span><span class="sxs-lookup"><span data-stu-id="81fc4-115">The management condition statement expression string value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="81fc4-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="81fc4-116">Relationships</span></span>
<span data-ttu-id="81fc4-117">なし</span><span class="sxs-lookup"><span data-stu-id="81fc4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="81fc4-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="81fc4-118">JSON Representation</span></span>
<span data-ttu-id="81fc4-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="81fc4-119">Here is a JSON representation of the resource.</span></span>
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





