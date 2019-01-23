---
title: hardwareInformation リソースの種類
description: 特定のデバイスのハードウェア情報です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32b6d0e637c477265a6d23f39e531ca89c7e490c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394825"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="bc567-103">hardwareInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bc567-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="bc567-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bc567-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="bc567-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bc567-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc567-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="bc567-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc567-107">特定のデバイスのハードウェア情報です。</span><span class="sxs-lookup"><span data-stu-id="bc567-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="bc567-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc567-108">Properties</span></span>
|<span data-ttu-id="bc567-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bc567-109">Property</span></span>|<span data-ttu-id="bc567-110">型</span><span class="sxs-lookup"><span data-stu-id="bc567-110">Type</span></span>|<span data-ttu-id="bc567-111">説明</span><span class="sxs-lookup"><span data-stu-id="bc567-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc567-112">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="bc567-112">serialNumber</span></span>|<span data-ttu-id="bc567-113">String</span><span class="sxs-lookup"><span data-stu-id="bc567-113">String</span></span>|<span data-ttu-id="bc567-114">シリアル番号です。</span><span class="sxs-lookup"><span data-stu-id="bc567-114">Serial number.</span></span>|
|<span data-ttu-id="bc567-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="bc567-115">totalStorageSpace</span></span>|<span data-ttu-id="bc567-116">Int64</span><span class="sxs-lookup"><span data-stu-id="bc567-116">Int64</span></span>|<span data-ttu-id="bc567-117">デバイスの合計容量。</span><span class="sxs-lookup"><span data-stu-id="bc567-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="bc567-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="bc567-118">freeStorageSpace</span></span>|<span data-ttu-id="bc567-119">Int64</span><span class="sxs-lookup"><span data-stu-id="bc567-119">Int64</span></span>|<span data-ttu-id="bc567-120">デバイスの空き容量。</span><span class="sxs-lookup"><span data-stu-id="bc567-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="bc567-121">imei</span><span class="sxs-lookup"><span data-stu-id="bc567-121">imei</span></span>|<span data-ttu-id="bc567-122">String</span><span class="sxs-lookup"><span data-stu-id="bc567-122">String</span></span>|<span data-ttu-id="bc567-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="bc567-123">IMEI</span></span>|
|<span data-ttu-id="bc567-124">meid</span><span class="sxs-lookup"><span data-stu-id="bc567-124">meid</span></span>|<span data-ttu-id="bc567-125">String</span><span class="sxs-lookup"><span data-stu-id="bc567-125">String</span></span>|<span data-ttu-id="bc567-126">MEID</span><span class="sxs-lookup"><span data-stu-id="bc567-126">MEID</span></span>|
|<span data-ttu-id="bc567-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="bc567-127">manufacturer</span></span>|<span data-ttu-id="bc567-128">String</span><span class="sxs-lookup"><span data-stu-id="bc567-128">String</span></span>|<span data-ttu-id="bc567-129">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="bc567-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="bc567-130">model</span><span class="sxs-lookup"><span data-stu-id="bc567-130">model</span></span>|<span data-ttu-id="bc567-131">String</span><span class="sxs-lookup"><span data-stu-id="bc567-131">String</span></span>|<span data-ttu-id="bc567-132">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="bc567-132">Model of the device</span></span>|
|<span data-ttu-id="bc567-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="bc567-133">phoneNumber</span></span>|<span data-ttu-id="bc567-134">String</span><span class="sxs-lookup"><span data-stu-id="bc567-134">String</span></span>|<span data-ttu-id="bc567-135">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="bc567-135">Phone number of the device</span></span>|
|<span data-ttu-id="bc567-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="bc567-136">subscriberCarrier</span></span>|<span data-ttu-id="bc567-137">String</span><span class="sxs-lookup"><span data-stu-id="bc567-137">String</span></span>|<span data-ttu-id="bc567-138">デバイスのサブスクライバーのキャリア</span><span class="sxs-lookup"><span data-stu-id="bc567-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="bc567-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="bc567-139">cellularTechnology</span></span>|<span data-ttu-id="bc567-140">String</span><span class="sxs-lookup"><span data-stu-id="bc567-140">String</span></span>|<span data-ttu-id="bc567-141">デバイスの携帯電話のテクノロジー</span><span class="sxs-lookup"><span data-stu-id="bc567-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="bc567-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="bc567-142">wifiMac</span></span>|<span data-ttu-id="bc567-143">String</span><span class="sxs-lookup"><span data-stu-id="bc567-143">String</span></span>|<span data-ttu-id="bc567-144">デバイスの WiFi の MAC アドレス</span><span class="sxs-lookup"><span data-stu-id="bc567-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="bc567-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="bc567-145">operatingSystemLanguage</span></span>|<span data-ttu-id="bc567-146">String</span><span class="sxs-lookup"><span data-stu-id="bc567-146">String</span></span>|<span data-ttu-id="bc567-147">デバイスのオペレーティング システムの言語</span><span class="sxs-lookup"><span data-stu-id="bc567-147">Operating system language of the device</span></span>|
|<span data-ttu-id="bc567-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="bc567-148">isSupervised</span></span>|<span data-ttu-id="bc567-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc567-149">Boolean</span></span>|<span data-ttu-id="bc567-150">デバイスのコールを管理モード</span><span class="sxs-lookup"><span data-stu-id="bc567-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="bc567-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="bc567-151">isEncrypted</span></span>|<span data-ttu-id="bc567-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc567-152">Boolean</span></span>|<span data-ttu-id="bc567-153">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="bc567-153">Encryption status of the device</span></span>|
|<span data-ttu-id="bc567-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="bc567-154">isSharedDevice</span></span>|<span data-ttu-id="bc567-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="bc567-155">Boolean</span></span>|<span data-ttu-id="bc567-156">IPad の共有</span><span class="sxs-lookup"><span data-stu-id="bc567-156">Shared iPad</span></span>|
|<span data-ttu-id="bc567-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="bc567-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="bc567-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="bc567-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="bc567-159">共有の Apple デバイス上のすべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="bc567-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="bc567-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="bc567-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="bc567-161">String</span><span class="sxs-lookup"><span data-stu-id="bc567-161">String</span></span>|<span data-ttu-id="bc567-162">仕様のバージョンを指定する文字列。</span><span class="sxs-lookup"><span data-stu-id="bc567-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="bc567-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="bc567-163">operatingSystemEdition</span></span>|<span data-ttu-id="bc567-164">String</span><span class="sxs-lookup"><span data-stu-id="bc567-164">String</span></span>|<span data-ttu-id="bc567-165">OS のエディションを指定する文字列。</span><span class="sxs-lookup"><span data-stu-id="bc567-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="bc567-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="bc567-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="bc567-167">String</span><span class="sxs-lookup"><span data-stu-id="bc567-167">String</span></span>|<span data-ttu-id="bc567-168">(存在する場合) は、デバイスの完全修飾ドメイン名を返します。</span><span class="sxs-lookup"><span data-stu-id="bc567-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="bc567-169">デバイスがドメインに参加していない場合は、空の文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="bc567-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="bc567-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="bc567-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="bc567-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="bc567-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="bc567-172">仮想化ベースのセキュリティ ハードウェアの要件の状態です。</span><span class="sxs-lookup"><span data-stu-id="bc567-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="bc567-173">可能な値は、`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable` です。</span><span class="sxs-lookup"><span data-stu-id="bc567-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="bc567-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="bc567-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="bc567-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="bc567-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="bc567-176">仮想化ベースのセキュリティの状態です。</span><span class="sxs-lookup"><span data-stu-id="bc567-176">Virtualization-based security status.</span></span> <span data-ttu-id="bc567-177">.</span><span class="sxs-lookup"><span data-stu-id="bc567-177"></span></span> <span data-ttu-id="bc567-178">可能な値は、`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="bc567-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="bc567-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="bc567-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="bc567-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="bc567-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="bc567-181">ローカル システム機関 (LSA) の資格情報のガード状態です。</span><span class="sxs-lookup"><span data-stu-id="bc567-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="bc567-182">.</span><span class="sxs-lookup"><span data-stu-id="bc567-182"></span></span> <span data-ttu-id="bc567-183">可能な値は、`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning` です。</span><span class="sxs-lookup"><span data-stu-id="bc567-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc567-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bc567-184">Relationships</span></span>
<span data-ttu-id="bc567-185">なし</span><span class="sxs-lookup"><span data-stu-id="bc567-185">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc567-186">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bc567-186">JSON Representation</span></span>
<span data-ttu-id="bc567-187">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bc567-187">Here is a JSON representation of the resource.</span></span>
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




