---
title: groupPolicyConfigurationAssignment リソースの種類
description: グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e0ec4346174bdaafbc37c0721462ba8fd612abcc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34975946"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="75775-103">groupPolicyConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75775-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="75775-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75775-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75775-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75775-106">グループポリシー構成割り当てエンティティは、1つ以上の AAD グループを特定のグループポリシー構成に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="75775-106">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="75775-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="75775-107">Methods</span></span>
|<span data-ttu-id="75775-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="75775-108">Method</span></span>|<span data-ttu-id="75775-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="75775-109">Return Type</span></span>|<span data-ttu-id="75775-110">説明</span><span class="sxs-lookup"><span data-stu-id="75775-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75775-111">GroupPolicyConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="75775-111">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="75775-112">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="75775-112">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="75775-113">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="75775-113">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="75775-114">GroupPolicyConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="75775-114">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="75775-115">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="75775-115">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="75775-116">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75775-116">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="75775-117">GroupPolicyConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="75775-117">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="75775-118">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="75775-118">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="75775-119">新しい[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="75775-119">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="75775-120">GroupPolicyConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="75775-120">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="75775-121">None</span><span class="sxs-lookup"><span data-stu-id="75775-121">None</span></span>|<span data-ttu-id="75775-122">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="75775-122">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="75775-123">GroupPolicyConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="75775-123">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="75775-124">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="75775-124">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="75775-125">[Grouppolicyconfigurationassignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="75775-125">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75775-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75775-126">Properties</span></span>
|<span data-ttu-id="75775-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75775-127">Property</span></span>|<span data-ttu-id="75775-128">型</span><span class="sxs-lookup"><span data-stu-id="75775-128">Type</span></span>|<span data-ttu-id="75775-129">説明</span><span class="sxs-lookup"><span data-stu-id="75775-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75775-130">id</span><span class="sxs-lookup"><span data-stu-id="75775-130">id</span></span>|<span data-ttu-id="75775-131">String</span><span class="sxs-lookup"><span data-stu-id="75775-131">String</span></span>|<span data-ttu-id="75775-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="75775-132">Key of the entity.</span></span>|
|<span data-ttu-id="75775-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75775-133">lastModifiedDateTime</span></span>|<span data-ttu-id="75775-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75775-134">DateTimeOffset</span></span>|<span data-ttu-id="75775-135">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="75775-135">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="75775-136">target</span><span class="sxs-lookup"><span data-stu-id="75775-136">target</span></span>|[<span data-ttu-id="75775-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="75775-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="75775-138">グループポリシー構成を対象としたグループの種類。</span><span class="sxs-lookup"><span data-stu-id="75775-138">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75775-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75775-139">Relationships</span></span>
<span data-ttu-id="75775-140">なし</span><span class="sxs-lookup"><span data-stu-id="75775-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75775-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75775-141">JSON Representation</span></span>
<span data-ttu-id="75775-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75775-142">Here is a JSON representation of the resource.</span></span>
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





