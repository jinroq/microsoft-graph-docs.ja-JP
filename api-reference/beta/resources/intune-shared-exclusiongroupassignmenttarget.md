---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 6d8973a8974c15c9243d901d65a3d5dd9dbe1a54
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010470"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="b7b43-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b7b43-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="b7b43-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7b43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7b43-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7b43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7b43-106">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="b7b43-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="b7b43-107">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b7b43-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="b7b43-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7b43-108">Properties</span></span>
|<span data-ttu-id="b7b43-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7b43-109">Property</span></span>|<span data-ttu-id="b7b43-110">型</span><span class="sxs-lookup"><span data-stu-id="b7b43-110">Type</span></span>|<span data-ttu-id="b7b43-111">説明</span><span class="sxs-lookup"><span data-stu-id="b7b43-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7b43-112">groupId</span><span class="sxs-lookup"><span data-stu-id="b7b43-112">groupId</span></span>|<span data-ttu-id="b7b43-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b7b43-113">String</span></span>|<span data-ttu-id="b7b43-114">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="b7b43-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="b7b43-115">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="b7b43-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b7b43-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b7b43-116">Relationships</span></span>
<span data-ttu-id="b7b43-117">なし</span><span class="sxs-lookup"><span data-stu-id="b7b43-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b7b43-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b7b43-118">JSON Representation</span></span>
<span data-ttu-id="b7b43-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b7b43-119">Here is a JSON representation of the resource.</span></span>
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





