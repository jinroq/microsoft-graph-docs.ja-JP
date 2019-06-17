---
title: importedDeviceIdentity リソースの種類
description: ImportedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 45af3e68fc5d19af08a822962eb5333ce4a98655
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34992627"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="8c037-103">importedDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8c037-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="8c037-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c037-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c037-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c037-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c037-106">ImportedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。</span><span class="sxs-lookup"><span data-stu-id="8c037-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="8c037-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c037-107">Methods</span></span>
|<span data-ttu-id="8c037-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8c037-108">Method</span></span>|<span data-ttu-id="8c037-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8c037-109">Return Type</span></span>|<span data-ttu-id="8c037-110">説明</span><span class="sxs-lookup"><span data-stu-id="8c037-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c037-111">リスト importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="8c037-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="8c037-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8c037-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="8c037-113">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8c037-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="8c037-114">ImportedDeviceIdentity を取得する</span><span class="sxs-lookup"><span data-stu-id="8c037-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="8c037-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8c037-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="8c037-116">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="8c037-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="8c037-117">ImportedDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="8c037-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="8c037-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8c037-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="8c037-119">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8c037-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="8c037-120">ImportedDeviceIdentity の削除</span><span class="sxs-lookup"><span data-stu-id="8c037-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="8c037-121">None</span><span class="sxs-lookup"><span data-stu-id="8c037-121">None</span></span>|<span data-ttu-id="8c037-122">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="8c037-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="8c037-123">ImportedDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="8c037-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="8c037-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="8c037-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="8c037-125">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8c037-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="8c037-126">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="8c037-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="8c037-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8c037-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="8c037-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8c037-128">Not yet documented</span></span>|
|[<span data-ttu-id="8c037-129">searchExistingIdentities アクション</span><span class="sxs-lookup"><span data-stu-id="8c037-129">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="8c037-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8c037-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="8c037-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="8c037-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="8c037-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c037-132">Properties</span></span>
|<span data-ttu-id="8c037-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8c037-133">Property</span></span>|<span data-ttu-id="8c037-134">型</span><span class="sxs-lookup"><span data-stu-id="8c037-134">Type</span></span>|<span data-ttu-id="8c037-135">説明</span><span class="sxs-lookup"><span data-stu-id="8c037-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c037-136">id</span><span class="sxs-lookup"><span data-stu-id="8c037-136">id</span></span>|<span data-ttu-id="8c037-137">String</span><span class="sxs-lookup"><span data-stu-id="8c037-137">String</span></span>|<span data-ttu-id="8c037-138">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="8c037-138">Id of the imported device identity</span></span>|
|<span data-ttu-id="8c037-139">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="8c037-139">importedDeviceIdentifier</span></span>|<span data-ttu-id="8c037-140">String</span><span class="sxs-lookup"><span data-stu-id="8c037-140">String</span></span>|<span data-ttu-id="8c037-141">インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="8c037-141">Imported Device Identifier</span></span>|
|<span data-ttu-id="8c037-142">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="8c037-142">importedDeviceIdentityType</span></span>|[<span data-ttu-id="8c037-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="8c037-143">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="8c037-144">インポートされたデバイス Id の種類。</span><span class="sxs-lookup"><span data-stu-id="8c037-144">Type of Imported Device Identity.</span></span> <span data-ttu-id="8c037-145">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="8c037-145">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="8c037-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c037-146">lastModifiedDateTime</span></span>|<span data-ttu-id="8c037-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c037-147">DateTimeOffset</span></span>|<span data-ttu-id="8c037-148">説明の最終更新日時</span><span class="sxs-lookup"><span data-stu-id="8c037-148">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="8c037-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8c037-149">createdDateTime</span></span>|<span data-ttu-id="8c037-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c037-150">DateTimeOffset</span></span>|<span data-ttu-id="8c037-151">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="8c037-151">Created Date Time of the device</span></span>|
|<span data-ttu-id="8c037-152">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="8c037-152">lastContactedDateTime</span></span>|<span data-ttu-id="8c037-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8c037-153">DateTimeOffset</span></span>|<span data-ttu-id="8c037-154">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="8c037-154">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="8c037-155">description</span><span class="sxs-lookup"><span data-stu-id="8c037-155">description</span></span>|<span data-ttu-id="8c037-156">String</span><span class="sxs-lookup"><span data-stu-id="8c037-156">String</span></span>|<span data-ttu-id="8c037-157">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="8c037-157">The description of the device</span></span>|
|<span data-ttu-id="8c037-158">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="8c037-158">enrollmentState</span></span>|[<span data-ttu-id="8c037-159">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="8c037-159">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="8c037-160">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="8c037-160">The state of the device in Intune.</span></span> <span data-ttu-id="8c037-161">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="8c037-161">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="8c037-162">platform</span><span class="sxs-lookup"><span data-stu-id="8c037-162">platform</span></span>|[<span data-ttu-id="8c037-163">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="8c037-163">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="8c037-164">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="8c037-164">The platform of the Device.</span></span> <span data-ttu-id="8c037-165">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="8c037-165">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c037-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8c037-166">Relationships</span></span>
<span data-ttu-id="8c037-167">なし</span><span class="sxs-lookup"><span data-stu-id="8c037-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c037-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8c037-168">JSON Representation</span></span>
<span data-ttu-id="8c037-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8c037-169">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.importedDeviceIdentity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.importedDeviceIdentity",
  "id": "String (identifier)",
  "importedDeviceIdentifier": "String",
  "importedDeviceIdentityType": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "lastContactedDateTime": "String (timestamp)",
  "description": "String",
  "enrollmentState": "String",
  "platform": "String"
}
```





