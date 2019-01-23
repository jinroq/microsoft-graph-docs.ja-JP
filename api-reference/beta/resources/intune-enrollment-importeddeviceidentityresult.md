---
title: importedDeviceIdentityResult リソースの種類
description: ImportedDeviceIdentityResult リソースでは、デバイスの識別情報をインポートしようとした結果を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e4a1720fee543b4814430476ebd6c84a0fc33d73
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395805"
---
# <a name="importeddeviceidentityresult-resource-type"></a><span data-ttu-id="bd2c6-103">importedDeviceIdentityResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bd2c6-103">importedDeviceIdentityResult resource type</span></span>

> <span data-ttu-id="bd2c6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bd2c6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bd2c6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd2c6-107">ImportedDeviceIdentityResult リソースでは、デバイスの識別情報をインポートしようとした結果を表します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-107">The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.</span></span>


<span data-ttu-id="bd2c6-108">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-108">Inherits from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>

## <a name="methods"></a><span data-ttu-id="bd2c6-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="bd2c6-109">Methods</span></span>
|<span data-ttu-id="bd2c6-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="bd2c6-110">Method</span></span>|<span data-ttu-id="bd2c6-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bd2c6-111">Return Type</span></span>|<span data-ttu-id="bd2c6-112">説明</span><span class="sxs-lookup"><span data-stu-id="bd2c6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bd2c6-113">リスト importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="bd2c6-113">List importedDeviceIdentityResults</span></span>](../api/intune-enrollment-importeddeviceidentityresult-list.md)|<span data-ttu-id="bd2c6-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bd2c6-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="bd2c6-115">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-115">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>|
|[<span data-ttu-id="bd2c6-116">ImportedDeviceIdentityResult を取得します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-116">Get importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[<span data-ttu-id="bd2c6-117">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="bd2c6-117">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="bd2c6-118">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-118">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="bd2c6-119">ImportedDeviceIdentityResult を作成します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-119">Create importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[<span data-ttu-id="bd2c6-120">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="bd2c6-120">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="bd2c6-121">新しい[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-121">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="bd2c6-122">ImportedDeviceIdentityResult を削除します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-122">Delete importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|<span data-ttu-id="bd2c6-123">なし</span><span class="sxs-lookup"><span data-stu-id="bd2c6-123">None</span></span>|<span data-ttu-id="bd2c6-124">の[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-124">Deletes a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>|
|[<span data-ttu-id="bd2c6-125">ImportedDeviceIdentityResult を更新します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-125">Update importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[<span data-ttu-id="bd2c6-126">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="bd2c6-126">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="bd2c6-127">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-127">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bd2c6-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd2c6-128">Properties</span></span>
|<span data-ttu-id="bd2c6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bd2c6-129">Property</span></span>|<span data-ttu-id="bd2c6-130">型</span><span class="sxs-lookup"><span data-stu-id="bd2c6-130">Type</span></span>|<span data-ttu-id="bd2c6-131">説明</span><span class="sxs-lookup"><span data-stu-id="bd2c6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd2c6-132">id</span><span class="sxs-lookup"><span data-stu-id="bd2c6-132">id</span></span>|<span data-ttu-id="bd2c6-133">String</span><span class="sxs-lookup"><span data-stu-id="bd2c6-133">String</span></span>|<span data-ttu-id="bd2c6-134">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるインポート済みのデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="bd2c6-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bd2c6-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="bd2c6-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="bd2c6-136">String</span><span class="sxs-lookup"><span data-stu-id="bd2c6-136">String</span></span>|<span data-ttu-id="bd2c6-137">インポートされたデバイスの識別子から継承された[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="bd2c6-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bd2c6-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="bd2c6-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="bd2c6-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="bd2c6-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="bd2c6-140">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からインポートされたデバイスの Id を継承の種類。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="bd2c6-141">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="bd2c6-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd2c6-142">lastModifiedDateTime</span></span>|<span data-ttu-id="bd2c6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd2c6-143">DateTimeOffset</span></span>|<span data-ttu-id="bd2c6-144">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承する」の説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="bd2c6-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bd2c6-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bd2c6-145">createdDateTime</span></span>|<span data-ttu-id="bd2c6-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd2c6-146">DateTimeOffset</span></span>|<span data-ttu-id="bd2c6-147">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの日時を作成</span><span class="sxs-lookup"><span data-stu-id="bd2c6-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bd2c6-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd2c6-148">lastContactedDateTime</span></span>|<span data-ttu-id="bd2c6-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd2c6-149">DateTimeOffset</span></span>|<span data-ttu-id="bd2c6-150">最終接続日時[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるデバイスの</span><span class="sxs-lookup"><span data-stu-id="bd2c6-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bd2c6-151">説明</span><span class="sxs-lookup"><span data-stu-id="bd2c6-151">description</span></span>|<span data-ttu-id="bd2c6-152">String</span><span class="sxs-lookup"><span data-stu-id="bd2c6-152">String</span></span>|<span data-ttu-id="bd2c6-153">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="bd2c6-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="bd2c6-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="bd2c6-154">enrollmentState</span></span>|[<span data-ttu-id="bd2c6-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="bd2c6-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="bd2c6-156">Intune 継承で[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="bd2c6-157">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="bd2c6-158">platform</span><span class="sxs-lookup"><span data-stu-id="bd2c6-158">platform</span></span>|[<span data-ttu-id="bd2c6-159">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="bd2c6-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="bd2c6-160">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-160">The platform of the Device.</span></span> <span data-ttu-id="bd2c6-161">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="bd2c6-162">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="bd2c6-163">status</span><span class="sxs-lookup"><span data-stu-id="bd2c6-163">status</span></span>|<span data-ttu-id="bd2c6-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="bd2c6-164">Boolean</span></span>|<span data-ttu-id="bd2c6-165">インポートされたデバイス id のステータス</span><span class="sxs-lookup"><span data-stu-id="bd2c6-165">Status of imported device identity</span></span>|

## <a name="relationships"></a><span data-ttu-id="bd2c6-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bd2c6-166">Relationships</span></span>
<span data-ttu-id="bd2c6-167">なし</span><span class="sxs-lookup"><span data-stu-id="bd2c6-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bd2c6-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bd2c6-168">JSON Representation</span></span>
<span data-ttu-id="bd2c6-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bd2c6-169">Here is a JSON representation of the resource.</span></span>
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




