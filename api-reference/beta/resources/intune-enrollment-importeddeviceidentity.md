---
title: importedDeviceIdentity リソースの種類
description: ImportedDeviceIdentity リソースでは、事前登録の構成を事前にステージングされたデバイスの一意なハードウェア id を表します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 3c33069520913c7c750220ca8938459ba9bf96c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811670"
---
# <a name="importeddeviceidentity-resource-type"></a><span data-ttu-id="2e85d-103">importedDeviceIdentity リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2e85d-103">importedDeviceIdentity resource type</span></span>

> <span data-ttu-id="2e85d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2e85d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2e85d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e85d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2e85d-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e85d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e85d-107">ImportedDeviceIdentity リソースでは、事前登録の構成を事前にステージングされたデバイスの一意なハードウェア id を表します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-107">The importedDeviceIdentity resource represents a unique hardware identity of a device that has been pre-staged for pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="2e85d-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e85d-108">Methods</span></span>
|<span data-ttu-id="2e85d-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e85d-109">Method</span></span>|<span data-ttu-id="2e85d-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2e85d-110">Return Type</span></span>|<span data-ttu-id="2e85d-111">説明</span><span class="sxs-lookup"><span data-stu-id="2e85d-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2e85d-112">リスト importedDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="2e85d-112">List importedDeviceIdentities</span></span>](../api/intune-enrollment-importeddeviceidentity-list.md)|<span data-ttu-id="2e85d-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2e85d-113">[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) collection</span></span>|<span data-ttu-id="2e85d-114">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-114">List properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) objects.</span></span>|
|[<span data-ttu-id="2e85d-115">ImportedDeviceIdentity を取得します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-115">Get importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-get.md)|[<span data-ttu-id="2e85d-116">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2e85d-116">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2e85d-117">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e85d-117">Read properties and relationships of the [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2e85d-118">ImportedDeviceIdentity を作成します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-118">Create importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-create.md)|[<span data-ttu-id="2e85d-119">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2e85d-119">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2e85d-120">新しい[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-120">Create a new [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2e85d-121">ImportedDeviceIdentity を削除します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-121">Delete importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-delete.md)|<span data-ttu-id="2e85d-122">なし</span><span class="sxs-lookup"><span data-stu-id="2e85d-122">None</span></span>|<span data-ttu-id="2e85d-123">の[importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-123">Deletes a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md).</span></span>|
|[<span data-ttu-id="2e85d-124">ImportedDeviceIdentity を更新します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-124">Update importedDeviceIdentity</span></span>](../api/intune-enrollment-importeddeviceidentity-update.md)|[<span data-ttu-id="2e85d-125">importedDeviceIdentity</span><span class="sxs-lookup"><span data-stu-id="2e85d-125">importedDeviceIdentity</span></span>](../resources/intune-enrollment-importeddeviceidentity.md)|<span data-ttu-id="2e85d-126">[ImportedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2e85d-126">Update the properties of a [importedDeviceIdentity](../resources/intune-enrollment-importeddeviceidentity.md) object.</span></span>|
|[<span data-ttu-id="2e85d-127">importDeviceIdentityList アクション</span><span class="sxs-lookup"><span data-stu-id="2e85d-127">importDeviceIdentityList action</span></span>](../api/intune-enrollment-importeddeviceidentity-importdeviceidentitylist.md)|<span data-ttu-id="2e85d-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="2e85d-128">[importedDeviceIdentityResult](../resources/intune-enrollment-importeddeviceidentityresult.md) collection</span></span>|<span data-ttu-id="2e85d-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2e85d-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="2e85d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e85d-130">Properties</span></span>
|<span data-ttu-id="2e85d-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e85d-131">Property</span></span>|<span data-ttu-id="2e85d-132">種類</span><span class="sxs-lookup"><span data-stu-id="2e85d-132">Type</span></span>|<span data-ttu-id="2e85d-133">説明</span><span class="sxs-lookup"><span data-stu-id="2e85d-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e85d-134">ID</span><span class="sxs-lookup"><span data-stu-id="2e85d-134">id</span></span>|<span data-ttu-id="2e85d-135">String</span><span class="sxs-lookup"><span data-stu-id="2e85d-135">String</span></span>|<span data-ttu-id="2e85d-136">インポートされたデバイス id の id</span><span class="sxs-lookup"><span data-stu-id="2e85d-136">Id of the imported device identity</span></span>|
|<span data-ttu-id="2e85d-137">importedDeviceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2e85d-137">importedDeviceIdentifier</span></span>|<span data-ttu-id="2e85d-138">String</span><span class="sxs-lookup"><span data-stu-id="2e85d-138">String</span></span>|<span data-ttu-id="2e85d-139">インポートされたデバイスの識別子</span><span class="sxs-lookup"><span data-stu-id="2e85d-139">Imported Device Identifier</span></span>|
|<span data-ttu-id="2e85d-140">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2e85d-140">importedDeviceIdentityType</span></span>|[<span data-ttu-id="2e85d-141">importedDeviceIdentityType</span><span class="sxs-lookup"><span data-stu-id="2e85d-141">importedDeviceIdentityType</span></span>](../resources/intune-enrollment-importeddeviceidentitytype.md)|<span data-ttu-id="2e85d-142">インポートされたデバイスの識別情報の種類です。</span><span class="sxs-lookup"><span data-stu-id="2e85d-142">Type of Imported Device Identity.</span></span> <span data-ttu-id="2e85d-143">可能な値は、`unknown`、`imei`、`serialNumber` です。</span><span class="sxs-lookup"><span data-stu-id="2e85d-143">Possible values are: `unknown`, `imei`, `serialNumber`.</span></span>|
|<span data-ttu-id="2e85d-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e85d-144">lastModifiedDateTime</span></span>|<span data-ttu-id="2e85d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e85d-145">DateTimeOffset</span></span>|<span data-ttu-id="2e85d-146">説明の最後の変更日時</span><span class="sxs-lookup"><span data-stu-id="2e85d-146">Last Modified DateTime of the description</span></span>|
|<span data-ttu-id="2e85d-147">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e85d-147">createdDateTime</span></span>|<span data-ttu-id="2e85d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e85d-148">DateTimeOffset</span></span>|<span data-ttu-id="2e85d-149">デバイスの作成日時</span><span class="sxs-lookup"><span data-stu-id="2e85d-149">Created Date Time of the device</span></span>|
|<span data-ttu-id="2e85d-150">lastContactedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e85d-150">lastContactedDateTime</span></span>|<span data-ttu-id="2e85d-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e85d-151">DateTimeOffset</span></span>|<span data-ttu-id="2e85d-152">最終アクセス日時、デバイスの</span><span class="sxs-lookup"><span data-stu-id="2e85d-152">Last Contacted Date Time of the device</span></span>|
|<span data-ttu-id="2e85d-153">説明</span><span class="sxs-lookup"><span data-stu-id="2e85d-153">description</span></span>|<span data-ttu-id="2e85d-154">String</span><span class="sxs-lookup"><span data-stu-id="2e85d-154">String</span></span>|<span data-ttu-id="2e85d-155">デバイスの説明</span><span class="sxs-lookup"><span data-stu-id="2e85d-155">The description of the device</span></span>|
|<span data-ttu-id="2e85d-156">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2e85d-156">enrollmentState</span></span>|[<span data-ttu-id="2e85d-157">enrollmentState</span><span class="sxs-lookup"><span data-stu-id="2e85d-157">enrollmentState</span></span>](../resources/intune-enrollment-enrollmentstate.md)|<span data-ttu-id="2e85d-158">Intune でデバイスの状態。</span><span class="sxs-lookup"><span data-stu-id="2e85d-158">The state of the device in Intune.</span></span> <span data-ttu-id="2e85d-159">使用可能な値: `unknown`、`enrolled`、`pendingReset`、`failed`、`notContacted`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="2e85d-159">Possible values are: `unknown`, `enrolled`, `pendingReset`, `failed`, `notContacted`, `blocked`.</span></span>|
|<span data-ttu-id="2e85d-160">platform</span><span class="sxs-lookup"><span data-stu-id="2e85d-160">platform</span></span>|[<span data-ttu-id="2e85d-161">プラットフォーム</span><span class="sxs-lookup"><span data-stu-id="2e85d-161">platform</span></span>](../resources/intune-enrollment-platform.md)|<span data-ttu-id="2e85d-162">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="2e85d-162">The platform of the Device.</span></span> <span data-ttu-id="2e85d-163">使用可能な値: `unknown`、`ios`、`android`、`windows`、`windowsMobile`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="2e85d-163">Possible values are: `unknown`, `ios`, `android`, `windows`, `windowsMobile`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e85d-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e85d-164">Relationships</span></span>
<span data-ttu-id="2e85d-165">なし</span><span class="sxs-lookup"><span data-stu-id="2e85d-165">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2e85d-166">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e85d-166">JSON Representation</span></span>
<span data-ttu-id="2e85d-167">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e85d-167">Here is a JSON representation of the resource.</span></span>
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





