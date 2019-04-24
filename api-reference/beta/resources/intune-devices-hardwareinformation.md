---
title: ハードウェア情報リソースの種類
description: 特定のデバイスのハードウェア情報。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c751b6601c296b01be91792105325e10a52ea2f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522483"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="04036-103">ハードウェア情報リソースの種類</span><span class="sxs-lookup"><span data-stu-id="04036-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="04036-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04036-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04036-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04036-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04036-106">特定のデバイスのハードウェア情報。</span><span class="sxs-lookup"><span data-stu-id="04036-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="04036-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04036-107">Properties</span></span>
|<span data-ttu-id="04036-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04036-108">Property</span></span>|<span data-ttu-id="04036-109">型</span><span class="sxs-lookup"><span data-stu-id="04036-109">Type</span></span>|<span data-ttu-id="04036-110">説明</span><span class="sxs-lookup"><span data-stu-id="04036-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04036-111">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="04036-111">serialNumber</span></span>|<span data-ttu-id="04036-112">String</span><span class="sxs-lookup"><span data-stu-id="04036-112">String</span></span>|<span data-ttu-id="04036-113">シリアル番号です。</span><span class="sxs-lookup"><span data-stu-id="04036-113">Serial number.</span></span>|
|<span data-ttu-id="04036-114">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="04036-114">totalStorageSpace</span></span>|<span data-ttu-id="04036-115">Int64</span><span class="sxs-lookup"><span data-stu-id="04036-115">Int64</span></span>|<span data-ttu-id="04036-116">デバイスの記憶領域の合計。</span><span class="sxs-lookup"><span data-stu-id="04036-116">Total storage space of the device.</span></span>|
|<span data-ttu-id="04036-117">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="04036-117">freeStorageSpace</span></span>|<span data-ttu-id="04036-118">Int64</span><span class="sxs-lookup"><span data-stu-id="04036-118">Int64</span></span>|<span data-ttu-id="04036-119">デバイスの記憶域スペースを解放します。</span><span class="sxs-lookup"><span data-stu-id="04036-119">Free storage space of the device.</span></span>|
|<span data-ttu-id="04036-120">imei</span><span class="sxs-lookup"><span data-stu-id="04036-120">imei</span></span>|<span data-ttu-id="04036-121">String</span><span class="sxs-lookup"><span data-stu-id="04036-121">String</span></span>|<span data-ttu-id="04036-122">IMEI</span><span class="sxs-lookup"><span data-stu-id="04036-122">IMEI</span></span>|
|<span data-ttu-id="04036-123">meid</span><span class="sxs-lookup"><span data-stu-id="04036-123">meid</span></span>|<span data-ttu-id="04036-124">String</span><span class="sxs-lookup"><span data-stu-id="04036-124">String</span></span>|<span data-ttu-id="04036-125">MEID</span><span class="sxs-lookup"><span data-stu-id="04036-125">MEID</span></span>|
|<span data-ttu-id="04036-126">manufacturer</span><span class="sxs-lookup"><span data-stu-id="04036-126">manufacturer</span></span>|<span data-ttu-id="04036-127">String</span><span class="sxs-lookup"><span data-stu-id="04036-127">String</span></span>|<span data-ttu-id="04036-128">デバイスのメーカー</span><span class="sxs-lookup"><span data-stu-id="04036-128">Manufacturer of the device</span></span>|
|<span data-ttu-id="04036-129">model</span><span class="sxs-lookup"><span data-stu-id="04036-129">model</span></span>|<span data-ttu-id="04036-130">String</span><span class="sxs-lookup"><span data-stu-id="04036-130">String</span></span>|<span data-ttu-id="04036-131">デバイスのモデル</span><span class="sxs-lookup"><span data-stu-id="04036-131">Model of the device</span></span>|
|<span data-ttu-id="04036-132">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="04036-132">phoneNumber</span></span>|<span data-ttu-id="04036-133">String</span><span class="sxs-lookup"><span data-stu-id="04036-133">String</span></span>|<span data-ttu-id="04036-134">デバイスの電話番号</span><span class="sxs-lookup"><span data-stu-id="04036-134">Phone number of the device</span></span>|
|<span data-ttu-id="04036-135">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="04036-135">subscriberCarrier</span></span>|<span data-ttu-id="04036-136">String</span><span class="sxs-lookup"><span data-stu-id="04036-136">String</span></span>|<span data-ttu-id="04036-137">デバイスのサブスクライバーキャリア</span><span class="sxs-lookup"><span data-stu-id="04036-137">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="04036-138">cellulartechnology</span><span class="sxs-lookup"><span data-stu-id="04036-138">cellularTechnology</span></span>|<span data-ttu-id="04036-139">String</span><span class="sxs-lookup"><span data-stu-id="04036-139">String</span></span>|<span data-ttu-id="04036-140">デバイスの携帯電話テクノロジ</span><span class="sxs-lookup"><span data-stu-id="04036-140">Cellular technology of the device</span></span>|
|<span data-ttu-id="04036-141">wifiMac</span><span class="sxs-lookup"><span data-stu-id="04036-141">wifiMac</span></span>|<span data-ttu-id="04036-142">String</span><span class="sxs-lookup"><span data-stu-id="04036-142">String</span></span>|<span data-ttu-id="04036-143">デバイスの WiFi MAC アドレス</span><span class="sxs-lookup"><span data-stu-id="04036-143">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="04036-144">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="04036-144">operatingSystemLanguage</span></span>|<span data-ttu-id="04036-145">String</span><span class="sxs-lookup"><span data-stu-id="04036-145">String</span></span>|<span data-ttu-id="04036-146">デバイスのオペレーティングシステムの言語</span><span class="sxs-lookup"><span data-stu-id="04036-146">Operating system language of the device</span></span>|
|<span data-ttu-id="04036-147">isSupervised</span><span class="sxs-lookup"><span data-stu-id="04036-147">isSupervised</span></span>|<span data-ttu-id="04036-148">ブール型</span><span class="sxs-lookup"><span data-stu-id="04036-148">Boolean</span></span>|<span data-ttu-id="04036-149">デバイスの監視モード</span><span class="sxs-lookup"><span data-stu-id="04036-149">Supervised mode of the device</span></span>|
|<span data-ttu-id="04036-150">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="04036-150">isEncrypted</span></span>|<span data-ttu-id="04036-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="04036-151">Boolean</span></span>|<span data-ttu-id="04036-152">デバイスの暗号化の状態</span><span class="sxs-lookup"><span data-stu-id="04036-152">Encryption status of the device</span></span>|
|<span data-ttu-id="04036-153">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="04036-153">isSharedDevice</span></span>|<span data-ttu-id="04036-154">ブール型</span><span class="sxs-lookup"><span data-stu-id="04036-154">Boolean</span></span>|<span data-ttu-id="04036-155">共有 iPad</span><span class="sxs-lookup"><span data-stu-id="04036-155">Shared iPad</span></span>|
|<span data-ttu-id="04036-156">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="04036-156">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="04036-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="04036-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="04036-158">共有 Apple デバイス上のすべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="04036-158">All users on the shared Apple device</span></span>|
|<span data-ttu-id="04036-159">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="04036-159">tpmSpecificationVersion</span></span>|<span data-ttu-id="04036-160">String</span><span class="sxs-lookup"><span data-stu-id="04036-160">String</span></span>|<span data-ttu-id="04036-161">仕様バージョンを指定する文字列。</span><span class="sxs-lookup"><span data-stu-id="04036-161">String that specifies the specification version.</span></span>|
|<span data-ttu-id="04036-162">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="04036-162">operatingSystemEdition</span></span>|<span data-ttu-id="04036-163">String</span><span class="sxs-lookup"><span data-stu-id="04036-163">String</span></span>|<span data-ttu-id="04036-164">OS のエディションを指定する文字列。</span><span class="sxs-lookup"><span data-stu-id="04036-164">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="04036-165">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="04036-165">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="04036-166">String</span><span class="sxs-lookup"><span data-stu-id="04036-166">String</span></span>|<span data-ttu-id="04036-167">デバイスの完全修飾ドメイン名を返します (存在する場合)。</span><span class="sxs-lookup"><span data-stu-id="04036-167">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="04036-168">デバイスがドメインに参加していない場合は、空の文字列が返されます。</span><span class="sxs-lookup"><span data-stu-id="04036-168">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="04036-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="04036-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="04036-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="04036-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="04036-171">仮想化ベースのセキュリティハードウェア要件の状態。</span><span class="sxs-lookup"><span data-stu-id="04036-171">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="04036-172">可能な値は、`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable` です。</span><span class="sxs-lookup"><span data-stu-id="04036-172">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="04036-173">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="04036-173">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="04036-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="04036-174">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="04036-175">仮想化ベースのセキュリティの状態。</span><span class="sxs-lookup"><span data-stu-id="04036-175">Virtualization-based security status.</span></span> <span data-ttu-id="04036-176">.</span><span class="sxs-lookup"><span data-stu-id="04036-176"></span></span> <span data-ttu-id="04036-177">可能な値は、`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other` です。</span><span class="sxs-lookup"><span data-stu-id="04036-177">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="04036-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="04036-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="04036-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="04036-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="04036-180">ローカルシステム権限 (LSA) credential guard の状態。</span><span class="sxs-lookup"><span data-stu-id="04036-180">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="04036-181">.</span><span class="sxs-lookup"><span data-stu-id="04036-181"></span></span> <span data-ttu-id="04036-182">可能な値は、`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning` です。</span><span class="sxs-lookup"><span data-stu-id="04036-182">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04036-183">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="04036-183">Relationships</span></span>
<span data-ttu-id="04036-184">なし</span><span class="sxs-lookup"><span data-stu-id="04036-184">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04036-185">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="04036-185">JSON Representation</span></span>
<span data-ttu-id="04036-186">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="04036-186">Here is a JSON representation of the resource.</span></span>
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





