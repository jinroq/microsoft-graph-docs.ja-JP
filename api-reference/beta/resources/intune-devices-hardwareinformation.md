---
title: ハードウェア情報リソースの種類
description: 特定のデバイスのハードウェア情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 874cee0b2b09b3d106d771f2c176ceed3d4d04e8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999788"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="139c7-103">ハードウェア情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="139c7-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="139c7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="139c7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="139c7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="139c7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="139c7-106">特定のデバイスのハードウェア情報。</span><span class="sxs-lookup"><span data-stu-id="139c7-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="139c7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="139c7-107">Properties</span></span>
|<span data-ttu-id="139c7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="139c7-108">Property</span></span>|<span data-ttu-id="139c7-109">型</span><span class="sxs-lookup"><span data-stu-id="139c7-109">Type</span></span>|<span data-ttu-id="139c7-110">説明</span><span class="sxs-lookup"><span data-stu-id="139c7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="139c7-111">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="139c7-111">serialNumber</span></span>|<span data-ttu-id="139c7-112">String</span><span class="sxs-lookup"><span data-stu-id="139c7-112">String</span></span>|<span data-ttu-id="139c7-113">シリアル番号です。</span><span class="sxs-lookup"><span data-stu-id="139c7-113">Serial number.</span></span>|
|<span data-ttu-id="139c7-114">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="139c7-114">totalStorageSpace</span></span>|<span data-ttu-id="139c7-115">Int64</span><span class="sxs-lookup"><span data-stu-id="139c7-115">Int64</span></span>|<span data-ttu-id="139c7-116">デバイスの記憶領域の合計。</span><span class="sxs-lookup"><span data-stu-id="139c7-116">Total storage space of the device.</span></span>|
|<span data-ttu-id="139c7-117">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="139c7-117">freeStorageSpace</span></span>|<span data-ttu-id="139c7-118">Int64</span><span class="sxs-lookup"><span data-stu-id="139c7-118">Int64</span></span>|<span data-ttu-id="139c7-119">デバイスの記憶域スペースを解放します。</span><span class="sxs-lookup"><span data-stu-id="139c7-119">Free storage space of the device.</span></span>|
|<span data-ttu-id="139c7-120">imei</span><span class="sxs-lookup"><span data-stu-id="139c7-120">imei</span></span>|<span data-ttu-id="139c7-121">String</span><span class="sxs-lookup"><span data-stu-id="139c7-121">String</span></span>|<span data-ttu-id="139c7-122">IMEI</span><span class="sxs-lookup"><span data-stu-id="139c7-122">IMEI</span></span>|
|<span data-ttu-id="139c7-123">meid</span><span class="sxs-lookup"><span data-stu-id="139c7-123">meid</span></span>|<span data-ttu-id="139c7-124">String</span><span class="sxs-lookup"><span data-stu-id="139c7-124">String</span></span>|<span data-ttu-id="139c7-125">MEID</span><span class="sxs-lookup"><span data-stu-id="139c7-125">MEID</span></span>|
|<span data-ttu-id="139c7-126">manufacturer</span><span class="sxs-lookup"><span data-stu-id="139c7-126">manufacturer</span></span>|<span data-ttu-id="139c7-127">String</span><span class="sxs-lookup"><span data-stu-id="139c7-127">String</span></span>|<span data-ttu-id="139c7-128">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="139c7-128">Manufacturer of the device</span></span>|
|<span data-ttu-id="139c7-129">model</span><span class="sxs-lookup"><span data-stu-id="139c7-129">model</span></span>|<span data-ttu-id="139c7-130">String</span><span class="sxs-lookup"><span data-stu-id="139c7-130">String</span></span>|<span data-ttu-id="139c7-131">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="139c7-131">Model of the device</span></span>|
|<span data-ttu-id="139c7-132">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="139c7-132">phoneNumber</span></span>|<span data-ttu-id="139c7-133">String</span><span class="sxs-lookup"><span data-stu-id="139c7-133">String</span></span>|<span data-ttu-id="139c7-134">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="139c7-134">Phone number of the device</span></span>|
|<span data-ttu-id="139c7-135">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="139c7-135">subscriberCarrier</span></span>|<span data-ttu-id="139c7-136">String</span><span class="sxs-lookup"><span data-stu-id="139c7-136">String</span></span>|<span data-ttu-id="139c7-137">デバイスのサブスクライバーキャリア</span><span class="sxs-lookup"><span data-stu-id="139c7-137">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="139c7-138">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="139c7-138">cellularTechnology</span></span>|<span data-ttu-id="139c7-139">String</span><span class="sxs-lookup"><span data-stu-id="139c7-139">String</span></span>|<span data-ttu-id="139c7-140">デバイスの携帯電話テクノロジ</span><span class="sxs-lookup"><span data-stu-id="139c7-140">Cellular technology of the device</span></span>|
|<span data-ttu-id="139c7-141">wifiMac</span><span class="sxs-lookup"><span data-stu-id="139c7-141">wifiMac</span></span>|<span data-ttu-id="139c7-142">String</span><span class="sxs-lookup"><span data-stu-id="139c7-142">String</span></span>|<span data-ttu-id="139c7-143">デバイスの WiFi MAC アドレス</span><span class="sxs-lookup"><span data-stu-id="139c7-143">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="139c7-144">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="139c7-144">operatingSystemLanguage</span></span>|<span data-ttu-id="139c7-145">String</span><span class="sxs-lookup"><span data-stu-id="139c7-145">String</span></span>|<span data-ttu-id="139c7-146">デバイスのオペレーティングシステムの言語</span><span class="sxs-lookup"><span data-stu-id="139c7-146">Operating system language of the device</span></span>|
|<span data-ttu-id="139c7-147">isSupervised</span><span class="sxs-lookup"><span data-stu-id="139c7-147">isSupervised</span></span>|<span data-ttu-id="139c7-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="139c7-148">Boolean</span></span>|<span data-ttu-id="139c7-149">デバイスの監視モード</span><span class="sxs-lookup"><span data-stu-id="139c7-149">Supervised mode of the device</span></span>|
|<span data-ttu-id="139c7-150">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="139c7-150">isEncrypted</span></span>|<span data-ttu-id="139c7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="139c7-151">Boolean</span></span>|<span data-ttu-id="139c7-152">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="139c7-152">Encryption status of the device</span></span>|
|<span data-ttu-id="139c7-153">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="139c7-153">isSharedDevice</span></span>|<span data-ttu-id="139c7-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="139c7-154">Boolean</span></span>|<span data-ttu-id="139c7-155">共有 iPad</span><span class="sxs-lookup"><span data-stu-id="139c7-155">Shared iPad</span></span>|
|<span data-ttu-id="139c7-156">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="139c7-156">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="139c7-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="139c7-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="139c7-158">共有 Apple デバイス上のすべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="139c7-158">All users on the shared Apple device</span></span>|
|<span data-ttu-id="139c7-159">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="139c7-159">tpmSpecificationVersion</span></span>|<span data-ttu-id="139c7-160">String</span><span class="sxs-lookup"><span data-stu-id="139c7-160">String</span></span>|<span data-ttu-id="139c7-161">仕様バージョンを指定する文字列。</span><span class="sxs-lookup"><span data-stu-id="139c7-161">String that specifies the specification version.</span></span>|
|<span data-ttu-id="139c7-162">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="139c7-162">operatingSystemEdition</span></span>|<span data-ttu-id="139c7-163">String</span><span class="sxs-lookup"><span data-stu-id="139c7-163">String</span></span>|<span data-ttu-id="139c7-164">OS のエディションを指定する文字列。</span><span class="sxs-lookup"><span data-stu-id="139c7-164">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="139c7-165">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="139c7-165">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="139c7-166">String</span><span class="sxs-lookup"><span data-stu-id="139c7-166">String</span></span>|<span data-ttu-id="139c7-167">デバイスの完全修飾ドメイン名を返します (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="139c7-167">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="139c7-168">デバイスがドメインに参加していない場合は、空の文字列が返されます。</span><span class="sxs-lookup"><span data-stu-id="139c7-168">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="139c7-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="139c7-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="139c7-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="139c7-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="139c7-171">仮想化ベースのセキュリティハードウェア要件の状態。</span><span class="sxs-lookup"><span data-stu-id="139c7-171">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="139c7-172">可能な値は、`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable` です。</span><span class="sxs-lookup"><span data-stu-id="139c7-172">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="139c7-173">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="139c7-173">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="139c7-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="139c7-174">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="139c7-175">仮想化ベースのセキュリティの状態。</span><span class="sxs-lookup"><span data-stu-id="139c7-175">Virtualization-based security status.</span></span> <span data-ttu-id="139c7-176">.</span><span class="sxs-lookup"><span data-stu-id="139c7-176"></span></span> <span data-ttu-id="139c7-177">可能な値は、`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="139c7-177">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="139c7-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="139c7-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="139c7-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="139c7-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="139c7-180">ローカルシステム権限 (LSA) credential guard の状態。</span><span class="sxs-lookup"><span data-stu-id="139c7-180">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="139c7-181">.</span><span class="sxs-lookup"><span data-stu-id="139c7-181"></span></span> <span data-ttu-id="139c7-182">可能な値は、`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning` です。</span><span class="sxs-lookup"><span data-stu-id="139c7-182">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="139c7-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="139c7-183">Relationships</span></span>
<span data-ttu-id="139c7-184">なし</span><span class="sxs-lookup"><span data-stu-id="139c7-184">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="139c7-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="139c7-185">JSON Representation</span></span>
<span data-ttu-id="139c7-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="139c7-186">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





