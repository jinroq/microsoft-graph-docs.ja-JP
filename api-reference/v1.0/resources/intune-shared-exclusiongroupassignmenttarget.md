---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: tfitzmac
ms.openlocfilehash: 8193ac714f7f68dc371454c809c3eaa3176f8453
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304516"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="a2b48-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a2b48-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="a2b48-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2b48-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2b48-105">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="a2b48-105">Represents a group that should be excluded from an assignment.</span></span>

<span data-ttu-id="a2b48-106">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a2b48-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a2b48-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2b48-107">Properties</span></span>
|<span data-ttu-id="a2b48-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2b48-108">Property</span></span>|<span data-ttu-id="a2b48-109">種類</span><span class="sxs-lookup"><span data-stu-id="a2b48-109">Type</span></span>|<span data-ttu-id="a2b48-110">説明</span><span class="sxs-lookup"><span data-stu-id="a2b48-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2b48-111">groupId</span><span class="sxs-lookup"><span data-stu-id="a2b48-111">groupId</span></span>|<span data-ttu-id="a2b48-112">文字列</span><span class="sxs-lookup"><span data-stu-id="a2b48-112">String</span></span>|<span data-ttu-id="a2b48-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="a2b48-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="a2b48-114">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a2b48-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2b48-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a2b48-115">Relationships</span></span>
<span data-ttu-id="a2b48-116">なし</span><span class="sxs-lookup"><span data-stu-id="a2b48-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a2b48-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a2b48-117">JSON Representation</span></span>
<span data-ttu-id="a2b48-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a2b48-118">Here is a JSON representation of the resource.</span></span>
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



