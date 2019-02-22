---
title: windowsinformationprotectionwipepeaction リソースの種類
description: テナント管理者が独自のデバイス (byod) Windows デバイス用に発行したワイプ要求を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e08cd6a2cf27830f6f88328440fb100bcd77ef6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148007"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a><span data-ttu-id="04089-103">windowsinformationprotectionwipepeaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04089-103">windowsInformationProtectionWipeAction resource type</span></span>

> <span data-ttu-id="04089-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04089-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04089-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04089-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04089-106">テナント管理者が独自のデバイス (byod) Windows デバイス用に発行したワイプ要求を表します。</span><span class="sxs-lookup"><span data-stu-id="04089-106">Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="04089-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="04089-107">Methods</span></span>
|<span data-ttu-id="04089-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="04089-108">Method</span></span>|<span data-ttu-id="04089-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="04089-109">Return Type</span></span>|<span data-ttu-id="04089-110">説明</span><span class="sxs-lookup"><span data-stu-id="04089-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="04089-111">windowsinformationprotectionwipeactions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="04089-111">List windowsInformationProtectionWipeActions</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|<span data-ttu-id="04089-112">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="04089-112">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) collection</span></span>|<span data-ttu-id="04089-113">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="04089-113">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>|
|[<span data-ttu-id="04089-114">windowsinformationprotectionwipeaction を取得する</span><span class="sxs-lookup"><span data-stu-id="04089-114">Get windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[<span data-ttu-id="04089-115">windowsinformationprotectionwipeaction</span><span class="sxs-lookup"><span data-stu-id="04089-115">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="04089-116">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="04089-116">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="04089-117">windowsinformationprotectionwipeaction を作成する</span><span class="sxs-lookup"><span data-stu-id="04089-117">Create windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[<span data-ttu-id="04089-118">windowsinformationprotectionwipeaction</span><span class="sxs-lookup"><span data-stu-id="04089-118">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="04089-119">新しい[windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="04089-119">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="04089-120">windowsinformationprotectionwipeaction を削除する</span><span class="sxs-lookup"><span data-stu-id="04089-120">Delete windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|<span data-ttu-id="04089-121">なし</span><span class="sxs-lookup"><span data-stu-id="04089-121">None</span></span>|<span data-ttu-id="04089-122">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="04089-122">Deletes a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>|
|[<span data-ttu-id="04089-123">windowsinformationprotectionwipeaction を更新する</span><span class="sxs-lookup"><span data-stu-id="04089-123">Update windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[<span data-ttu-id="04089-124">windowsinformationprotectionwipeaction</span><span class="sxs-lookup"><span data-stu-id="04089-124">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="04089-125">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="04089-125">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="04089-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04089-126">Properties</span></span>
|<span data-ttu-id="04089-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04089-127">Property</span></span>|<span data-ttu-id="04089-128">型</span><span class="sxs-lookup"><span data-stu-id="04089-128">Type</span></span>|<span data-ttu-id="04089-129">説明</span><span class="sxs-lookup"><span data-stu-id="04089-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04089-130">id</span><span class="sxs-lookup"><span data-stu-id="04089-130">id</span></span>|<span data-ttu-id="04089-131">String</span><span class="sxs-lookup"><span data-stu-id="04089-131">String</span></span>|<span data-ttu-id="04089-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="04089-132">Key of the entity.</span></span>|
|<span data-ttu-id="04089-133">status</span><span class="sxs-lookup"><span data-stu-id="04089-133">status</span></span>|[<span data-ttu-id="04089-134">actionState</span><span class="sxs-lookup"><span data-stu-id="04089-134">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="04089-135">ワイプアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="04089-135">Wipe action status.</span></span> <span data-ttu-id="04089-136">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="04089-136">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="04089-137">targeteduserid</span><span class="sxs-lookup"><span data-stu-id="04089-137">targetedUserId</span></span>|<span data-ttu-id="04089-138">String</span><span class="sxs-lookup"><span data-stu-id="04089-138">String</span></span>|<span data-ttu-id="04089-139">このワイプアクションの対象となる UserId。</span><span class="sxs-lookup"><span data-stu-id="04089-139">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="04089-140">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="04089-140">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="04089-141">String</span><span class="sxs-lookup"><span data-stu-id="04089-141">String</span></span>|<span data-ttu-id="04089-142">このワイプアクションの対象となる DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="04089-142">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="04089-143">targeteddevicename</span><span class="sxs-lookup"><span data-stu-id="04089-143">targetedDeviceName</span></span>|<span data-ttu-id="04089-144">String</span><span class="sxs-lookup"><span data-stu-id="04089-144">String</span></span>|<span data-ttu-id="04089-145">対象のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="04089-145">Targeted device name.</span></span>|
|<span data-ttu-id="04089-146">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="04089-146">targetedDeviceMacAddress</span></span>|<span data-ttu-id="04089-147">String</span><span class="sxs-lookup"><span data-stu-id="04089-147">String</span></span>|<span data-ttu-id="04089-148">対象デバイスの Mac アドレス。</span><span class="sxs-lookup"><span data-stu-id="04089-148">Targeted device Mac address.</span></span>|
|<span data-ttu-id="04089-149">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="04089-149">lastCheckInDateTime</span></span>|<span data-ttu-id="04089-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04089-150">DateTimeOffset</span></span>|<span data-ttu-id="04089-151">このワイプアクションの対象となったデバイスの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="04089-151">Last checkin time of the device that was targeted by this wipe action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04089-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="04089-152">Relationships</span></span>
<span data-ttu-id="04089-153">なし</span><span class="sxs-lookup"><span data-stu-id="04089-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04089-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04089-154">JSON Representation</span></span>
<span data-ttu-id="04089-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04089-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsInformationProtectionWipeAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionWipeAction",
  "id": "String (identifier)",
  "status": "String",
  "targetedUserId": "String",
  "targetedDeviceRegistrationId": "String",
  "targetedDeviceName": "String",
  "targetedDeviceMacAddress": "String",
  "lastCheckInDateTime": "String (timestamp)"
}
```




