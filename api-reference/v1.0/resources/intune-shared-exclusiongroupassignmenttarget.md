---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fbfa4e6df9dae514a99fa96aace073bd702def9
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254087"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="92e58-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="92e58-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="92e58-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92e58-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92e58-105">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="92e58-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="92e58-106">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="92e58-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="92e58-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92e58-107">Properties</span></span>
|<span data-ttu-id="92e58-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="92e58-108">Property</span></span>|<span data-ttu-id="92e58-109">型</span><span class="sxs-lookup"><span data-stu-id="92e58-109">Type</span></span>|<span data-ttu-id="92e58-110">説明</span><span class="sxs-lookup"><span data-stu-id="92e58-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="92e58-111">groupId</span><span class="sxs-lookup"><span data-stu-id="92e58-111">groupId</span></span>|<span data-ttu-id="92e58-112">文字列</span><span class="sxs-lookup"><span data-stu-id="92e58-112">String</span></span>|<span data-ttu-id="92e58-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="92e58-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="92e58-114">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="92e58-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="92e58-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="92e58-115">Relationships</span></span>
<span data-ttu-id="92e58-116">なし</span><span class="sxs-lookup"><span data-stu-id="92e58-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="92e58-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="92e58-117">JSON Representation</span></span>
<span data-ttu-id="92e58-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="92e58-118">Here is a JSON representation of the resource.</span></span>
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



