---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbd211bec428ff3a03ff989fa9ece36e5c55c561
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31775192"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="ff47d-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff47d-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="ff47d-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff47d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff47d-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff47d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff47d-106">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="ff47d-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="ff47d-107">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ff47d-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ff47d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff47d-108">Properties</span></span>
|<span data-ttu-id="ff47d-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff47d-109">Property</span></span>|<span data-ttu-id="ff47d-110">型</span><span class="sxs-lookup"><span data-stu-id="ff47d-110">Type</span></span>|<span data-ttu-id="ff47d-111">説明</span><span class="sxs-lookup"><span data-stu-id="ff47d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff47d-112">groupId</span><span class="sxs-lookup"><span data-stu-id="ff47d-112">groupId</span></span>|<span data-ttu-id="ff47d-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ff47d-113">String</span></span>|<span data-ttu-id="ff47d-114">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="ff47d-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="ff47d-115">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="ff47d-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff47d-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="ff47d-116">Relationships</span></span>
<span data-ttu-id="ff47d-117">なし</span><span class="sxs-lookup"><span data-stu-id="ff47d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff47d-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff47d-118">JSON Representation</span></span>
<span data-ttu-id="ff47d-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ff47d-119">Here is a JSON representation of the resource.</span></span>
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





