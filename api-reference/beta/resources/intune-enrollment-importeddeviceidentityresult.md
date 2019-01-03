---
title: importedDeviceIdentityResult リソースの種類
description: ImportedDeviceIdentityResult リソースでは、デバイスの識別情報をインポートしようとした結果を表します。
author: tfitzmac
ms.openlocfilehash: 060ebbebb38cd258e57ca30794e44e5e651d5fe2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310172"
---
# <a name="importeddeviceidentityresult-resource-type"></a><span data-ttu-id="cc2ae-103">importedDeviceIdentityResult リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cc2ae-103">importedDeviceIdentityResult resource type</span></span>

> <span data-ttu-id="cc2ae-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cc2ae-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc2ae-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cc2ae-107">ImportedDeviceIdentityResult リソースでは、デバイスの識別情報をインポートしようとした結果を表します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-107">The importedDeviceIdentityResult resource represents the result of attempting to import a device identity.</span></span>

<span data-ttu-id="cc2ae-108">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-108">Inherits from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>

## <a name="methods"></a><span data-ttu-id="cc2ae-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc2ae-109">Methods</span></span>
|<span data-ttu-id="cc2ae-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="cc2ae-110">Method</span></span>|<span data-ttu-id="cc2ae-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cc2ae-111">Return Type</span></span>|<span data-ttu-id="cc2ae-112">説明</span><span class="sxs-lookup"><span data-stu-id="cc2ae-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cc2ae-113">リスト importedDeviceIdentityResults</span><span class="sxs-lookup"><span data-stu-id="cc2ae-113">List importedDeviceIdentityResults</span></span>](../api/intune-enrollment-importeddeviceidentityresult-list.md)|<span data-ttu-id="cc2ae-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="cc2ae-114">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="cc2ae-115">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-115">List properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) objects.</span></span>|
|[<span data-ttu-id="cc2ae-116">ImportedDeviceIdentityResult を取得します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-116">Get importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-get.md)|[<span data-ttu-id="cc2ae-117">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="cc2ae-117">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="cc2ae-118">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-118">Read properties and relationships of the [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="cc2ae-119">ImportedDeviceIdentityResult を作成します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-119">Create importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-create.md)|[<span data-ttu-id="cc2ae-120">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="cc2ae-120">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="cc2ae-121">新しい[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-121">Create a new [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|
|[<span data-ttu-id="cc2ae-122">ImportedDeviceIdentityResult を削除します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-122">Delete importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-delete.md)|<span data-ttu-id="cc2ae-123">なし</span><span class="sxs-lookup"><span data-stu-id="cc2ae-123">None</span></span>|<span data-ttu-id="cc2ae-124">の[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-124">Deletes a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md).</span></span>|
|[<span data-ttu-id="cc2ae-125">ImportedDeviceIdentityResult を更新します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-125">Update importedDeviceIdentityResult</span></span>](../api/intune-enrollment-importeddeviceidentityresult-update.md)|[<span data-ttu-id="cc2ae-126">importedDeviceIdentityResult</span><span class="sxs-lookup"><span data-stu-id="cc2ae-126">importedDeviceIdentityResult</span></span>](../resources/intune-enrollment-importeddeviceidentityresult.md)|<span data-ttu-id="cc2ae-127">[ImportedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-127">Update the properties of a [importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="cc2ae-128">Properties</span><span class="sxs-lookup"><span data-stu-id="cc2ae-128">Properties</span></span>
|<span data-ttu-id="cc2ae-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cc2ae-129">Property</span></span>|<span data-ttu-id="cc2ae-130">種類</span><span class="sxs-lookup"><span data-stu-id="cc2ae-130">Type</span></span>|<span data-ttu-id="cc2ae-131">説明</span><span class="sxs-lookup"><span data-stu-id="cc2ae-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc2ae-132">ID</span><span class="sxs-lookup"><span data-stu-id="cc2ae-132">id</span></span>|<span data-ttu-id="cc2ae-133">String</span><span class="sxs-lookup"><span data-stu-id="cc2ae-133">String</span></span>|<span data-ttu-id="cc2ae-134">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるインポート済みのデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="cc2ae-134">Id of the imported device identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="cc2ae-135">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="cc2ae-135">importedDeviceIdentifier</span></span>|<span data-ttu-id="cc2ae-136">String</span><span class="sxs-lookup"><span data-stu-id="cc2ae-136">String</span></span>|<span data-ttu-id="cc2ae-137">インポートされたデバイスの識別子から継承された[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span><span class="sxs-lookup"><span data-stu-id="cc2ae-137">Imported Device Identifier Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="cc2ae-138">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="cc2ae-138">importedDeviceIdentityType</span></span>|[<span data-ttu-id="cc2ae-139">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="cc2ae-139">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="cc2ae-140">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からインポートされたデバイスの Id を継承の種類。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-140">Type of Imported Device Identity Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="cc2ae-141">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-141">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="cc2ae-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc2ae-142">lastModifiedDateTime</span></span>|<span data-ttu-id="cc2ae-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc2ae-143">DateTimeOffset</span></span>|<span data-ttu-id="cc2ae-144">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承する」の説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="cc2ae-144">Last Modified DateTime of the description Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="cc2ae-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cc2ae-145">createdDateTime</span></span>|<span data-ttu-id="cc2ae-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc2ae-146">DateTimeOffset</span></span>|<span data-ttu-id="cc2ae-147">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの日時を作成</span><span class="sxs-lookup"><span data-stu-id="cc2ae-147">Created Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="cc2ae-148">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="cc2ae-148">lastContactedDateTime</span></span>|<span data-ttu-id="cc2ae-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cc2ae-149">DateTimeOffset</span></span>|<span data-ttu-id="cc2ae-150">最終接続日時[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されるデバイスの</span><span class="sxs-lookup"><span data-stu-id="cc2ae-150">Last Contacted Date Time of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="cc2ae-151">説明</span><span class="sxs-lookup"><span data-stu-id="cc2ae-151">description</span></span>|<span data-ttu-id="cc2ae-152">String</span><span class="sxs-lookup"><span data-stu-id="cc2ae-152">String</span></span>|<span data-ttu-id="cc2ae-153">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承される、デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="cc2ae-153">The description of the device Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)</span></span>|
|<span data-ttu-id="cc2ae-154">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="cc2ae-154">enrollmentState</span></span>|[<span data-ttu-id="cc2ae-155">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="cc2ae-155">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="cc2ae-156">Intune 継承で[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)からのデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-156">The state of the device in Intune Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="cc2ae-157">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-157">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="cc2ae-158">platform</span><span class="sxs-lookup"><span data-stu-id="cc2ae-158">platform</span></span>|[<span data-ttu-id="cc2ae-159">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="cc2ae-159">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="cc2ae-160">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-160">The platform of the Device.</span></span> <span data-ttu-id="cc2ae-161">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-161">Inherited from [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span> <span data-ttu-id="cc2ae-162">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-162">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|
|<span data-ttu-id="cc2ae-163">status</span><span class="sxs-lookup"><span data-stu-id="cc2ae-163">status</span></span>|<span data-ttu-id="cc2ae-164">ブール型</span><span class="sxs-lookup"><span data-stu-id="cc2ae-164">Boolean</span></span>|<span data-ttu-id="cc2ae-165">インポートされたデバイス id のステータス</span><span class="sxs-lookup"><span data-stu-id="cc2ae-165">Status of imported device identity</span></span>|

## <a name="relationships"></a><span data-ttu-id="cc2ae-166">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cc2ae-166">Relationships</span></span>
<span data-ttu-id="cc2ae-167">なし</span><span class="sxs-lookup"><span data-stu-id="cc2ae-167">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cc2ae-168">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cc2ae-168">JSON Representation</span></span>
<span data-ttu-id="cc2ae-169">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cc2ae-169">Here is a JSON representation of the resource.</span></span>
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




