---
title: importedDeviceIdentity リソースの種類
description: importedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d7cc903fa1b30177f037493fe090ebfde31831b0
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771944"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="cb9ff-103">importedDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb9ff-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="cb9ff-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cb9ff-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cb9ff-106">importedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="cb9ff-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="cb9ff-107">Methods</span></span>
|<span data-ttu-id="cb9ff-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cb9ff-108">Method</span></span>|<span data-ttu-id="cb9ff-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cb9ff-109">Return Type</span></span>|<span data-ttu-id="cb9ff-110">説明</span><span class="sxs-lookup"><span data-stu-id="cb9ff-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cb9ff-111">リスト importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="cb9ff-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="cb9ff-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cb9ff-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="cb9ff-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="cb9ff-114">importedDeviceIdentity を取得する</span><span class="sxs-lookup"><span data-stu-id="cb9ff-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="cb9ff-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="cb9ff-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="cb9ff-116">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="cb9ff-117">importedDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="cb9ff-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="cb9ff-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="cb9ff-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="cb9ff-119">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="cb9ff-120">importedDeviceIdentity の削除</span><span class="sxs-lookup"><span data-stu-id="cb9ff-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="cb9ff-121">なし</span><span class="sxs-lookup"><span data-stu-id="cb9ff-121">None</span></span>|<span data-ttu-id="cb9ff-122">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="cb9ff-123">importedDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="cb9ff-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="cb9ff-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="cb9ff-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="cb9ff-125">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="cb9ff-126">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="cb9ff-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="cb9ff-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cb9ff-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="cb9ff-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cb9ff-128">Not yet documented</span></span>|
|[<span data-ttu-id="cb9ff-129">searchExistingIdentities アクション</span><span class="sxs-lookup"><span data-stu-id="cb9ff-129">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="cb9ff-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cb9ff-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="cb9ff-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cb9ff-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cb9ff-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb9ff-132">Properties</span></span>
|<span data-ttu-id="cb9ff-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb9ff-133">Property</span></span>|<span data-ttu-id="cb9ff-134">型</span><span class="sxs-lookup"><span data-stu-id="cb9ff-134">Type</span></span>|<span data-ttu-id="cb9ff-135">説明</span><span class="sxs-lookup"><span data-stu-id="cb9ff-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb9ff-136">id</span><span class="sxs-lookup"><span data-stu-id="cb9ff-136">id</span></span>|<span data-ttu-id="cb9ff-137">String</span><span class="sxs-lookup"><span data-stu-id="cb9ff-137">String</span></span>|<span data-ttu-id="cb9ff-138">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="cb9ff-138">Id of the imported device identity</span></span>|
|<span data-ttu-id="cb9ff-139">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cb9ff-139">importedDeviceIdentifier</span></span>|<span data-ttu-id="cb9ff-140">文字列</span><span class="sxs-lookup"><span data-stu-id="cb9ff-140">String</span></span>|<span data-ttu-id="cb9ff-141">インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="cb9ff-141">Imported Device Identifier</span></span>|
|<span data-ttu-id="cb9ff-142">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="cb9ff-142">importedDeviceIdentityType</span></span>|[<span data-ttu-id="cb9ff-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="cb9ff-143">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="cb9ff-144">インポートされたデバイス id の種類。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-144">Type of Imported Device Identity.</span></span> <span data-ttu-id="cb9ff-145">使用可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-145">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="cb9ff-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb9ff-146">lastModifiedDateTime</span></span>|<span data-ttu-id="cb9ff-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb9ff-147">DateTimeOffset</span></span>|<span data-ttu-id="cb9ff-148">説明の最終更新日時</span><span class="sxs-lookup"><span data-stu-id="cb9ff-148">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="cb9ff-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cb9ff-149">createdDateTime</span></span>|<span data-ttu-id="cb9ff-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb9ff-150">DateTimeOffset</span></span>|<span data-ttu-id="cb9ff-151">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="cb9ff-151">Created Date Time of the device</span></span>|
|<span data-ttu-id="cb9ff-152">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="cb9ff-152">lastContactedDateTime</span></span>|<span data-ttu-id="cb9ff-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cb9ff-153">DateTimeOffset</span></span>|<span data-ttu-id="cb9ff-154">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="cb9ff-154">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="cb9ff-155">説明</span><span class="sxs-lookup"><span data-stu-id="cb9ff-155">description</span></span>|<span data-ttu-id="cb9ff-156">String</span><span class="sxs-lookup"><span data-stu-id="cb9ff-156">String</span></span>|<span data-ttu-id="cb9ff-157">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="cb9ff-157">The description of the device</span></span>|
|<span data-ttu-id="cb9ff-158">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="cb9ff-158">enrollmentState</span></span>|[<span data-ttu-id="cb9ff-159">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="cb9ff-159">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="cb9ff-160">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-160">The state of the device in Intune.</span></span> <span data-ttu-id="cb9ff-161">可能な値は `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-161">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="cb9ff-162">platform</span><span class="sxs-lookup"><span data-stu-id="cb9ff-162">platform</span></span>|[<span data-ttu-id="cb9ff-163">platform</span><span class="sxs-lookup"><span data-stu-id="cb9ff-163">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="cb9ff-164">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-164">The platform of the Device.</span></span> <span data-ttu-id="cb9ff-165">可能な値は `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS` です。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-165">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb9ff-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cb9ff-166">Relationships</span></span>
<span data-ttu-id="cb9ff-167">なし</span><span class="sxs-lookup"><span data-stu-id="cb9ff-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cb9ff-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb9ff-168">JSON Representation</span></span>
<span data-ttu-id="cb9ff-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cb9ff-169">Here is a JSON representation of the resource.</span></span>
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





