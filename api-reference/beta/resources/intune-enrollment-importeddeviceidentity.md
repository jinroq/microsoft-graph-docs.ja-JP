---
title: importedDeviceIdentity リソースの種類
description: ImportedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 20109d058fe34644867719a0c689a72139a501be
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36327928"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="f2f0c-103">importedDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2f0c-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="f2f0c-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f2f0c-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f2f0c-106">ImportedDeviceIdentity リソースは、事前登録構成のために事前にステージングされたデバイスの一意のハードウェア id を表します。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-106">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="f2f0c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2f0c-107">Methods</span></span>
|<span data-ttu-id="f2f0c-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="f2f0c-108">Method</span></span>|<span data-ttu-id="f2f0c-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f2f0c-109">Return Type</span></span>|<span data-ttu-id="f2f0c-110">説明</span><span class="sxs-lookup"><span data-stu-id="f2f0c-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f2f0c-111">リスト importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="f2f0c-111">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="f2f0c-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f2f0c-112">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="f2f0c-113">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-113">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="f2f0c-114">ImportedDeviceIdentity を取得する</span><span class="sxs-lookup"><span data-stu-id="f2f0c-114">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="f2f0c-115">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f2f0c-115">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f2f0c-116">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-116">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f2f0c-117">ImportedDeviceIdentity を作成する</span><span class="sxs-lookup"><span data-stu-id="f2f0c-117">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="f2f0c-118">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f2f0c-118">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f2f0c-119">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-119">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f2f0c-120">ImportedDeviceIdentity の削除</span><span class="sxs-lookup"><span data-stu-id="f2f0c-120">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="f2f0c-121">None</span><span class="sxs-lookup"><span data-stu-id="f2f0c-121">None</span></span>|<span data-ttu-id="f2f0c-122">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-122">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="f2f0c-123">ImportedDeviceIdentity の更新</span><span class="sxs-lookup"><span data-stu-id="f2f0c-123">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="f2f0c-124">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="f2f0c-124">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="f2f0c-125">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-125">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="f2f0c-126">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="f2f0c-126">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="f2f0c-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f2f0c-127">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="f2f0c-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f2f0c-128">Not yet documented</span></span>|
|[<span data-ttu-id="f2f0c-129">searchExistingIdentities アクション</span><span class="sxs-lookup"><span data-stu-id="f2f0c-129">searchExistingIdentities action</span></span>](../api/intune-enrollment-importeddeviceidentity-searchexistingidentities.md)|<span data-ttu-id="f2f0c-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="f2f0c-130">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="f2f0c-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="f2f0c-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="f2f0c-132">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2f0c-132">Properties</span></span>
|<span data-ttu-id="f2f0c-133">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2f0c-133">Property</span></span>|<span data-ttu-id="f2f0c-134">型</span><span class="sxs-lookup"><span data-stu-id="f2f0c-134">Type</span></span>|<span data-ttu-id="f2f0c-135">説明</span><span class="sxs-lookup"><span data-stu-id="f2f0c-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2f0c-136">id</span><span class="sxs-lookup"><span data-stu-id="f2f0c-136">id</span></span>|<span data-ttu-id="f2f0c-137">String</span><span class="sxs-lookup"><span data-stu-id="f2f0c-137">String</span></span>|<span data-ttu-id="f2f0c-138">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="f2f0c-138">Id of the imported device identity</span></span>|
|<span data-ttu-id="f2f0c-139">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="f2f0c-139">importedDeviceIdentifier</span></span>|<span data-ttu-id="f2f0c-140">String</span><span class="sxs-lookup"><span data-stu-id="f2f0c-140">String</span></span>|<span data-ttu-id="f2f0c-141">インポートされたデバイス識別子</span><span class="sxs-lookup"><span data-stu-id="f2f0c-141">Imported Device Identifier</span></span>|
|<span data-ttu-id="f2f0c-142">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f2f0c-142">importedDeviceIdentityType</span></span>|[<span data-ttu-id="f2f0c-143">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="f2f0c-143">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="f2f0c-144">インポートされたデバイス Id の種類。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-144">Type of Imported Device Identity.</span></span> <span data-ttu-id="f2f0c-145">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-145">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="f2f0c-146">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2f0c-146">lastModifiedDateTime</span></span>|<span data-ttu-id="f2f0c-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f0c-147">DateTimeOffset</span></span>|<span data-ttu-id="f2f0c-148">説明の最終更新日時</span><span class="sxs-lookup"><span data-stu-id="f2f0c-148">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="f2f0c-149">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2f0c-149">createdDateTime</span></span>|<span data-ttu-id="f2f0c-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f0c-150">DateTimeOffset</span></span>|<span data-ttu-id="f2f0c-151">デバイスの日時の作成日時</span><span class="sxs-lookup"><span data-stu-id="f2f0c-151">Created Date Time of the device</span></span>|
|<span data-ttu-id="f2f0c-152">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="f2f0c-152">lastContactedDateTime</span></span>|<span data-ttu-id="f2f0c-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2f0c-153">DateTimeOffset</span></span>|<span data-ttu-id="f2f0c-154">デバイスの最終連絡日時</span><span class="sxs-lookup"><span data-stu-id="f2f0c-154">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="f2f0c-155">description</span><span class="sxs-lookup"><span data-stu-id="f2f0c-155">description</span></span>|<span data-ttu-id="f2f0c-156">String</span><span class="sxs-lookup"><span data-stu-id="f2f0c-156">String</span></span>|<span data-ttu-id="f2f0c-157">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="f2f0c-157">The description of the device</span></span>|
|<span data-ttu-id="f2f0c-158">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f2f0c-158">enrollmentState</span></span>|[<span data-ttu-id="f2f0c-159">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="f2f0c-159">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="f2f0c-160">Intune でのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-160">The state of the device in Intune.</span></span> <span data-ttu-id="f2f0c-161">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-161">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="f2f0c-162">platform</span><span class="sxs-lookup"><span data-stu-id="f2f0c-162">platform</span></span>|[<span data-ttu-id="f2f0c-163">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="f2f0c-163">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="f2f0c-164">デバイスのプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-164">The platform of the Device.</span></span> <span data-ttu-id="f2f0c-165">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-165">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2f0c-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f2f0c-166">Relationships</span></span>
<span data-ttu-id="f2f0c-167">なし</span><span class="sxs-lookup"><span data-stu-id="f2f0c-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f2f0c-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2f0c-168">JSON Representation</span></span>
<span data-ttu-id="f2f0c-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f2f0c-169">Here is a JSON representation of the resource.</span></span>
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



