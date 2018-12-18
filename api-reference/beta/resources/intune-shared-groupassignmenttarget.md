---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
author: tfitzmac
ms.openlocfilehash: 5371554d069237dc6bc017c29574423b415f4f33
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323136"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="692ed-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="692ed-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="692ed-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="692ed-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="692ed-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="692ed-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="692ed-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="692ed-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="692ed-107">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="692ed-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="692ed-108">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="692ed-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="692ed-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="692ed-109">Properties</span></span>
|<span data-ttu-id="692ed-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="692ed-110">Property</span></span>|<span data-ttu-id="692ed-111">種類</span><span class="sxs-lookup"><span data-stu-id="692ed-111">Type</span></span>|<span data-ttu-id="692ed-112">説明</span><span class="sxs-lookup"><span data-stu-id="692ed-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="692ed-113">groupId</span><span class="sxs-lookup"><span data-stu-id="692ed-113">groupId</span></span>|<span data-ttu-id="692ed-114">文字列</span><span class="sxs-lookup"><span data-stu-id="692ed-114">String</span></span>|<span data-ttu-id="692ed-115">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="692ed-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="692ed-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="692ed-116">Relationships</span></span>
<span data-ttu-id="692ed-117">なし</span><span class="sxs-lookup"><span data-stu-id="692ed-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="692ed-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="692ed-118">JSON Representation</span></span>
<span data-ttu-id="692ed-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="692ed-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupAssignmentTarget",
  "groupId": "String"
}
```





