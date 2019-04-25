---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fbfa4e6df9dae514a99fa96aace073bd702def9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523764"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="b5297-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b5297-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="b5297-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5297-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5297-105">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="b5297-105">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="b5297-106">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b5297-106">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b5297-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5297-107">Properties</span></span>
|<span data-ttu-id="b5297-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5297-108">Property</span></span>|<span data-ttu-id="b5297-109">型</span><span class="sxs-lookup"><span data-stu-id="b5297-109">Type</span></span>|<span data-ttu-id="b5297-110">説明</span><span class="sxs-lookup"><span data-stu-id="b5297-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5297-111">groupId</span><span class="sxs-lookup"><span data-stu-id="b5297-111">groupId</span></span>|<span data-ttu-id="b5297-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b5297-112">String</span></span>|<span data-ttu-id="b5297-113">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="b5297-113">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="b5297-114">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b5297-114">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b5297-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b5297-115">Relationships</span></span>
<span data-ttu-id="b5297-116">なし</span><span class="sxs-lookup"><span data-stu-id="b5297-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b5297-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5297-117">JSON Representation</span></span>
<span data-ttu-id="b5297-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5297-118">Here is a JSON representation of the resource.</span></span>
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



