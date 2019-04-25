---
title: deviceConfigurationAssignment リソースの種類
description: デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69c7fc6dc2a4a3ff90e14d430fba9b564930e0a7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567901"
---
# <a name="deviceconfigurationassignment-resource-type"></a><span data-ttu-id="ce9c5-103">deviceConfigurationAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce9c5-103">deviceConfigurationAssignment resource type</span></span>

> <span data-ttu-id="ce9c5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce9c5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce9c5-106">デバイス構成の割り当てエンティティは、特定のデバイス構成に AAD グループを割り当てます。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-106">The device configuration assignment entity assigns an AAD group to a specific device configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="ce9c5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce9c5-107">Methods</span></span>
|<span data-ttu-id="ce9c5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="ce9c5-108">Method</span></span>|<span data-ttu-id="ce9c5-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="ce9c5-109">Return Type</span></span>|<span data-ttu-id="ce9c5-110">説明</span><span class="sxs-lookup"><span data-stu-id="ce9c5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce9c5-111">deviceConfigurationAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="ce9c5-111">List deviceConfigurationAssignments</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-list.md)|<span data-ttu-id="ce9c5-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ce9c5-112">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="ce9c5-113">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-113">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>|
|[<span data-ttu-id="ce9c5-114">deviceConfigurationAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="ce9c5-114">Get deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-get.md)|[<span data-ttu-id="ce9c5-115">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ce9c5-115">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="ce9c5-116">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-116">Read properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="ce9c5-117">deviceConfigurationAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="ce9c5-117">Create deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-create.md)|[<span data-ttu-id="ce9c5-118">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ce9c5-118">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="ce9c5-119">新しい [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-119">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|
|[<span data-ttu-id="ce9c5-120">deviceConfigurationAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="ce9c5-120">Delete deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-delete.md)|<span data-ttu-id="ce9c5-121">なし</span><span class="sxs-lookup"><span data-stu-id="ce9c5-121">None</span></span>|<span data-ttu-id="ce9c5-122">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-122">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>|
|[<span data-ttu-id="ce9c5-123">deviceConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="ce9c5-123">Update deviceConfigurationAssignment</span></span>](../api/intune-deviceconfig-deviceconfigurationassignment-update.md)|[<span data-ttu-id="ce9c5-124">deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ce9c5-124">deviceConfigurationAssignment</span></span>](../resources/intune-deviceconfig-deviceconfigurationassignment.md)|<span data-ttu-id="ce9c5-125">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-125">Update the properties of a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce9c5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce9c5-126">Properties</span></span>
|<span data-ttu-id="ce9c5-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce9c5-127">Property</span></span>|<span data-ttu-id="ce9c5-128">型</span><span class="sxs-lookup"><span data-stu-id="ce9c5-128">Type</span></span>|<span data-ttu-id="ce9c5-129">説明</span><span class="sxs-lookup"><span data-stu-id="ce9c5-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce9c5-130">id</span><span class="sxs-lookup"><span data-stu-id="ce9c5-130">id</span></span>|<span data-ttu-id="ce9c5-131">String</span><span class="sxs-lookup"><span data-stu-id="ce9c5-131">String</span></span>|<span data-ttu-id="ce9c5-132">割り当てのキー。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-132">The key of the assignment.</span></span>|
|<span data-ttu-id="ce9c5-133">target</span><span class="sxs-lookup"><span data-stu-id="ce9c5-133">target</span></span>|[<span data-ttu-id="ce9c5-134">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ce9c5-134">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="ce9c5-135">デバイス構成の割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-135">The assignment target for the device configuration.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce9c5-136">関係</span><span class="sxs-lookup"><span data-stu-id="ce9c5-136">Relationships</span></span>
<span data-ttu-id="ce9c5-137">なし</span><span class="sxs-lookup"><span data-stu-id="ce9c5-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce9c5-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce9c5-138">JSON Representation</span></span>
<span data-ttu-id="ce9c5-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ce9c5-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





