---
title: groupPolicyConfigurationAssignment リソースの種類
description: グループ ポリシー設定の割り当てエンティティでは、特定のグループ ポリシーの構成を AAD の 1 つまたは複数のグループが割り当てられます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 508581ba7b5ac689338c179f4f6b211928c9abaf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430333"
---
# <a name="grouppolicyconfigurationassignment-resource-type"></a><span data-ttu-id="2642e-103">groupPolicyConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2642e-103">groupPolicyConfigurationAssignment resource type</span></span>

> <span data-ttu-id="2642e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2642e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2642e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2642e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2642e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2642e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2642e-107">グループ ポリシー設定の割り当てエンティティでは、特定のグループ ポリシーの構成を AAD の 1 つまたは複数のグループが割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="2642e-107">The group policy configuration assignment entity assigns one or more AAD groups to a specific group policy configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="2642e-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2642e-108">Methods</span></span>
|<span data-ttu-id="2642e-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2642e-109">Method</span></span>|<span data-ttu-id="2642e-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2642e-110">Return Type</span></span>|<span data-ttu-id="2642e-111">説明</span><span class="sxs-lookup"><span data-stu-id="2642e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2642e-112">リスト groupPolicyConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="2642e-112">List groupPolicyConfigurationAssignments</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-list.md)|<span data-ttu-id="2642e-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2642e-113">[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) collection</span></span>|<span data-ttu-id="2642e-114">[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2642e-114">List properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="2642e-115">GroupPolicyConfigurationAssignment を取得します。</span><span class="sxs-lookup"><span data-stu-id="2642e-115">Get groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-get.md)|[<span data-ttu-id="2642e-116">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2642e-116">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="2642e-117">[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2642e-117">Read properties and relationships of the [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2642e-118">GroupPolicyConfigurationAssignment を作成します。</span><span class="sxs-lookup"><span data-stu-id="2642e-118">Create groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-create.md)|[<span data-ttu-id="2642e-119">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2642e-119">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="2642e-120">新しい[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2642e-120">Create a new [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="2642e-121">GroupPolicyConfigurationAssignment を削除します。</span><span class="sxs-lookup"><span data-stu-id="2642e-121">Delete groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-delete.md)|<span data-ttu-id="2642e-122">なし</span><span class="sxs-lookup"><span data-stu-id="2642e-122">None</span></span>|<span data-ttu-id="2642e-123">の[groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="2642e-123">Deletes a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="2642e-124">GroupPolicyConfigurationAssignment を更新します。</span><span class="sxs-lookup"><span data-stu-id="2642e-124">Update groupPolicyConfigurationAssignment</span></span>](../api/intune-grouppolicy-grouppolicyconfigurationassignment-update.md)|[<span data-ttu-id="2642e-125">groupPolicyConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="2642e-125">groupPolicyConfigurationAssignment</span></span>](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)|<span data-ttu-id="2642e-126">[GroupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2642e-126">Update the properties of a [groupPolicyConfigurationAssignment](../resources/intune-grouppolicy-grouppolicyconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2642e-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2642e-127">Properties</span></span>
|<span data-ttu-id="2642e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2642e-128">Property</span></span>|<span data-ttu-id="2642e-129">型</span><span class="sxs-lookup"><span data-stu-id="2642e-129">Type</span></span>|<span data-ttu-id="2642e-130">説明</span><span class="sxs-lookup"><span data-stu-id="2642e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2642e-131">id</span><span class="sxs-lookup"><span data-stu-id="2642e-131">id</span></span>|<span data-ttu-id="2642e-132">String</span><span class="sxs-lookup"><span data-stu-id="2642e-132">String</span></span>|<span data-ttu-id="2642e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2642e-133">Key of the entity.</span></span>|
|<span data-ttu-id="2642e-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2642e-134">lastModifiedDateTime</span></span>|<span data-ttu-id="2642e-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2642e-135">DateTimeOffset</span></span>|<span data-ttu-id="2642e-136">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="2642e-136">The date and time the entity was last modified.</span></span>|
|<span data-ttu-id="2642e-137">target</span><span class="sxs-lookup"><span data-stu-id="2642e-137">target</span></span>|[<span data-ttu-id="2642e-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="2642e-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="2642e-139">グループの種類は、グループ ポリシーの構成を対象とします。</span><span class="sxs-lookup"><span data-stu-id="2642e-139">The type of groups targeted the group policy configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2642e-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2642e-140">Relationships</span></span>
<span data-ttu-id="2642e-141">なし</span><span class="sxs-lookup"><span data-stu-id="2642e-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2642e-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2642e-142">JSON Representation</span></span>
<span data-ttu-id="2642e-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2642e-143">Here is a JSON representation of the resource.</span></span>
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




