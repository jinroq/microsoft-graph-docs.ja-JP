---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f344c0ed718f32352901af63da32c11ca02e2db6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849813"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="0c8b0-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0c8b0-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="0c8b0-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c8b0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c8b0-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c8b0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c8b0-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c8b0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c8b0-107">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="0c8b0-107">Represents an assignment to a group.</span></span>

<span data-ttu-id="0c8b0-108">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0c8b0-108">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0c8b0-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c8b0-109">Properties</span></span>
|<span data-ttu-id="0c8b0-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c8b0-110">Property</span></span>|<span data-ttu-id="0c8b0-111">種類</span><span class="sxs-lookup"><span data-stu-id="0c8b0-111">Type</span></span>|<span data-ttu-id="0c8b0-112">説明</span><span class="sxs-lookup"><span data-stu-id="0c8b0-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c8b0-113">groupId</span><span class="sxs-lookup"><span data-stu-id="0c8b0-113">groupId</span></span>|<span data-ttu-id="0c8b0-114">文字列</span><span class="sxs-lookup"><span data-stu-id="0c8b0-114">String</span></span>|<span data-ttu-id="0c8b0-115">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="0c8b0-115">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0c8b0-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0c8b0-116">Relationships</span></span>
<span data-ttu-id="0c8b0-117">なし</span><span class="sxs-lookup"><span data-stu-id="0c8b0-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0c8b0-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0c8b0-118">JSON Representation</span></span>
<span data-ttu-id="0c8b0-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0c8b0-119">Here is a JSON representation of the resource.</span></span>
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





