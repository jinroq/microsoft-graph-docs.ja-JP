---
title: importedDeviceIdentityResult リソースの種類
description: importedDeviceIdentityResult リソースは、デバイス id のインポートを試行した結果を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b94eff5ea5e2ed37173341b45980e9b60437822d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32524499"
---
# <a name="importeddeviceidentityresult-resource-type"></a><span data-ttu-id="7e7b4-103">importedDeviceIdentityResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7e7b4-103">importedDeviceIdentityResult resource type</span></span>

> <span data-ttu-id="7e7b4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e7b4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e7b4-106">importedDeviceIdentityResult リソースは、デバイス id のインポートを試行した結果を表します。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-106">The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.</span></span>


<span data-ttu-id="7e7b4-107">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-107">Inherits from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>

## <a name="methods"></a><span data-ttu-id="7e7b4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e7b4-108">Methods</span></span>
|<span data-ttu-id="7e7b4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="7e7b4-109">Method</span></span>|<span data-ttu-id="7e7b4-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="7e7b4-110">Return Type</span></span>|<span data-ttu-id="7e7b4-111">説明</span><span class="sxs-lookup"><span data-stu-id="7e7b4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7e7b4-112">リスト importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="7e7b4-112">List importedDeviceIdentityResults</span></span>](../api/intune-enrollment-importeddeviceidentityresult-list.md)|<span data-ttu-id="7e7b4-113">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7e7b4-113">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="7e7b4-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-114">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>|
|[<span data-ttu-id="7e7b4-115">importedDeviceIdentityResult を取得する</span><span class="sxs-lookup"><span data-stu-id="7e7b4-115">Get importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[<span data-ttu-id="7e7b4-116">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="7e7b4-116">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="7e7b4-117">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-117">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="7e7b4-118">importedDeviceIdentityResult を作成する</span><span class="sxs-lookup"><span data-stu-id="7e7b4-118">Create importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[<span data-ttu-id="7e7b4-119">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="7e7b4-119">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="7e7b4-120">新しい[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-120">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="7e7b4-121">importedDeviceIdentityResult の削除</span><span class="sxs-lookup"><span data-stu-id="7e7b4-121">Delete importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|<span data-ttu-id="7e7b4-122">なし</span><span class="sxs-lookup"><span data-stu-id="7e7b4-122">None</span></span>|<span data-ttu-id="7e7b4-123">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-123">Deletes a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>|
|[<span data-ttu-id="7e7b4-124">importedDeviceIdentityResult の更新</span><span class="sxs-lookup"><span data-stu-id="7e7b4-124">Update importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[<span data-ttu-id="7e7b4-125">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="7e7b4-125">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="7e7b4-126">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-126">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7e7b4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e7b4-127">Properties</span></span>
|<span data-ttu-id="7e7b4-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7e7b4-128">Property</span></span>|<span data-ttu-id="7e7b4-129">型</span><span class="sxs-lookup"><span data-stu-id="7e7b4-129">Type</span></span>|<span data-ttu-id="7e7b4-130">説明</span><span class="sxs-lookup"><span data-stu-id="7e7b4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e7b4-131">id</span><span class="sxs-lookup"><span data-stu-id="7e7b4-131">id</span></span>|<span data-ttu-id="7e7b4-132">String</span><span class="sxs-lookup"><span data-stu-id="7e7b4-132">String</span></span>|<span data-ttu-id="7e7b4-133">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="7e7b4-133">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7e7b4-134">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="7e7b4-134">importedDeviceIdentifier</span></span>|<span data-ttu-id="7e7b4-135">String</span><span class="sxs-lookup"><span data-stu-id="7e7b4-135">String</span></span>|<span data-ttu-id="7e7b4-136">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="7e7b4-136">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7e7b4-137">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="7e7b4-137">importedDeviceIdentityType</span></span>|[<span data-ttu-id="7e7b4-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="7e7b4-138">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="7e7b4-139">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス id の種類。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-139">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7e7b4-140">使用可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-140">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="7e7b4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e7b4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="7e7b4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e7b4-142">DateTimeOffset</span></span>|<span data-ttu-id="7e7b4-143">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された説明の最終更新日時。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-143">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7e7b4-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7e7b4-144">createdDateTime</span></span>|<span data-ttu-id="7e7b4-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e7b4-145">DateTimeOffset</span></span>|<span data-ttu-id="7e7b4-146">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="7e7b4-146">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7e7b4-147">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="7e7b4-147">lastContactedDateTime</span></span>|<span data-ttu-id="7e7b4-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e7b4-148">DateTimeOffset</span></span>|<span data-ttu-id="7e7b4-149">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの最後の連絡日時。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-149">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7e7b4-150">description</span><span class="sxs-lookup"><span data-stu-id="7e7b4-150">description</span></span>|<span data-ttu-id="7e7b4-151">String</span><span class="sxs-lookup"><span data-stu-id="7e7b4-151">String</span></span>|<span data-ttu-id="7e7b4-152">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの説明</span><span class="sxs-lookup"><span data-stu-id="7e7b4-152">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="7e7b4-153">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7e7b4-153">enrollmentState</span></span>|[<span data-ttu-id="7e7b4-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="7e7b4-154">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="7e7b4-155">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された Intune のデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-155">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7e7b4-156">可能な値は `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-156">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="7e7b4-157">platform</span><span class="sxs-lookup"><span data-stu-id="7e7b4-157">platform</span></span>|[<span data-ttu-id="7e7b4-158">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="7e7b4-158">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="7e7b4-159">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-159">The platform of the Device.</span></span> <span data-ttu-id="7e7b4-160">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-160">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="7e7b4-161">可能な値は `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS` です。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="7e7b4-162">status</span><span class="sxs-lookup"><span data-stu-id="7e7b4-162">status</span></span>|<span data-ttu-id="7e7b4-163">ブール値</span><span class="sxs-lookup"><span data-stu-id="7e7b4-163">Boolean</span></span>|<span data-ttu-id="7e7b4-164">インポートされたデバイス id の状態</span><span class="sxs-lookup"><span data-stu-id="7e7b4-164">Status of imported device identity</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e7b4-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="7e7b4-165">Relationships</span></span>
<span data-ttu-id="7e7b4-166">なし</span><span class="sxs-lookup"><span data-stu-id="7e7b4-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e7b4-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7e7b4-167">JSON Representation</span></span>
<span data-ttu-id="7e7b4-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="7e7b4-168">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentityResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentityResult",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String",
  "status": true
}
```





