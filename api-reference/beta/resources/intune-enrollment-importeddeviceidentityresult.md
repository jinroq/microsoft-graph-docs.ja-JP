---
title: importedDeviceIdentityResult リソースの種類
description: ImportedDeviceIdentityResult リソースは、デバイス id のインポートを試行した結果を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9bdac4b02fd009705ef79acff5656b00c660e9ef
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327907"
---
# <a name="importeddeviceidentityresult-resource-type"></a><span data-ttu-id="75509-103">importedDeviceIdentityResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75509-103">importedDeviceIdentityResult resource type</span></span>

> <span data-ttu-id="75509-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75509-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75509-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75509-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75509-106">ImportedDeviceIdentityResult リソースは、デバイス id のインポートを試行した結果を表します。</span><span class="sxs-lookup"><span data-stu-id="75509-106">The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.</span></span>


<span data-ttu-id="75509-107">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="75509-107">Inherits from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>

## <a name="methods"></a><span data-ttu-id="75509-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="75509-108">Methods</span></span>
|<span data-ttu-id="75509-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="75509-109">Method</span></span>|<span data-ttu-id="75509-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="75509-110">Return Type</span></span>|<span data-ttu-id="75509-111">説明</span><span class="sxs-lookup"><span data-stu-id="75509-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75509-112">リスト importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="75509-112">List importedDeviceIdentityResults</span></span>](../api/intune-enrollment-importeddeviceidentityresult-list.md)|<span data-ttu-id="75509-113">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="75509-113">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="75509-114">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="75509-114">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>|
|[<span data-ttu-id="75509-115">ImportedDeviceIdentityResult を取得する</span><span class="sxs-lookup"><span data-stu-id="75509-115">Get importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[<span data-ttu-id="75509-116">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="75509-116">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="75509-117">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75509-117">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="75509-118">ImportedDeviceIdentityResult を作成する</span><span class="sxs-lookup"><span data-stu-id="75509-118">Create importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[<span data-ttu-id="75509-119">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="75509-119">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="75509-120">新しい[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="75509-120">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="75509-121">ImportedDeviceIdentityResult の削除</span><span class="sxs-lookup"><span data-stu-id="75509-121">Delete importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|<span data-ttu-id="75509-122">None</span><span class="sxs-lookup"><span data-stu-id="75509-122">None</span></span>|<span data-ttu-id="75509-123">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="75509-123">Deletes a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>|
|[<span data-ttu-id="75509-124">ImportedDeviceIdentityResult の更新</span><span class="sxs-lookup"><span data-stu-id="75509-124">Update importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[<span data-ttu-id="75509-125">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="75509-125">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="75509-126">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="75509-126">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75509-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75509-127">Properties</span></span>
|<span data-ttu-id="75509-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75509-128">Property</span></span>|<span data-ttu-id="75509-129">型</span><span class="sxs-lookup"><span data-stu-id="75509-129">Type</span></span>|<span data-ttu-id="75509-130">説明</span><span class="sxs-lookup"><span data-stu-id="75509-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75509-131">id</span><span class="sxs-lookup"><span data-stu-id="75509-131">id</span></span>|<span data-ttu-id="75509-132">String</span><span class="sxs-lookup"><span data-stu-id="75509-132">String</span></span>|<span data-ttu-id="75509-133">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="75509-133">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75509-134">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="75509-134">importedDeviceIdentifier</span></span>|<span data-ttu-id="75509-135">String</span><span class="sxs-lookup"><span data-stu-id="75509-135">String</span></span>|<span data-ttu-id="75509-136">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="75509-136">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75509-137">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="75509-137">importedDeviceIdentityType</span></span>|[<span data-ttu-id="75509-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="75509-138">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="75509-139">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された、インポートされたデバイス id の種類。</span><span class="sxs-lookup"><span data-stu-id="75509-139">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="75509-140">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="75509-140">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="75509-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75509-141">lastModifiedDateTime</span></span>|<span data-ttu-id="75509-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75509-142">DateTimeOffset</span></span>|<span data-ttu-id="75509-143">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された説明の最終更新日時。</span><span class="sxs-lookup"><span data-stu-id="75509-143">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75509-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75509-144">createdDateTime</span></span>|<span data-ttu-id="75509-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75509-145">DateTimeOffset</span></span>|<span data-ttu-id="75509-146">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="75509-146">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75509-147">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="75509-147">lastContactedDateTime</span></span>|<span data-ttu-id="75509-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75509-148">DateTimeOffset</span></span>|<span data-ttu-id="75509-149">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの最後の連絡日時。</span><span class="sxs-lookup"><span data-stu-id="75509-149">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75509-150">description</span><span class="sxs-lookup"><span data-stu-id="75509-150">description</span></span>|<span data-ttu-id="75509-151">String</span><span class="sxs-lookup"><span data-stu-id="75509-151">String</span></span>|<span data-ttu-id="75509-152">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されたデバイスの説明</span><span class="sxs-lookup"><span data-stu-id="75509-152">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="75509-153">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="75509-153">enrollmentState</span></span>|[<span data-ttu-id="75509-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="75509-154">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="75509-155">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承された Intune のデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="75509-155">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="75509-156">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="75509-156">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="75509-157">platform</span><span class="sxs-lookup"><span data-stu-id="75509-157">platform</span></span>|[<span data-ttu-id="75509-158">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="75509-158">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="75509-159">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="75509-159">The platform of the Device.</span></span> <span data-ttu-id="75509-160">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="75509-160">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="75509-161">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="75509-161">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="75509-162">status</span><span class="sxs-lookup"><span data-stu-id="75509-162">status</span></span>|<span data-ttu-id="75509-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="75509-163">Boolean</span></span>|<span data-ttu-id="75509-164">インポートされたデバイス id の状態</span><span class="sxs-lookup"><span data-stu-id="75509-164">Status of imported device identity</span></span>|

## <a name="relationships"></a><span data-ttu-id="75509-165">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75509-165">Relationships</span></span>
<span data-ttu-id="75509-166">なし</span><span class="sxs-lookup"><span data-stu-id="75509-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75509-167">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75509-167">JSON Representation</span></span>
<span data-ttu-id="75509-168">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75509-168">Here is a JSON representation of the resource.</span></span>
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



