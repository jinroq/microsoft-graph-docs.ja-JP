---
title: deviceManagementCollectionSettingInstance リソースの種類
description: 値のコレクションを表す設定インスタンス
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b569bb4d0b38eb3fd9c3909d559e3066b4ccae6f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36365420"
---
# <a name="devicemanagementcollectionsettinginstance-resource-type"></a><span data-ttu-id="b8090-103">deviceManagementCollectionSettingInstance リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8090-103">deviceManagementCollectionSettingInstance resource type</span></span>

> <span data-ttu-id="b8090-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b8090-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8090-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b8090-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8090-106">値のコレクションを表す設定インスタンス</span><span class="sxs-lookup"><span data-stu-id="b8090-106">A setting instance representing a collection of values</span></span>


<span data-ttu-id="b8090-107">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="b8090-107">Inherits from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b8090-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8090-108">Methods</span></span>
|<span data-ttu-id="b8090-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8090-109">Method</span></span>|<span data-ttu-id="b8090-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8090-110">Return Type</span></span>|<span data-ttu-id="b8090-111">説明</span><span class="sxs-lookup"><span data-stu-id="b8090-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8090-112">DeviceManagementCollectionSettingInstances を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="b8090-112">List deviceManagementCollectionSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-list.md)|<span data-ttu-id="b8090-113">[Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b8090-113">[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) collection</span></span>|<span data-ttu-id="b8090-114">[Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b8090-114">List properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="b8090-115">DeviceManagementCollectionSettingInstance を取得する</span><span class="sxs-lookup"><span data-stu-id="b8090-115">Get deviceManagementCollectionSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-get.md)|[<span data-ttu-id="b8090-116">deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="b8090-116">deviceManagementCollectionSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|<span data-ttu-id="b8090-117">[Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b8090-117">Read properties and relationships of the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>|
|[<span data-ttu-id="b8090-118">DeviceManagementCollectionSettingInstance の作成</span><span class="sxs-lookup"><span data-stu-id="b8090-118">Create deviceManagementCollectionSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-create.md)|[<span data-ttu-id="b8090-119">deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="b8090-119">deviceManagementCollectionSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|<span data-ttu-id="b8090-120">新しい[Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b8090-120">Create a new [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>|
|[<span data-ttu-id="b8090-121">DeviceManagementCollectionSettingInstance の削除</span><span class="sxs-lookup"><span data-stu-id="b8090-121">Delete deviceManagementCollectionSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-delete.md)|<span data-ttu-id="b8090-122">None</span><span class="sxs-lookup"><span data-stu-id="b8090-122">None</span></span>|<span data-ttu-id="b8090-123">[Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="b8090-123">Deletes a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>|
|[<span data-ttu-id="b8090-124">DeviceManagementCollectionSettingInstance の更新</span><span class="sxs-lookup"><span data-stu-id="b8090-124">Update deviceManagementCollectionSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementcollectionsettinginstance-update.md)|[<span data-ttu-id="b8090-125">deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="b8090-125">deviceManagementCollectionSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)|<span data-ttu-id="b8090-126">[Devicemanagementcollectionsettinginstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8090-126">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b8090-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8090-127">Properties</span></span>
|<span data-ttu-id="b8090-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8090-128">Property</span></span>|<span data-ttu-id="b8090-129">型</span><span class="sxs-lookup"><span data-stu-id="b8090-129">Type</span></span>|<span data-ttu-id="b8090-130">説明</span><span class="sxs-lookup"><span data-stu-id="b8090-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8090-131">id</span><span class="sxs-lookup"><span data-stu-id="b8090-131">id</span></span>|<span data-ttu-id="b8090-132">String</span><span class="sxs-lookup"><span data-stu-id="b8090-132">String</span></span>|<span data-ttu-id="b8090-133">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された設定インスタンス ID</span><span class="sxs-lookup"><span data-stu-id="b8090-133">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b8090-134">definitionId</span><span class="sxs-lookup"><span data-stu-id="b8090-134">definitionId</span></span>|<span data-ttu-id="b8090-135">String</span><span class="sxs-lookup"><span data-stu-id="b8090-135">String</span></span>|<span data-ttu-id="b8090-136">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承されたこのインスタンスの設定定義の ID</span><span class="sxs-lookup"><span data-stu-id="b8090-136">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b8090-137">valueJson</span><span class="sxs-lookup"><span data-stu-id="b8090-137">valueJson</span></span>|<span data-ttu-id="b8090-138">String</span><span class="sxs-lookup"><span data-stu-id="b8090-138">String</span></span>|<span data-ttu-id="b8090-139">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)から継承された値の JSON 表現</span><span class="sxs-lookup"><span data-stu-id="b8090-139">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8090-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8090-140">Relationships</span></span>
|<span data-ttu-id="b8090-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8090-141">Relationship</span></span>|<span data-ttu-id="b8090-142">型</span><span class="sxs-lookup"><span data-stu-id="b8090-142">Type</span></span>|<span data-ttu-id="b8090-143">説明</span><span class="sxs-lookup"><span data-stu-id="b8090-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8090-144">value</span><span class="sxs-lookup"><span data-stu-id="b8090-144">value</span></span>|<span data-ttu-id="b8090-145">[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b8090-145">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="b8090-146">値のコレクション</span><span class="sxs-lookup"><span data-stu-id="b8090-146">The collection of values</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b8090-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8090-147">JSON Representation</span></span>
<span data-ttu-id="b8090-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8090-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCollectionSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```



