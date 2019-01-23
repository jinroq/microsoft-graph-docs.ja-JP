---
title: importedDeviceIdentity リソースの種類
description: ImportedDeviceIdentity リソースでは、事前登録の構成を事前にステージングされたデバイスの一意なハードウェア id を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c151257a95d1161e07de17ed6d9fc01fc021146e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421446"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="24373-103">importedDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="24373-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="24373-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="24373-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="24373-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="24373-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24373-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="24373-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24373-107">ImportedDeviceIdentity リソースでは、事前登録の構成を事前にステージングされたデバイスの一意なハードウェア id を表します。</span><span class="sxs-lookup"><span data-stu-id="24373-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>

## <a name="methods"></a><span data-ttu-id="24373-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="24373-108">Methods</span></span>
|<span data-ttu-id="24373-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="24373-109">Method</span></span>|<span data-ttu-id="24373-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="24373-110">Return Type</span></span>|<span data-ttu-id="24373-111">説明</span><span class="sxs-lookup"><span data-stu-id="24373-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24373-112">リスト importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="24373-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="24373-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="24373-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="24373-114">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="24373-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="24373-115">ImportedDeviceIdentity を取得します。</span><span class="sxs-lookup"><span data-stu-id="24373-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="24373-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="24373-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="24373-117">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="24373-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="24373-118">ImportedDeviceIdentity を作成します。</span><span class="sxs-lookup"><span data-stu-id="24373-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="24373-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="24373-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="24373-120">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="24373-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="24373-121">ImportedDeviceIdentity を削除します。</span><span class="sxs-lookup"><span data-stu-id="24373-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="24373-122">なし</span><span class="sxs-lookup"><span data-stu-id="24373-122">None</span></span>|<span data-ttu-id="24373-123">の[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="24373-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="24373-124">ImportedDeviceIdentity を更新します。</span><span class="sxs-lookup"><span data-stu-id="24373-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="24373-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="24373-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="24373-126">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="24373-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="24373-127">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="24373-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="24373-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="24373-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="24373-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="24373-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="24373-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24373-130">Properties</span></span>
|<span data-ttu-id="24373-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="24373-131">Property</span></span>|<span data-ttu-id="24373-132">型</span><span class="sxs-lookup"><span data-stu-id="24373-132">Type</span></span>|<span data-ttu-id="24373-133">説明</span><span class="sxs-lookup"><span data-stu-id="24373-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24373-134">id</span><span class="sxs-lookup"><span data-stu-id="24373-134">id</span></span>|<span data-ttu-id="24373-135">String</span><span class="sxs-lookup"><span data-stu-id="24373-135">String</span></span>|<span data-ttu-id="24373-136">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="24373-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="24373-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="24373-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="24373-138">String</span><span class="sxs-lookup"><span data-stu-id="24373-138">String</span></span>|<span data-ttu-id="24373-139">インポートされたデバイスの識別子</span><span class="sxs-lookup"><span data-stu-id="24373-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="24373-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="24373-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="24373-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="24373-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="24373-142">インポートされたデバイスの識別情報の種類です。</span><span class="sxs-lookup"><span data-stu-id="24373-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="24373-143">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="24373-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="24373-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24373-144">lastModifiedDateTime</span></span>|<span data-ttu-id="24373-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24373-145">DateTimeOffset</span></span>|<span data-ttu-id="24373-146">説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="24373-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="24373-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24373-147">createdDateTime</span></span>|<span data-ttu-id="24373-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24373-148">DateTimeOffset</span></span>|<span data-ttu-id="24373-149">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="24373-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="24373-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="24373-150">lastContactedDateTime</span></span>|<span data-ttu-id="24373-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24373-151">DateTimeOffset</span></span>|<span data-ttu-id="24373-152">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="24373-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="24373-153">説明</span><span class="sxs-lookup"><span data-stu-id="24373-153">description</span></span>|<span data-ttu-id="24373-154">String</span><span class="sxs-lookup"><span data-stu-id="24373-154">String</span></span>|<span data-ttu-id="24373-155">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="24373-155">The description of the device</span></span>|
|<span data-ttu-id="24373-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="24373-156">enrollmentState</span></span>|[<span data-ttu-id="24373-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="24373-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="24373-158">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="24373-158">The state of the device in Intune.</span></span> <span data-ttu-id="24373-159">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="24373-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="24373-160">platform</span><span class="sxs-lookup"><span data-stu-id="24373-160">platform</span></span>|[<span data-ttu-id="24373-161">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="24373-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="24373-162">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="24373-162">The platform of the Device.</span></span> <span data-ttu-id="24373-163">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="24373-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24373-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="24373-164">Relationships</span></span>
<span data-ttu-id="24373-165">なし</span><span class="sxs-lookup"><span data-stu-id="24373-165">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24373-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="24373-166">JSON Representation</span></span>
<span data-ttu-id="24373-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="24373-167">Here is a JSON representation of the resource.</span></span>
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




