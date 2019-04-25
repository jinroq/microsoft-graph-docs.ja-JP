---
title: grouppolicyconfigurationassignment リソースの種類
description: グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1f6fcd7ace912075189ec3e9b5a817181dd392a5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575822"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="c5a2a-103">grouppolicyconfigurationassignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c5a2a-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="c5a2a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c5a2a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c5a2a-106">グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="c5a2a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c5a2a-107">Methods</span></span>
|<span data-ttu-id="c5a2a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c5a2a-108">Method</span></span>|<span data-ttu-id="c5a2a-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c5a2a-109">Return Type</span></span>|<span data-ttu-id="c5a2a-110">説明</span><span class="sxs-lookup"><span data-stu-id="c5a2a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c5a2a-111">grouppolicyconfigurationassignments のリスト</span><span class="sxs-lookup"><span data-stu-id="c5a2a-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="c5a2a-112">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c5a2a-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c5a2a-113">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="c5a2a-114">grouppolicyconfigurationassignment の取得</span><span class="sxs-lookup"><span data-stu-id="c5a2a-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="c5a2a-115">grouppolicyconfigurationassignment</span><span class="sxs-lookup"><span data-stu-id="c5a2a-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c5a2a-116">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c5a2a-117">grouppolicyconfigurationassignment の作成</span><span class="sxs-lookup"><span data-stu-id="c5a2a-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="c5a2a-118">grouppolicyconfigurationassignment</span><span class="sxs-lookup"><span data-stu-id="c5a2a-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c5a2a-119">新しい[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="c5a2a-120">grouppolicyconfigurationassignment の削除</span><span class="sxs-lookup"><span data-stu-id="c5a2a-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="c5a2a-121">なし</span><span class="sxs-lookup"><span data-stu-id="c5a2a-121">None</span></span>|<span data-ttu-id="c5a2a-122">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="c5a2a-123">grouppolicyconfigurationassignment の更新</span><span class="sxs-lookup"><span data-stu-id="c5a2a-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="c5a2a-124">grouppolicyconfigurationassignment</span><span class="sxs-lookup"><span data-stu-id="c5a2a-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="c5a2a-125">[grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c5a2a-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5a2a-126">Properties</span></span>
|<span data-ttu-id="c5a2a-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c5a2a-127">Property</span></span>|<span data-ttu-id="c5a2a-128">型</span><span class="sxs-lookup"><span data-stu-id="c5a2a-128">Type</span></span>|<span data-ttu-id="c5a2a-129">説明</span><span class="sxs-lookup"><span data-stu-id="c5a2a-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c5a2a-130">id</span><span class="sxs-lookup"><span data-stu-id="c5a2a-130">id</span></span>|<span data-ttu-id="c5a2a-131">String</span><span class="sxs-lookup"><span data-stu-id="c5a2a-131">String</span></span>|<span data-ttu-id="c5a2a-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-132">Key of the entity.</span></span>|
|<span data-ttu-id="c5a2a-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c5a2a-133">lastModifiedDateTime</span></span>|<span data-ttu-id="c5a2a-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c5a2a-134">DateTimeOffset</span></span>|<span data-ttu-id="c5a2a-135">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="c5a2a-136">target</span><span class="sxs-lookup"><span data-stu-id="c5a2a-136">target</span></span>|[<span data-ttu-id="c5a2a-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c5a2a-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c5a2a-138">グループポリシー構成を対象としたグループの種類。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c5a2a-139">関係</span><span class="sxs-lookup"><span data-stu-id="c5a2a-139">Relationships</span></span>
<span data-ttu-id="c5a2a-140">なし</span><span class="sxs-lookup"><span data-stu-id="c5a2a-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c5a2a-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c5a2a-141">JSON Representation</span></span>
<span data-ttu-id="c5a2a-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c5a2a-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyConfigurationAssignment",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





