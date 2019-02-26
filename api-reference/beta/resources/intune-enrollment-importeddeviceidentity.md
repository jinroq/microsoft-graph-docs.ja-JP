---
title: importedDeviceIdentity リソースの種類
description: importedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c7ef77b550060d5544a6ee0eda4e6b11923d3571
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151227"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="3869f-103">importedDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3869f-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="3869f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3869f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3869f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3869f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3869f-106">importedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。</span><span class="sxs-lookup"><span data-stu-id="3869f-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="3869f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="3869f-107">Methods</span></span>
|<span data-ttu-id="3869f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="3869f-108">Method</span></span>|<span data-ttu-id="3869f-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3869f-109">Return Type</span></span>|<span data-ttu-id="3869f-110">説明</span><span class="sxs-lookup"><span data-stu-id="3869f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3869f-111">リスト importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="3869f-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="3869f-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3869f-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="3869f-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3869f-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="3869f-114">importedDeviceIdentity を取得する</span><span class="sxs-lookup"><span data-stu-id="3869f-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="3869f-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3869f-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="3869f-116">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3869f-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="3869f-117">importedDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="3869f-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="3869f-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3869f-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="3869f-119">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3869f-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="3869f-120">importedDeviceIdentity の削除</span><span class="sxs-lookup"><span data-stu-id="3869f-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="3869f-121">なし</span><span class="sxs-lookup"><span data-stu-id="3869f-121">None</span></span>|<span data-ttu-id="3869f-122">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="3869f-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="3869f-123">importedDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="3869f-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="3869f-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="3869f-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="3869f-125">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3869f-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="3869f-126">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="3869f-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="3869f-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="3869f-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="3869f-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="3869f-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="3869f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3869f-129">Properties</span></span>
|<span data-ttu-id="3869f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3869f-130">Property</span></span>|<span data-ttu-id="3869f-131">型</span><span class="sxs-lookup"><span data-stu-id="3869f-131">Type</span></span>|<span data-ttu-id="3869f-132">説明</span><span class="sxs-lookup"><span data-stu-id="3869f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3869f-133">id</span><span class="sxs-lookup"><span data-stu-id="3869f-133">id</span></span>|<span data-ttu-id="3869f-134">文字列</span><span class="sxs-lookup"><span data-stu-id="3869f-134">String</span></span>|<span data-ttu-id="3869f-135">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="3869f-135">Id of the imported device identity</span></span>|
|<span data-ttu-id="3869f-136">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3869f-136">importedDeviceIdentifier</span></span>|<span data-ttu-id="3869f-137">String</span><span class="sxs-lookup"><span data-stu-id="3869f-137">String</span></span>|<span data-ttu-id="3869f-138">インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="3869f-138">Imported Device Identifier</span></span>|
|<span data-ttu-id="3869f-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="3869f-139">importedDeviceIdentityType</span></span>|[<span data-ttu-id="3869f-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="3869f-140">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="3869f-141">インポートされたデバイス id の種類。</span><span class="sxs-lookup"><span data-stu-id="3869f-141">Type of Imported Device Identity.</span></span> <span data-ttu-id="3869f-142">可能な値は `unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="3869f-142">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="3869f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3869f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="3869f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3869f-144">DateTimeOffset</span></span>|<span data-ttu-id="3869f-145">説明の最終更新日時</span><span class="sxs-lookup"><span data-stu-id="3869f-145">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="3869f-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3869f-146">createdDateTime</span></span>|<span data-ttu-id="3869f-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3869f-147">DateTimeOffset</span></span>|<span data-ttu-id="3869f-148">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="3869f-148">Created Date Time of the device</span></span>|
|<span data-ttu-id="3869f-149">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="3869f-149">lastContactedDateTime</span></span>|<span data-ttu-id="3869f-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3869f-150">DateTimeOffset</span></span>|<span data-ttu-id="3869f-151">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="3869f-151">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="3869f-152">説明</span><span class="sxs-lookup"><span data-stu-id="3869f-152">description</span></span>|<span data-ttu-id="3869f-153">String</span><span class="sxs-lookup"><span data-stu-id="3869f-153">String</span></span>|<span data-ttu-id="3869f-154">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="3869f-154">The description of the device</span></span>|
|<span data-ttu-id="3869f-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="3869f-155">enrollmentState</span></span>|[<span data-ttu-id="3869f-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="3869f-156">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="3869f-157">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="3869f-157">The state of the device in Intune.</span></span> <span data-ttu-id="3869f-158">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="3869f-158">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="3869f-159">platform</span><span class="sxs-lookup"><span data-stu-id="3869f-159">platform</span></span>|[<span data-ttu-id="3869f-160">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="3869f-160">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="3869f-161">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="3869f-161">The platform of the Device.</span></span> <span data-ttu-id="3869f-162">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="3869f-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3869f-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3869f-163">Relationships</span></span>
<span data-ttu-id="3869f-164">なし</span><span class="sxs-lookup"><span data-stu-id="3869f-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3869f-165">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3869f-165">JSON Representation</span></span>
<span data-ttu-id="3869f-166">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3869f-166">Here is a JSON representation of the resource.</span></span>
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




