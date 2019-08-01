---
title: groupAssignmentTarget リソースの種類
description: グループへの割り当てを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 87e4e4707a1884e7d657bae9c6e41fee69dc831d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036919"
---
# <a name="groupassignmenttarget-resource-type"></a><span data-ttu-id="bb522-103">groupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb522-103">groupAssignmentTarget resource type</span></span>

> <span data-ttu-id="bb522-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bb522-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb522-105">グループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="bb522-105">Represents an assignment to a group.</span></span>


<span data-ttu-id="bb522-106">[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="bb522-106">Inherits from [deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bb522-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb522-107">Properties</span></span>
|<span data-ttu-id="bb522-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb522-108">Property</span></span>|<span data-ttu-id="bb522-109">型</span><span class="sxs-lookup"><span data-stu-id="bb522-109">Type</span></span>|<span data-ttu-id="bb522-110">説明</span><span class="sxs-lookup"><span data-stu-id="bb522-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb522-111">groupId</span><span class="sxs-lookup"><span data-stu-id="bb522-111">groupId</span></span>|<span data-ttu-id="bb522-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="bb522-112">String</span></span>|<span data-ttu-id="bb522-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="bb522-113">The group Id that is the target of the assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb522-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb522-114">Relationships</span></span>
<span data-ttu-id="bb522-115">なし</span><span class="sxs-lookup"><span data-stu-id="bb522-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb522-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb522-116">JSON Representation</span></span>
<span data-ttu-id="bb522-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb522-117">Here is a JSON representation of the resource.</span></span>
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



