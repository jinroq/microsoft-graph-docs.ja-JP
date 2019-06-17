---
title: Windowsinformationprotectionwipepeaction リソースの種類
description: テナント管理者が独自のデバイス (BYOD) Windows デバイス用に発行したワイプ要求を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dccbc89b38abd00a9b464f82cc0531e6fbab47ab
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994399"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a><span data-ttu-id="5828b-103">Windowsinformationprotectionwipepeaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5828b-103">windowsInformationProtectionWipeAction resource type</span></span>

> <span data-ttu-id="5828b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5828b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5828b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5828b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5828b-106">テナント管理者が独自のデバイス (BYOD) Windows デバイス用に発行したワイプ要求を表します。</span><span class="sxs-lookup"><span data-stu-id="5828b-106">Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="5828b-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="5828b-107">Methods</span></span>
|<span data-ttu-id="5828b-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5828b-108">Method</span></span>|<span data-ttu-id="5828b-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5828b-109">Return Type</span></span>|<span data-ttu-id="5828b-110">説明</span><span class="sxs-lookup"><span data-stu-id="5828b-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5828b-111">WindowsInformationProtectionWipeActions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="5828b-111">List windowsInformationProtectionWipeActions</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|<span data-ttu-id="5828b-112">[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5828b-112">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) collection</span></span>|<span data-ttu-id="5828b-113">[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5828b-113">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>|
|[<span data-ttu-id="5828b-114">WindowsInformationProtectionWipeAction を取得する</span><span class="sxs-lookup"><span data-stu-id="5828b-114">Get windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[<span data-ttu-id="5828b-115">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="5828b-115">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="5828b-116">[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5828b-116">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="5828b-117">WindowsInformationProtectionWipeAction を作成する</span><span class="sxs-lookup"><span data-stu-id="5828b-117">Create windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[<span data-ttu-id="5828b-118">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="5828b-118">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="5828b-119">新しい[Windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5828b-119">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="5828b-120">WindowsInformationProtectionWipeAction を削除する</span><span class="sxs-lookup"><span data-stu-id="5828b-120">Delete windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|<span data-ttu-id="5828b-121">None</span><span class="sxs-lookup"><span data-stu-id="5828b-121">None</span></span>|<span data-ttu-id="5828b-122">[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5828b-122">Deletes a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>|
|[<span data-ttu-id="5828b-123">WindowsInformationProtectionWipeAction を更新する</span><span class="sxs-lookup"><span data-stu-id="5828b-123">Update windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[<span data-ttu-id="5828b-124">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="5828b-124">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="5828b-125">[Windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5828b-125">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5828b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5828b-126">Properties</span></span>
|<span data-ttu-id="5828b-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5828b-127">Property</span></span>|<span data-ttu-id="5828b-128">型</span><span class="sxs-lookup"><span data-stu-id="5828b-128">Type</span></span>|<span data-ttu-id="5828b-129">説明</span><span class="sxs-lookup"><span data-stu-id="5828b-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5828b-130">id</span><span class="sxs-lookup"><span data-stu-id="5828b-130">id</span></span>|<span data-ttu-id="5828b-131">String</span><span class="sxs-lookup"><span data-stu-id="5828b-131">String</span></span>|<span data-ttu-id="5828b-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5828b-132">Key of the entity.</span></span>|
|<span data-ttu-id="5828b-133">status</span><span class="sxs-lookup"><span data-stu-id="5828b-133">status</span></span>|[<span data-ttu-id="5828b-134">actionState</span><span class="sxs-lookup"><span data-stu-id="5828b-134">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="5828b-135">ワイプアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="5828b-135">Wipe action status.</span></span> <span data-ttu-id="5828b-136">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="5828b-136">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="5828b-137">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="5828b-137">targetedUserId</span></span>|<span data-ttu-id="5828b-138">String</span><span class="sxs-lookup"><span data-stu-id="5828b-138">String</span></span>|<span data-ttu-id="5828b-139">このワイプアクションの対象となる UserId。</span><span class="sxs-lookup"><span data-stu-id="5828b-139">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="5828b-140">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="5828b-140">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="5828b-141">String</span><span class="sxs-lookup"><span data-stu-id="5828b-141">String</span></span>|<span data-ttu-id="5828b-142">このワイプアクションの対象となる DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="5828b-142">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="5828b-143">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="5828b-143">targetedDeviceName</span></span>|<span data-ttu-id="5828b-144">String</span><span class="sxs-lookup"><span data-stu-id="5828b-144">String</span></span>|<span data-ttu-id="5828b-145">対象のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="5828b-145">Targeted device name.</span></span>|
|<span data-ttu-id="5828b-146">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="5828b-146">targetedDeviceMacAddress</span></span>|<span data-ttu-id="5828b-147">String</span><span class="sxs-lookup"><span data-stu-id="5828b-147">String</span></span>|<span data-ttu-id="5828b-148">対象デバイスの Mac アドレス。</span><span class="sxs-lookup"><span data-stu-id="5828b-148">Targeted device Mac address.</span></span>|
|<span data-ttu-id="5828b-149">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="5828b-149">lastCheckInDateTime</span></span>|<span data-ttu-id="5828b-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5828b-150">DateTimeOffset</span></span>|<span data-ttu-id="5828b-151">このワイプアクションの対象となったデバイスの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="5828b-151">Last checkin time of the device that was targeted by this wipe action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5828b-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5828b-152">Relationships</span></span>
<span data-ttu-id="5828b-153">なし</span><span class="sxs-lookup"><span data-stu-id="5828b-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5828b-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5828b-154">JSON Representation</span></span>
<span data-ttu-id="5828b-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5828b-155">Here is a JSON representation of the resource.</span></span>
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





