---
title: hardwareInformation リソースの種類
description: 特定のデバイスのハードウェア情報です。
author: tfitzmac
ms.openlocfilehash: c483aa800d920a50392d21c326cd20dea7b72e18
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334525"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="19ab5-103">hardwareInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="19ab5-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="19ab5-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="19ab5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="19ab5-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19ab5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="19ab5-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="19ab5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19ab5-107">特定のデバイスのハードウェア情報です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="19ab5-108">Properties</span><span class="sxs-lookup"><span data-stu-id="19ab5-108">Properties</span></span>
|<span data-ttu-id="19ab5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19ab5-109">Property</span></span>|<span data-ttu-id="19ab5-110">種類</span><span class="sxs-lookup"><span data-stu-id="19ab5-110">Type</span></span>|<span data-ttu-id="19ab5-111">説明</span><span class="sxs-lookup"><span data-stu-id="19ab5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19ab5-112">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="19ab5-112">serialNumber</span></span>|<span data-ttu-id="19ab5-113">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-113">String</span></span>|<span data-ttu-id="19ab5-114">シリアル番号です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-114">Serial number.</span></span>|
|<span data-ttu-id="19ab5-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="19ab5-115">totalStorageSpace</span></span>|<span data-ttu-id="19ab5-116">Int64</span><span class="sxs-lookup"><span data-stu-id="19ab5-116">Int64</span></span>|<span data-ttu-id="19ab5-117">デバイスの合計容量。</span><span class="sxs-lookup"><span data-stu-id="19ab5-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="19ab5-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="19ab5-118">freeStorageSpace</span></span>|<span data-ttu-id="19ab5-119">Int64</span><span class="sxs-lookup"><span data-stu-id="19ab5-119">Int64</span></span>|<span data-ttu-id="19ab5-120">デバイスの空き容量。</span><span class="sxs-lookup"><span data-stu-id="19ab5-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="19ab5-121">imei</span><span class="sxs-lookup"><span data-stu-id="19ab5-121">imei</span></span>|<span data-ttu-id="19ab5-122">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-122">String</span></span>|<span data-ttu-id="19ab5-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="19ab5-123">IMEI</span></span>|
|<span data-ttu-id="19ab5-124">meid</span><span class="sxs-lookup"><span data-stu-id="19ab5-124">meid</span></span>|<span data-ttu-id="19ab5-125">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-125">String</span></span>|<span data-ttu-id="19ab5-126">MEID</span><span class="sxs-lookup"><span data-stu-id="19ab5-126">MEID</span></span>|
|<span data-ttu-id="19ab5-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="19ab5-127">manufacturer</span></span>|<span data-ttu-id="19ab5-128">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-128">String</span></span>|<span data-ttu-id="19ab5-129">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="19ab5-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="19ab5-130">model</span><span class="sxs-lookup"><span data-stu-id="19ab5-130">model</span></span>|<span data-ttu-id="19ab5-131">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-131">String</span></span>|<span data-ttu-id="19ab5-132">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="19ab5-132">Model of the device</span></span>|
|<span data-ttu-id="19ab5-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="19ab5-133">phoneNumber</span></span>|<span data-ttu-id="19ab5-134">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-134">String</span></span>|<span data-ttu-id="19ab5-135">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="19ab5-135">Phone number of the device</span></span>|
|<span data-ttu-id="19ab5-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="19ab5-136">subscriberCarrier</span></span>|<span data-ttu-id="19ab5-137">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-137">String</span></span>|<span data-ttu-id="19ab5-138">デバイスのサブスクライバーのキャリア</span><span class="sxs-lookup"><span data-stu-id="19ab5-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="19ab5-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="19ab5-139">cellularTechnology</span></span>|<span data-ttu-id="19ab5-140">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-140">String</span></span>|<span data-ttu-id="19ab5-141">デバイスの携帯電話のテクノロジー</span><span class="sxs-lookup"><span data-stu-id="19ab5-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="19ab5-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="19ab5-142">wifiMac</span></span>|<span data-ttu-id="19ab5-143">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-143">String</span></span>|<span data-ttu-id="19ab5-144">デバイスの WiFi の MAC アドレス</span><span class="sxs-lookup"><span data-stu-id="19ab5-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="19ab5-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="19ab5-145">operatingSystemLanguage</span></span>|<span data-ttu-id="19ab5-146">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-146">String</span></span>|<span data-ttu-id="19ab5-147">デバイスのオペレーティング システムの言語</span><span class="sxs-lookup"><span data-stu-id="19ab5-147">Operating system language of the device</span></span>|
|<span data-ttu-id="19ab5-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="19ab5-148">isSupervised</span></span>|<span data-ttu-id="19ab5-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="19ab5-149">Boolean</span></span>|<span data-ttu-id="19ab5-150">デバイスのコールを管理モード</span><span class="sxs-lookup"><span data-stu-id="19ab5-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="19ab5-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="19ab5-151">isEncrypted</span></span>|<span data-ttu-id="19ab5-152">ブール型</span><span class="sxs-lookup"><span data-stu-id="19ab5-152">Boolean</span></span>|<span data-ttu-id="19ab5-153">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="19ab5-153">Encryption status of the device</span></span>|
|<span data-ttu-id="19ab5-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="19ab5-154">isSharedDevice</span></span>|<span data-ttu-id="19ab5-155">ブール型</span><span class="sxs-lookup"><span data-stu-id="19ab5-155">Boolean</span></span>|<span data-ttu-id="19ab5-156">IPad の共有</span><span class="sxs-lookup"><span data-stu-id="19ab5-156">Shared iPad</span></span>|
|<span data-ttu-id="19ab5-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="19ab5-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="19ab5-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="19ab5-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="19ab5-159">共有の Apple デバイス上のすべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="19ab5-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="19ab5-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="19ab5-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="19ab5-161">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-161">String</span></span>|<span data-ttu-id="19ab5-162">仕様のバージョンを指定する文字列。</span><span class="sxs-lookup"><span data-stu-id="19ab5-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="19ab5-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="19ab5-163">operatingSystemEdition</span></span>|<span data-ttu-id="19ab5-164">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-164">String</span></span>|<span data-ttu-id="19ab5-165">OS のエディションを指定する文字列。</span><span class="sxs-lookup"><span data-stu-id="19ab5-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="19ab5-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="19ab5-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="19ab5-167">String</span><span class="sxs-lookup"><span data-stu-id="19ab5-167">String</span></span>|<span data-ttu-id="19ab5-168">(存在する場合) は、デバイスの完全修飾ドメイン名を返します。</span><span class="sxs-lookup"><span data-stu-id="19ab5-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="19ab5-169">デバイスがドメインに参加していない場合は、空の文字列を返します。</span><span class="sxs-lookup"><span data-stu-id="19ab5-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="19ab5-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="19ab5-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="19ab5-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="19ab5-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="19ab5-172">仮想化ベースのセキュリティ ハードウェアの要件の状態です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="19ab5-173">可能な値は、`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable` です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="19ab5-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="19ab5-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="19ab5-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="19ab5-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="19ab5-176">仮想化ベースのセキュリティの状態です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-176">Virtualization-based security status.</span></span> <span data-ttu-id="19ab5-177">.</span><span class="sxs-lookup"><span data-stu-id="19ab5-177"></span></span> <span data-ttu-id="19ab5-178">可能な値は、`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="19ab5-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="19ab5-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="19ab5-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="19ab5-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="19ab5-181">ローカル システム機関 (LSA) の資格情報のガード状態です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="19ab5-182">.</span><span class="sxs-lookup"><span data-stu-id="19ab5-182"></span></span> <span data-ttu-id="19ab5-183">可能な値は、`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning` です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="19ab5-184">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="19ab5-184">Relationships</span></span>
<span data-ttu-id="19ab5-185">なし</span><span class="sxs-lookup"><span data-stu-id="19ab5-185">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="19ab5-186">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="19ab5-186">JSON Representation</span></span>
<span data-ttu-id="19ab5-187">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="19ab5-187">Here is a JSON representation of the resource.</span></span>
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





