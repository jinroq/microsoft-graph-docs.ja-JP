---
title: importedDeviceIdentity リソースの種類
description: ImportedDeviceIdentity リソースでは、事前登録の構成を事前にステージングされたデバイスの一意なハードウェア id を表します。
author: tfitzmac
ms.openlocfilehash: f7b6b054eab3815203a208382a19fbd9974cfb37
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350513"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="5206a-103">importedDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5206a-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="5206a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5206a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5206a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5206a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5206a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5206a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5206a-107">ImportedDeviceIdentity リソースでは、事前登録の構成を事前にステージングされたデバイスの一意なハードウェア id を表します。</span><span class="sxs-lookup"><span data-stu-id="5206a-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="5206a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5206a-108">Methods</span></span>
|<span data-ttu-id="5206a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5206a-109">Method</span></span>|<span data-ttu-id="5206a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5206a-110">Return Type</span></span>|<span data-ttu-id="5206a-111">説明</span><span class="sxs-lookup"><span data-stu-id="5206a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5206a-112">リスト importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="5206a-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="5206a-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5206a-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="5206a-114">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5206a-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="5206a-115">ImportedDeviceIdentity を取得します。</span><span class="sxs-lookup"><span data-stu-id="5206a-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="5206a-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5206a-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="5206a-117">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5206a-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="5206a-118">ImportedDeviceIdentity を作成します。</span><span class="sxs-lookup"><span data-stu-id="5206a-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="5206a-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5206a-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="5206a-120">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5206a-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="5206a-121">ImportedDeviceIdentity を削除します。</span><span class="sxs-lookup"><span data-stu-id="5206a-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="5206a-122">なし</span><span class="sxs-lookup"><span data-stu-id="5206a-122">None</span></span>|<span data-ttu-id="5206a-123">の[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5206a-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="5206a-124">ImportedDeviceIdentity を更新します。</span><span class="sxs-lookup"><span data-stu-id="5206a-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="5206a-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="5206a-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="5206a-126">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5206a-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="5206a-127">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="5206a-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="5206a-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5206a-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="5206a-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5206a-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5206a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5206a-130">Properties</span></span>
|<span data-ttu-id="5206a-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5206a-131">Property</span></span>|<span data-ttu-id="5206a-132">種類</span><span class="sxs-lookup"><span data-stu-id="5206a-132">Type</span></span>|<span data-ttu-id="5206a-133">説明</span><span class="sxs-lookup"><span data-stu-id="5206a-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5206a-134">ID</span><span class="sxs-lookup"><span data-stu-id="5206a-134">id</span></span>|<span data-ttu-id="5206a-135">String</span><span class="sxs-lookup"><span data-stu-id="5206a-135">String</span></span>|<span data-ttu-id="5206a-136">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="5206a-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="5206a-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="5206a-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="5206a-138">String</span><span class="sxs-lookup"><span data-stu-id="5206a-138">String</span></span>|<span data-ttu-id="5206a-139">インポートされたデバイスの識別子</span><span class="sxs-lookup"><span data-stu-id="5206a-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="5206a-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="5206a-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="5206a-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="5206a-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="5206a-142">インポートされたデバイスの識別情報の種類です。</span><span class="sxs-lookup"><span data-stu-id="5206a-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="5206a-143">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="5206a-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="5206a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5206a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="5206a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5206a-145">DateTimeOffset</span></span>|<span data-ttu-id="5206a-146">説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="5206a-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="5206a-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5206a-147">createdDateTime</span></span>|<span data-ttu-id="5206a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5206a-148">DateTimeOffset</span></span>|<span data-ttu-id="5206a-149">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="5206a-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="5206a-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="5206a-150">lastContactedDateTime</span></span>|<span data-ttu-id="5206a-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5206a-151">DateTimeOffset</span></span>|<span data-ttu-id="5206a-152">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="5206a-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="5206a-153">説明</span><span class="sxs-lookup"><span data-stu-id="5206a-153">description</span></span>|<span data-ttu-id="5206a-154">String</span><span class="sxs-lookup"><span data-stu-id="5206a-154">String</span></span>|<span data-ttu-id="5206a-155">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="5206a-155">The description of the device</span></span>|
|<span data-ttu-id="5206a-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5206a-156">enrollmentState</span></span>|[<span data-ttu-id="5206a-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="5206a-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="5206a-158">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="5206a-158">The state of the device in Intune.</span></span> <span data-ttu-id="5206a-159">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="5206a-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="5206a-160">platform</span><span class="sxs-lookup"><span data-stu-id="5206a-160">platform</span></span>|[<span data-ttu-id="5206a-161">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="5206a-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="5206a-162">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="5206a-162">The platform of the Device.</span></span> <span data-ttu-id="5206a-163">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="5206a-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5206a-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5206a-164">Relationships</span></span>
<span data-ttu-id="5206a-165">なし</span><span class="sxs-lookup"><span data-stu-id="5206a-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5206a-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5206a-166">JSON Representation</span></span>
<span data-ttu-id="5206a-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5206a-167">Here is a JSON representation of the resource.</span></span>
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





