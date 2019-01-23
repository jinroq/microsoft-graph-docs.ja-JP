---
title: windowsInformationProtectionWipeAction リソースの種類
description: 表しますは、Bring-Your-Own-Device(BYOD) Windows デバイス用のテナント管理者によって発行された要求を拭きます。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67af8bdde412381bb6362ef1768dca12fdfce6c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431655"
---
# <a name="windowsinformationprotectionwipeaction-resource-type"></a><span data-ttu-id="c4570-103">windowsInformationProtectionWipeAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c4570-103">windowsInformationProtectionWipeAction resource type</span></span>

> <span data-ttu-id="c4570-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c4570-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c4570-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c4570-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c4570-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c4570-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4570-107">表しますは、Bring-Your-Own-Device(BYOD) Windows デバイス用のテナント管理者によって発行された要求を拭きます。</span><span class="sxs-lookup"><span data-stu-id="c4570-107">Represents wipe requests issued by tenant admin for Bring-Your-Own-Device(BYOD) Windows devices.</span></span>

## <a name="methods"></a><span data-ttu-id="c4570-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c4570-108">Methods</span></span>
|<span data-ttu-id="c4570-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="c4570-109">Method</span></span>|<span data-ttu-id="c4570-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c4570-110">Return Type</span></span>|<span data-ttu-id="c4570-111">説明</span><span class="sxs-lookup"><span data-stu-id="c4570-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c4570-112">リスト windowsInformationProtectionWipeActions</span><span class="sxs-lookup"><span data-stu-id="c4570-112">List windowsInformationProtectionWipeActions</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-list.md)|<span data-ttu-id="c4570-113">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c4570-113">[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) collection</span></span>|<span data-ttu-id="c4570-114">[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="c4570-114">List properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) objects.</span></span>|
|[<span data-ttu-id="c4570-115">WindowsInformationProtectionWipeAction を取得します。</span><span class="sxs-lookup"><span data-stu-id="c4570-115">Get windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-get.md)|[<span data-ttu-id="c4570-116">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="c4570-116">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="c4570-117">[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c4570-117">Read properties and relationships of the [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="c4570-118">WindowsInformationProtectionWipeAction を作成します。</span><span class="sxs-lookup"><span data-stu-id="c4570-118">Create windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-create.md)|[<span data-ttu-id="c4570-119">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="c4570-119">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="c4570-120">新しい[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="c4570-120">Create a new [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|
|[<span data-ttu-id="c4570-121">WindowsInformationProtectionWipeAction を削除します。</span><span class="sxs-lookup"><span data-stu-id="c4570-121">Delete windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-delete.md)|<span data-ttu-id="c4570-122">なし</span><span class="sxs-lookup"><span data-stu-id="c4570-122">None</span></span>|<span data-ttu-id="c4570-123">の[windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="c4570-123">Deletes a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md).</span></span>|
|[<span data-ttu-id="c4570-124">WindowsInformationProtectionWipeAction を更新します。</span><span class="sxs-lookup"><span data-stu-id="c4570-124">Update windowsInformationProtectionWipeAction</span></span>](../api/intune-mam-windowsinformationprotectionwipeaction-update.md)|[<span data-ttu-id="c4570-125">windowsInformationProtectionWipeAction</span><span class="sxs-lookup"><span data-stu-id="c4570-125">windowsInformationProtectionWipeAction</span></span>](../resources/intune-mam-windowsinformationprotectionwipeaction.md)|<span data-ttu-id="c4570-126">[WindowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c4570-126">Update the properties of a [windowsInformationProtectionWipeAction](../resources/intune-mam-windowsinformationprotectionwipeaction.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c4570-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4570-127">Properties</span></span>
|<span data-ttu-id="c4570-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c4570-128">Property</span></span>|<span data-ttu-id="c4570-129">型</span><span class="sxs-lookup"><span data-stu-id="c4570-129">Type</span></span>|<span data-ttu-id="c4570-130">説明</span><span class="sxs-lookup"><span data-stu-id="c4570-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4570-131">id</span><span class="sxs-lookup"><span data-stu-id="c4570-131">id</span></span>|<span data-ttu-id="c4570-132">String</span><span class="sxs-lookup"><span data-stu-id="c4570-132">String</span></span>|<span data-ttu-id="c4570-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c4570-133">Key of the entity.</span></span>|
|<span data-ttu-id="c4570-134">status</span><span class="sxs-lookup"><span data-stu-id="c4570-134">status</span></span>|[<span data-ttu-id="c4570-135">actionState</span><span class="sxs-lookup"><span data-stu-id="c4570-135">actionState</span></span>](../resources/intune-shared-actionstate.md)|<span data-ttu-id="c4570-136">アクションのステータスを消去します。</span><span class="sxs-lookup"><span data-stu-id="c4570-136">Wipe action status.</span></span> <span data-ttu-id="c4570-137">可能な値は、`none`、`pending`、`canceled`、`active`、`done`、`failed`、`notSupported` です。</span><span class="sxs-lookup"><span data-stu-id="c4570-137">Possible values are: `none`, `pending`, `canceled`, `active`, `done`, `failed`, `notSupported`.</span></span>|
|<span data-ttu-id="c4570-138">targetedUserId</span><span class="sxs-lookup"><span data-stu-id="c4570-138">targetedUserId</span></span>|<span data-ttu-id="c4570-139">String</span><span class="sxs-lookup"><span data-stu-id="c4570-139">String</span></span>|<span data-ttu-id="c4570-140">このワイプ操作のターゲットとなるユーザーの Id。</span><span class="sxs-lookup"><span data-stu-id="c4570-140">The UserId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="c4570-141">targetedDeviceRegistrationId</span><span class="sxs-lookup"><span data-stu-id="c4570-141">targetedDeviceRegistrationId</span></span>|<span data-ttu-id="c4570-142">String</span><span class="sxs-lookup"><span data-stu-id="c4570-142">String</span></span>|<span data-ttu-id="c4570-143">このワイプ操作のターゲットとなる DeviceRegistrationId。</span><span class="sxs-lookup"><span data-stu-id="c4570-143">The DeviceRegistrationId being targeted by this wipe action.</span></span>|
|<span data-ttu-id="c4570-144">targetedDeviceName</span><span class="sxs-lookup"><span data-stu-id="c4570-144">targetedDeviceName</span></span>|<span data-ttu-id="c4570-145">String</span><span class="sxs-lookup"><span data-stu-id="c4570-145">String</span></span>|<span data-ttu-id="c4570-146">ターゲット ・ デバイスの名前です。</span><span class="sxs-lookup"><span data-stu-id="c4570-146">Targeted device name.</span></span>|
|<span data-ttu-id="c4570-147">targetedDeviceMacAddress</span><span class="sxs-lookup"><span data-stu-id="c4570-147">targetedDeviceMacAddress</span></span>|<span data-ttu-id="c4570-148">String</span><span class="sxs-lookup"><span data-stu-id="c4570-148">String</span></span>|<span data-ttu-id="c4570-149">ターゲット デバイスの Mac アドレスです。</span><span class="sxs-lookup"><span data-stu-id="c4570-149">Targeted device Mac address.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c4570-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c4570-150">Relationships</span></span>
<span data-ttu-id="c4570-151">なし</span><span class="sxs-lookup"><span data-stu-id="c4570-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c4570-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c4570-152">JSON Representation</span></span>
<span data-ttu-id="c4570-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c4570-153">Here is a JSON representation of the resource.</span></span>
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
  "targetedDeviceMacAddress": "String"
}
```




