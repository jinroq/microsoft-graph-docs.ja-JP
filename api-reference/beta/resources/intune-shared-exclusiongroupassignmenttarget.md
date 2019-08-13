---
title: exclusionGroupAssignmentTarget リソースの種類
description: 割り当てから除外するグループを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: acaee282e4b78e3076a226f5918f8a71d7e0874f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348054"
---
# <a name="exclusiongroupassignmenttarget-resource-type"></a><span data-ttu-id="0376c-103">exclusionGroupAssignmentTarget リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0376c-103">exclusionGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="0376c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0376c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0376c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0376c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0376c-106">割り当てから除外するグループを表します。</span><span class="sxs-lookup"><span data-stu-id="0376c-106">Represents a group that should be excluded from an assignment.</span></span>


<span data-ttu-id="0376c-107">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0376c-107">Inherits from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="0376c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0376c-108">Properties</span></span>
|<span data-ttu-id="0376c-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0376c-109">Property</span></span>|<span data-ttu-id="0376c-110">型</span><span class="sxs-lookup"><span data-stu-id="0376c-110">Type</span></span>|<span data-ttu-id="0376c-111">説明</span><span class="sxs-lookup"><span data-stu-id="0376c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0376c-112">groupId</span><span class="sxs-lookup"><span data-stu-id="0376c-112">groupId</span></span>|<span data-ttu-id="0376c-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0376c-113">String</span></span>|<span data-ttu-id="0376c-114">割り当てのターゲットとなるグループ ID です。</span><span class="sxs-lookup"><span data-stu-id="0376c-114">The group Id that is the target of the assignment.</span></span> <span data-ttu-id="0376c-115">[groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="0376c-115">Inherited from [groupAssignmentTarget](../resources/intune-shared-groupassignmenttarget.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="0376c-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0376c-116">Relationships</span></span>
<span data-ttu-id="0376c-117">なし</span><span class="sxs-lookup"><span data-stu-id="0376c-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0376c-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0376c-118">JSON Representation</span></span>
<span data-ttu-id="0376c-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0376c-119">Here is a JSON representation of the resource.</span></span>
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



