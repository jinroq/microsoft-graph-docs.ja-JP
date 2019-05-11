---
title: deviceEnrollmentWindowsHelloForBusinessConfiguration の更新
description: deviceEnrollmentWindowsHelloForBusinessConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bd2eea7a906fcad21b52250971f12a5087971ce1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33900160"
---
# <a name="update-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="a2e58-103">deviceEnrollmentWindowsHelloForBusinessConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="a2e58-103">Update deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="a2e58-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2e58-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2e58-106">[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-106">Update the properties of a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2e58-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2e58-107">Prerequisites</span></span>
<span data-ttu-id="a2e58-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2e58-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2e58-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2e58-110">Permission type</span></span>|<span data-ttu-id="a2e58-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2e58-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2e58-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2e58-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2e58-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2e58-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a2e58-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2e58-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2e58-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-115">Not supported.</span></span>|
|<span data-ttu-id="a2e58-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2e58-116">Application</span></span>|<span data-ttu-id="a2e58-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2e58-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2e58-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a2e58-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2e58-119">Request headers</span></span>
|<span data-ttu-id="a2e58-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2e58-120">Header</span></span>|<span data-ttu-id="a2e58-121">値</span><span class="sxs-lookup"><span data-stu-id="a2e58-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2e58-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2e58-122">Authorization</span></span>|<span data-ttu-id="a2e58-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2e58-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a2e58-124">Accept</span></span>|<span data-ttu-id="a2e58-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2e58-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2e58-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2e58-126">Request body</span></span>
<span data-ttu-id="a2e58-127">要求本文で、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-127">In the request body, supply a JSON representation for the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object.</span></span>

<span data-ttu-id="a2e58-128">次の表に、[deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-128">The following table shows the properties that are required when you create the [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

|<span data-ttu-id="a2e58-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2e58-129">Property</span></span>|<span data-ttu-id="a2e58-130">型</span><span class="sxs-lookup"><span data-stu-id="a2e58-130">Type</span></span>|<span data-ttu-id="a2e58-131">説明</span><span class="sxs-lookup"><span data-stu-id="a2e58-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2e58-132">id</span><span class="sxs-lookup"><span data-stu-id="a2e58-132">id</span></span>|<span data-ttu-id="a2e58-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a2e58-133">String</span></span>|<span data-ttu-id="a2e58-134">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたアカウントの一意識別子</span><span class="sxs-lookup"><span data-stu-id="a2e58-134">Unique Identifier for the account Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a2e58-135">displayName</span><span class="sxs-lookup"><span data-stu-id="a2e58-135">displayName</span></span>|<span data-ttu-id="a2e58-136">String</span><span class="sxs-lookup"><span data-stu-id="a2e58-136">String</span></span>|<span data-ttu-id="a2e58-137">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の表示名。</span><span class="sxs-lookup"><span data-stu-id="a2e58-137">The display name of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a2e58-138">description</span><span class="sxs-lookup"><span data-stu-id="a2e58-138">description</span></span>|<span data-ttu-id="a2e58-139">String</span><span class="sxs-lookup"><span data-stu-id="a2e58-139">String</span></span>|<span data-ttu-id="a2e58-140">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の説明</span><span class="sxs-lookup"><span data-stu-id="a2e58-140">The description of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a2e58-141">priority</span><span class="sxs-lookup"><span data-stu-id="a2e58-141">priority</span></span>|<span data-ttu-id="a2e58-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a2e58-142">Int32</span></span>|<span data-ttu-id="a2e58-143">優先度は、登録構成が割り当てられている複数のグループにユーザーが存在するときに使用されます。</span><span class="sxs-lookup"><span data-stu-id="a2e58-143">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="a2e58-144">ユーザーは、優先度の低い値を持つ構成のみに適用されます。</span><span class="sxs-lookup"><span data-stu-id="a2e58-144">Users are subject only to the configuration with the lowest priority value.</span></span> <span data-ttu-id="a2e58-145">[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a2e58-145">Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a2e58-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e58-146">createdDateTime</span></span>|<span data-ttu-id="a2e58-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e58-147">DateTimeOffset</span></span>|<span data-ttu-id="a2e58-148">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承された、デバイス登録構成の日時を UTC として作成した日時</span><span class="sxs-lookup"><span data-stu-id="a2e58-148">Created date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a2e58-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2e58-149">lastModifiedDateTime</span></span>|<span data-ttu-id="a2e58-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2e58-150">DateTimeOffset</span></span>|<span data-ttu-id="a2e58-151">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成の最終変更日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="a2e58-151">Last modified date time in UTC of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a2e58-152">version</span><span class="sxs-lookup"><span data-stu-id="a2e58-152">version</span></span>|<span data-ttu-id="a2e58-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a2e58-153">Int32</span></span>|<span data-ttu-id="a2e58-154">[DeviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)から継承されたデバイス登録構成のバージョン</span><span class="sxs-lookup"><span data-stu-id="a2e58-154">The version of the device enrollment configuration Inherited from [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="a2e58-155">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a2e58-155">pinMinimumLength</span></span>|<span data-ttu-id="a2e58-156">Int32</span><span class="sxs-lookup"><span data-stu-id="a2e58-156">Int32</span></span>|<span data-ttu-id="a2e58-157">Windows Hello for Business の PIN に必要な最小文字数を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-157">Controls the minimum number of characters required for the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a2e58-158">この値は、4 ~ 127 の範囲で、最大 PIN の値よりも小さいか等しい必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2e58-158">This value must be between 4 and 127, inclusive, and less than or equal to the value set for the maximum PIN.</span></span>|
|<span data-ttu-id="a2e58-159">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="a2e58-159">pinMaximumLength</span></span>|<span data-ttu-id="a2e58-160">Int32</span><span class="sxs-lookup"><span data-stu-id="a2e58-160">Int32</span></span>|<span data-ttu-id="a2e58-161">Windows Hello for Business の PIN に使用できる最大文字数を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-161">Controls the maximum number of characters allowed for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="a2e58-162">この値は、4 ~ 127 の範囲にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2e58-162">This value must be between 4 and 127, inclusive.</span></span> <span data-ttu-id="a2e58-163">この値は、最小 PIN の値より大きいか等しい必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2e58-163">This value must be greater than or equal to the value set for the minimum PIN.</span></span>|
|<span data-ttu-id="a2e58-164">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a2e58-164">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="a2e58-165">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a2e58-165">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a2e58-166">Windows Hello for Business の PIN で大文字を使用する機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-166">Controls the ability to use uppercase letters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a2e58-167">[許可] 大文字/小文字の使用が許可されますが、必要であれば必ず存在することを確認します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-167">Allowed permits the use of uppercase letter(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="a2e58-168">[許可しない] に設定した場合、大文字は使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-168">If set to Not Allowed, uppercase letters will not be permitted.</span></span> <span data-ttu-id="a2e58-169">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-169">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a2e58-170">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a2e58-170">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="a2e58-171">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a2e58-171">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a2e58-172">Windows Hello for Business の PIN で小文字を使用する機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-172">Controls the ability to use lowercase letters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a2e58-173">許可されている場合は小文字の使用が許可されますが、必要であれば必ず存在することを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a2e58-173">Allowed permits the use of lowercase letter(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="a2e58-174">[許可しない] に設定した場合、小文字は使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-174">If set to Not Allowed, lowercase letters will not be permitted.</span></span> <span data-ttu-id="a2e58-175">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-175">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a2e58-176">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="a2e58-176">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="a2e58-177">windowsHelloForBusinessPinUsage</span><span class="sxs-lookup"><span data-stu-id="a2e58-177">windowsHelloForBusinessPinUsage</span></span>](../resources/intune-onboarding-windowshelloforbusinesspinusage.md)|<span data-ttu-id="a2e58-178">Windows Hello for Business の PIN で特殊文字を使用する機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-178">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a2e58-179">許可されている場合、特殊文字の使用が許可されますが、必要に応じて存在することが保証されます。</span><span class="sxs-lookup"><span data-stu-id="a2e58-179">Allowed permits the use of special character(s), whereas Required ensures they are present.</span></span> <span data-ttu-id="a2e58-180">[許可しない] に設定した場合、特殊文字は使用できません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-180">If set to Not Allowed, special character(s) will not be permitted.</span></span> <span data-ttu-id="a2e58-181">可能な値は、`allowed`、`required`、`disallowed` です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-181">Possible values are: `allowed`, `required`, `disallowed`.</span></span>|
|<span data-ttu-id="a2e58-182">state</span><span class="sxs-lookup"><span data-stu-id="a2e58-182">state</span></span>|[<span data-ttu-id="a2e58-183">購入</span><span class="sxs-lookup"><span data-stu-id="a2e58-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a2e58-184">Windows Hello for Business 用にデバイスを構成することを許可するかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-184">Controls whether to allow the device to be configured for Windows Hello for Business.</span></span> <span data-ttu-id="a2e58-185">[無効] に設定されている場合、ユーザーは、必要に応じて、Azure Active Directory に参加しているモバイル電話を除き、Windows Hello for Business をプロビジョニングすることはできません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-185">If set to disabled, the user cannot provision Windows Hello for Business except on Azure Active Directory joined mobile phones if otherwise required.</span></span> <span data-ttu-id="a2e58-186">未構成に設定した場合、Intune はクライアントの既定値を上書きしません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-186">If set to Not Configured, Intune will not override client defaults.</span></span> <span data-ttu-id="a2e58-187">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-187">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a2e58-188">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="a2e58-188">securityDeviceRequired</span></span>|<span data-ttu-id="a2e58-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2e58-189">Boolean</span></span>|<span data-ttu-id="a2e58-190">Windows Hello for Business のプロビジョニングにトラステッドプラットフォームモジュール (TPM) を必要とするかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-190">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="a2e58-191">TPM に格納されたデータは、他のデバイスでは使用できないため、追加のセキュリティ上の利点があります。</span><span class="sxs-lookup"><span data-stu-id="a2e58-191">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="a2e58-192">False に設定されている場合は、使用可能な TPM がない場合でも、すべてのデバイスが Windows Hello for Business をプロビジョニングできます。</span><span class="sxs-lookup"><span data-stu-id="a2e58-192">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="a2e58-193">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="a2e58-193">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="a2e58-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2e58-194">Boolean</span></span>|<span data-ttu-id="a2e58-195">Windows Hello for Business PIN の代わりに、顔文字や指紋などのバイオメトリクスジェスチャの使用を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-195">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="a2e58-196">False に設定すると、生体認証ジェスチャは許可されません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-196">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="a2e58-197">ユーザーは、障害が発生した場合に、バックアップとして PIN を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2e58-197">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="a2e58-198">remotePassportEnabled</span><span class="sxs-lookup"><span data-stu-id="a2e58-198">remotePassportEnabled</span></span>|<span data-ttu-id="a2e58-199">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="a2e58-199">Boolean</span></span>|<span data-ttu-id="a2e58-200">リモートの Windows Hello for Business の使用を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-200">Controls the use of Remote Windows Hello for Business.</span></span> <span data-ttu-id="a2e58-201">リモート Windows Hello for Business は、デスクトップ認証のコンパニオンとして使用できる、ポータブルで登録されたデバイスの機能を提供します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-201">Remote Windows Hello for Business provides the ability for a portable, registered device to be usable as a companion for desktop authentication.</span></span> <span data-ttu-id="a2e58-202">デスクトップは Azure AD に参加している必要があります。コンパニオンデバイスには、Windows Hello for Business の PIN が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-202">The desktop must be Azure AD joined and the companion device must have a Windows Hello for Business PIN.</span></span>|
|<span data-ttu-id="a2e58-203">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="a2e58-203">pinPreviousBlockCount</span></span>|<span data-ttu-id="a2e58-204">Int32</span><span class="sxs-lookup"><span data-stu-id="a2e58-204">Int32</span></span>|<span data-ttu-id="a2e58-205">ユーザーが過去の Pin を使用できないようにする機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-205">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="a2e58-206">0 ~ 50 の範囲で設定する必要があり、ユーザーの現在の PIN がその数に含まれています。</span><span class="sxs-lookup"><span data-stu-id="a2e58-206">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="a2e58-207">0に設定すると、以前の Pin は保存されません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-207">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="a2e58-208">Pin をリセットすると、PIN 履歴は保持されません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-208">PIN history is not preserved through a PIN reset.</span></span>|
|<span data-ttu-id="a2e58-209">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="a2e58-209">pinExpirationInDays</span></span>|<span data-ttu-id="a2e58-210">Int32</span><span class="sxs-lookup"><span data-stu-id="a2e58-210">Int32</span></span>|<span data-ttu-id="a2e58-211">ユーザーがシステムに PIN を変更することを要求するまでの時間 (日数) を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-211">Controls the period of time (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="a2e58-212">0 ~ 730 の範囲で設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a2e58-212">This must be set between 0 and 730, inclusive.</span></span> <span data-ttu-id="a2e58-213">0に設定すると、ユーザーの PIN は期限切れになりません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-213">If set to 0, the user's PIN will never expire</span></span>|
|<span data-ttu-id="a2e58-214">enhancedBiometricsState</span><span class="sxs-lookup"><span data-stu-id="a2e58-214">enhancedBiometricsState</span></span>|[<span data-ttu-id="a2e58-215">購入</span><span class="sxs-lookup"><span data-stu-id="a2e58-215">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a2e58-216">この機能をサポートするデバイス上の顔認識に対して、スプーフィング対策機能を使用する機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-216">Controls the ability to use the anti-spoofing features for facial recognition on devices which support it.</span></span> <span data-ttu-id="a2e58-217">Disabled に設定した場合、スプーフィング対策機能は許可されません。</span><span class="sxs-lookup"><span data-stu-id="a2e58-217">If set to disabled, anti-spoofing features are not allowed.</span></span> <span data-ttu-id="a2e58-218">[未構成] に設定した場合、ユーザーはスプーフィング対策を使用するかどうかを選択できます。</span><span class="sxs-lookup"><span data-stu-id="a2e58-218">If set to Not Configured, the user can choose whether they want to use anti-spoofing.</span></span> <span data-ttu-id="a2e58-219">可能な値は、`notConfigured`、`enabled`、`disabled` です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-219">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="a2e58-220">応答</span><span class="sxs-lookup"><span data-stu-id="a2e58-220">Response</span></span>
<span data-ttu-id="a2e58-221">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="a2e58-221">If successful, this method returns a `200 OK` response code and an updated [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2e58-222">例</span><span class="sxs-lookup"><span data-stu-id="a2e58-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2e58-223">要求</span><span class="sxs-lookup"><span data-stu-id="a2e58-223">Request</span></span>
<span data-ttu-id="a2e58-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2e58-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
Content-type: application/json
Content-length: 629

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="a2e58-225">応答</span><span class="sxs-lookup"><span data-stu-id="a2e58-225">Response</span></span>
<span data-ttu-id="a2e58-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2e58-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 801

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentWindowsHelloForBusinessConfiguration",
  "id": "3068e0cd-e0cd-3068-cde0-6830cde06830",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "state": "enabled",
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "remotePassportEnabled": true,
  "pinPreviousBlockCount": 5,
  "pinExpirationInDays": 3,
  "enhancedBiometricsState": "enabled"
}
```




