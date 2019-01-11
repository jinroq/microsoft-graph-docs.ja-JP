---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ad844205e0cb5f5b4d0b86d71212e2d9c2ca223e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826454"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="f59ad-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f59ad-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="f59ad-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f59ad-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f59ad-105">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="f59ad-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="f59ad-106">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f59ad-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f59ad-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f59ad-107">Properties</span></span>
|<span data-ttu-id="f59ad-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f59ad-108">Property</span></span>|<span data-ttu-id="f59ad-109">種類</span><span class="sxs-lookup"><span data-stu-id="f59ad-109">Type</span></span>|<span data-ttu-id="f59ad-110">説明</span><span class="sxs-lookup"><span data-stu-id="f59ad-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f59ad-111">groupId</span><span class="sxs-lookup"><span data-stu-id="f59ad-111">groupId</span></span>|<span data-ttu-id="f59ad-112">文字列</span><span class="sxs-lookup"><span data-stu-id="f59ad-112">String</span></span>|<span data-ttu-id="f59ad-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="f59ad-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="f59ad-114">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f59ad-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="f59ad-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f59ad-115">Relationships</span></span>
<span data-ttu-id="f59ad-116">なし</span><span class="sxs-lookup"><span data-stu-id="f59ad-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f59ad-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f59ad-117">JSON Representation</span></span>
<span data-ttu-id="f59ad-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f59ad-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.exclusionGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.exclusionGroupAssignmentTarget",
  "groupId": "String"
}
```



