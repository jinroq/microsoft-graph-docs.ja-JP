---
title: windowsinformationprotectionwipepeaction リソースの種類
description: テナント管理者が独自のデバイス (byod) Windows デバイス用に発行したワイプ要求を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 47047f401bbf0a690494490cbbd3b934340a26c9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32558273"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a><span data-ttu-id="dfaeb-103">windowsinformationprotectionwipepeaction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfaeb-103">windowsInformationProtectionWipeAction resource type</span></span>

> <span data-ttu-id="dfaeb-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfaeb-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfaeb-106">テナント管理者が独自のデバイス (byod) Windows デバイス用に発行したワイプ要求を表します。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-106">Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="dfaeb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfaeb-107">Methods</span></span>
|<span data-ttu-id="dfaeb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfaeb-108">Method</span></span>|<span data-ttu-id="dfaeb-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dfaeb-109">Return Type</span></span>|<span data-ttu-id="dfaeb-110">説明</span><span class="sxs-lookup"><span data-stu-id="dfaeb-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dfaeb-111">windowsinformationprotectionwipeactions を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="dfaeb-111">List windowsInformationProtectionWipeActions</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|<span data-ttu-id="dfaeb-112">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dfaeb-112">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) collection</span></span>|<span data-ttu-id="dfaeb-113">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-113">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>|
|[<span data-ttu-id="dfaeb-114">windowsinformationprotectionwipeaction を取得する</span><span class="sxs-lookup"><span data-stu-id="dfaeb-114">Get windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[<span data-ttu-id="dfaeb-115">windowsinformationprotectionwipeaction</span><span class="sxs-lookup"><span data-stu-id="dfaeb-115">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="dfaeb-116">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-116">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="dfaeb-117">windowsinformationprotectionwipeaction を作成する</span><span class="sxs-lookup"><span data-stu-id="dfaeb-117">Create windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[<span data-ttu-id="dfaeb-118">windowsinformationprotectionwipeaction</span><span class="sxs-lookup"><span data-stu-id="dfaeb-118">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="dfaeb-119">新しい[windowsinformationprotectionwipeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-119">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="dfaeb-120">windowsinformationprotectionwipeaction を削除する</span><span class="sxs-lookup"><span data-stu-id="dfaeb-120">Delete windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|<span data-ttu-id="dfaeb-121">なし</span><span class="sxs-lookup"><span data-stu-id="dfaeb-121">None</span></span>|<span data-ttu-id="dfaeb-122">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-122">Deletes a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>|
|[<span data-ttu-id="dfaeb-123">windowsinformationprotectionwipeaction を更新する</span><span class="sxs-lookup"><span data-stu-id="dfaeb-123">Update windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[<span data-ttu-id="dfaeb-124">windowsinformationprotectionwipeaction</span><span class="sxs-lookup"><span data-stu-id="dfaeb-124">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="dfaeb-125">[windowsinformationprotectionwipepeaction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-125">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dfaeb-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfaeb-126">Properties</span></span>
|<span data-ttu-id="dfaeb-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfaeb-127">Property</span></span>|<span data-ttu-id="dfaeb-128">型</span><span class="sxs-lookup"><span data-stu-id="dfaeb-128">Type</span></span>|<span data-ttu-id="dfaeb-129">説明</span><span class="sxs-lookup"><span data-stu-id="dfaeb-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfaeb-130">id</span><span class="sxs-lookup"><span data-stu-id="dfaeb-130">id</span></span>|<span data-ttu-id="dfaeb-131">String</span><span class="sxs-lookup"><span data-stu-id="dfaeb-131">String</span></span>|<span data-ttu-id="dfaeb-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-132">Key of the entity.</span></span>|
|<span data-ttu-id="dfaeb-133">status</span><span class="sxs-lookup"><span data-stu-id="dfaeb-133">status</span></span>|[<span data-ttu-id="dfaeb-134">actionState</span><span class="sxs-lookup"><span data-stu-id="dfaeb-134">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="dfaeb-135">ワイプアクションの状態。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-135">Wipe action status.</span></span> <span data-ttu-id="dfaeb-136">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-136">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="dfaeb-137">targeteduserid</span><span class="sxs-lookup"><span data-stu-id="dfaeb-137">targetedUserId</span></span>|<span data-ttu-id="dfaeb-138">String</span><span class="sxs-lookup"><span data-stu-id="dfaeb-138">String</span></span>|<span data-ttu-id="dfaeb-139">このワイプアクションの対象となる UserId。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-139">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="dfaeb-140">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="dfaeb-140">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="dfaeb-141">String</span><span class="sxs-lookup"><span data-stu-id="dfaeb-141">String</span></span>|<span data-ttu-id="dfaeb-142">このワイプアクションの対象となる DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-142">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="dfaeb-143">targeteddevicename</span><span class="sxs-lookup"><span data-stu-id="dfaeb-143">targetedDeviceName</span></span>|<span data-ttu-id="dfaeb-144">String</span><span class="sxs-lookup"><span data-stu-id="dfaeb-144">String</span></span>|<span data-ttu-id="dfaeb-145">対象のデバイス名。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-145">Targeted device name.</span></span>|
|<span data-ttu-id="dfaeb-146">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="dfaeb-146">targetedDeviceMacAddress</span></span>|<span data-ttu-id="dfaeb-147">String</span><span class="sxs-lookup"><span data-stu-id="dfaeb-147">String</span></span>|<span data-ttu-id="dfaeb-148">対象デバイスの Mac アドレス。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-148">Targeted device Mac address.</span></span>|
|<span data-ttu-id="dfaeb-149">lastCheckInDateTime</span><span class="sxs-lookup"><span data-stu-id="dfaeb-149">lastCheckInDateTime</span></span>|<span data-ttu-id="dfaeb-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfaeb-150">DateTimeOffset</span></span>|<span data-ttu-id="dfaeb-151">このワイプアクションの対象となったデバイスの最終チェックイン時刻。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-151">Last checkin time of the device that was targeted by this wipe action.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfaeb-152">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfaeb-152">Relationships</span></span>
<span data-ttu-id="dfaeb-153">なし</span><span class="sxs-lookup"><span data-stu-id="dfaeb-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dfaeb-154">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfaeb-154">JSON Representation</span></span>
<span data-ttu-id="dfaeb-155">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dfaeb-155">Here is a JSON representation of the resource.</span></span>
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





