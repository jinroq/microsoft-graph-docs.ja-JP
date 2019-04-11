---
title: managedDeviceCertificateState を作成する
description: 新しい managedDeviceCertificateState オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3510ca1d4f4d593ea0bb396d5fe34c56cf2ac5f5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31806077"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="2093f-103">managedDeviceCertificateState を作成する</span><span class="sxs-lookup"><span data-stu-id="2093f-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="2093f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2093f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2093f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2093f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2093f-106">新しい[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2093f-106">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2093f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="2093f-107">Prerequisites</span></span>
<span data-ttu-id="2093f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2093f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2093f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2093f-110">Permission type</span></span>|<span data-ttu-id="2093f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2093f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2093f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2093f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2093f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2093f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2093f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2093f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2093f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2093f-115">Not supported.</span></span>|
|<span data-ttu-id="2093f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2093f-116">Application</span></span>|<span data-ttu-id="2093f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2093f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2093f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2093f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidWorkProfileScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidForWorkImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkPkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/microsoft.graph.androidForWorkScepCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10PkcsCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows81SCEPCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windows10ImportedPFXCertificateProfile/managedDeviceCertificateStates
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/microsoft.graph.windowsPhone81ImportedPFXCertificateProfile/managedDeviceCertificateStates
```

## <a name="request-headers"></a><span data-ttu-id="2093f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2093f-119">Request headers</span></span>
|<span data-ttu-id="2093f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2093f-120">Header</span></span>|<span data-ttu-id="2093f-121">値</span><span class="sxs-lookup"><span data-stu-id="2093f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2093f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2093f-122">Authorization</span></span>|<span data-ttu-id="2093f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2093f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2093f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="2093f-124">Accept</span></span>|<span data-ttu-id="2093f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2093f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2093f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="2093f-126">Request body</span></span>
<span data-ttu-id="2093f-127">要求本文で、managedDeviceCertificateState オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2093f-127">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="2093f-128">次の表に、managedDeviceCertificateState の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2093f-128">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="2093f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2093f-129">Property</span></span>|<span data-ttu-id="2093f-130">型</span><span class="sxs-lookup"><span data-stu-id="2093f-130">Type</span></span>|<span data-ttu-id="2093f-131">説明</span><span class="sxs-lookup"><span data-stu-id="2093f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2093f-132">id</span><span class="sxs-lookup"><span data-stu-id="2093f-132">id</span></span>|<span data-ttu-id="2093f-133">String</span><span class="sxs-lookup"><span data-stu-id="2093f-133">String</span></span>|<span data-ttu-id="2093f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2093f-134">Key of the entity.</span></span>|
|<span data-ttu-id="2093f-135">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="2093f-135">devicePlatform</span></span>|[<span data-ttu-id="2093f-136">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="2093f-136">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="2093f-137">デバイスプラットフォーム。</span><span class="sxs-lookup"><span data-stu-id="2093f-137">Device platform.</span></span> <span data-ttu-id="2093f-138">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="2093f-138">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="2093f-139">certificatekeyusage</span><span class="sxs-lookup"><span data-stu-id="2093f-139">certificateKeyUsage</span></span>|[<span data-ttu-id="2093f-140">keyusages</span><span class="sxs-lookup"><span data-stu-id="2093f-140">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="2093f-141">キー使用法。</span><span class="sxs-lookup"><span data-stu-id="2093f-141">Key usage.</span></span> <span data-ttu-id="2093f-142">可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="2093f-142">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="2093f-143">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="2093f-143">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="2093f-144">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="2093f-144">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="2093f-145">有効期間の単位。</span><span class="sxs-lookup"><span data-stu-id="2093f-145">Validity period units.</span></span> <span data-ttu-id="2093f-146">使用可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="2093f-146">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="2093f-147">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="2093f-147">certificateIssuanceState</span></span>|[<span data-ttu-id="2093f-148">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="2093f-148">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="2093f-149">発行状態。</span><span class="sxs-lookup"><span data-stu-id="2093f-149">Issuance State.</span></span> <span data-ttu-id="2093f-150">可能な値: `unknown`、 `challengeIssued` `challengeIssueFailed` `requestCreationFailed` `requestSubmitFailed` `challengeValidationSucceeded` `challengeValidationFailed` `issueFailed` `issuePending` `issued` `responseProcessingFailed` `responsePending`、、、、、、、、、、、、 `enrollmentSucceeded` `enrollmentNotNeeded` `revoked` `removedFromCollection` `renewVerified` `installFailed` `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="2093f-150">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="2093f-151">certificatekeystorageprovider</span><span class="sxs-lookup"><span data-stu-id="2093f-151">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="2093f-152">keystorageprovideroption</span><span class="sxs-lookup"><span data-stu-id="2093f-152">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="2093f-153">キーストレージプロバイダー。</span><span class="sxs-lookup"><span data-stu-id="2093f-153">Key Storage Provider.</span></span> <span data-ttu-id="2093f-154">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="2093f-154">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="2093f-155">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2093f-155">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="2093f-156">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="2093f-156">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="2093f-157">サブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="2093f-157">Subject name format.</span></span> <span data-ttu-id="2093f-158">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="2093f-158">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="2093f-159">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="2093f-159">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="2093f-160">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="2093f-160">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="2093f-161">サブジェクトの別名形式。</span><span class="sxs-lookup"><span data-stu-id="2093f-161">Subject alternative name format.</span></span> <span data-ttu-id="2093f-162">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="2093f-162">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="2093f-163">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="2093f-163">certificateRevokeStatus</span></span>|[<span data-ttu-id="2093f-164">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="2093f-164">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="2093f-165">状態を取り消します。</span><span class="sxs-lookup"><span data-stu-id="2093f-165">Revoke status.</span></span> <span data-ttu-id="2093f-166">可能な値は、`none`、`pending`、`issued`、`failed`、`revoked` です。</span><span class="sxs-lookup"><span data-stu-id="2093f-166">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="2093f-167">certificateprofiledisplayname</span><span class="sxs-lookup"><span data-stu-id="2093f-167">certificateProfileDisplayName</span></span>|<span data-ttu-id="2093f-168">文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-168">String</span></span>|<span data-ttu-id="2093f-169">証明書プロファイルの表示名</span><span class="sxs-lookup"><span data-stu-id="2093f-169">Certificate profile display name</span></span>|
|<span data-ttu-id="2093f-170">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="2093f-170">deviceDisplayName</span></span>|<span data-ttu-id="2093f-171">String</span><span class="sxs-lookup"><span data-stu-id="2093f-171">String</span></span>|<span data-ttu-id="2093f-172">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="2093f-172">Device display name</span></span>|
|<span data-ttu-id="2093f-173">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="2093f-173">userDisplayName</span></span>|<span data-ttu-id="2093f-174">String</span><span class="sxs-lookup"><span data-stu-id="2093f-174">String</span></span>|<span data-ttu-id="2093f-175">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="2093f-175">User display name</span></span>|
|<span data-ttu-id="2093f-176">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2093f-176">certificateExpirationDateTime</span></span>|<span data-ttu-id="2093f-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2093f-177">DateTimeOffset</span></span>|<span data-ttu-id="2093f-178">証明書の有効期限</span><span class="sxs-lookup"><span data-stu-id="2093f-178">Certificate expiry date</span></span>|
|<span data-ttu-id="2093f-179">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="2093f-179">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="2093f-180">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2093f-180">DateTimeOffset</span></span>|<span data-ttu-id="2093f-181">証明書の発行状態の最終変更</span><span class="sxs-lookup"><span data-stu-id="2093f-181">Last certificate issuance state change</span></span>|
|<span data-ttu-id="2093f-182">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="2093f-182">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="2093f-183">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2093f-183">DateTimeOffset</span></span>|<span data-ttu-id="2093f-184">証明書の発行状態の最終変更</span><span class="sxs-lookup"><span data-stu-id="2093f-184">Last certificate issuance state change</span></span>|
|<span data-ttu-id="2093f-185">certificateissuer</span><span class="sxs-lookup"><span data-stu-id="2093f-185">certificateIssuer</span></span>|<span data-ttu-id="2093f-186">文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-186">String</span></span>|<span data-ttu-id="2093f-187">発行者</span><span class="sxs-lookup"><span data-stu-id="2093f-187">Issuer</span></span>|
|<span data-ttu-id="2093f-188">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="2093f-188">certificateThumbprint</span></span>|<span data-ttu-id="2093f-189">文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-189">String</span></span>|<span data-ttu-id="2093f-190">拇印</span><span class="sxs-lookup"><span data-stu-id="2093f-190">Thumbprint</span></span>|
|<span data-ttu-id="2093f-191">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="2093f-191">certificateSerialNumber</span></span>|<span data-ttu-id="2093f-192">文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-192">String</span></span>|<span data-ttu-id="2093f-193">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="2093f-193">Serial number</span></span>|
|<span data-ttu-id="2093f-194">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="2093f-194">certificateKeyLength</span></span>|<span data-ttu-id="2093f-195">Int32</span><span class="sxs-lookup"><span data-stu-id="2093f-195">Int32</span></span>|<span data-ttu-id="2093f-196">キーの長さ</span><span class="sxs-lookup"><span data-stu-id="2093f-196">Key length</span></span>|
|<span data-ttu-id="2093f-197">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="2093f-197">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="2093f-198">文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-198">String</span></span>|<span data-ttu-id="2093f-199">拡張キーの使用</span><span class="sxs-lookup"><span data-stu-id="2093f-199">Extended key usage</span></span>|
|<span data-ttu-id="2093f-200">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="2093f-200">certificateValidityPeriod</span></span>|<span data-ttu-id="2093f-201">Int32</span><span class="sxs-lookup"><span data-stu-id="2093f-201">Int32</span></span>|<span data-ttu-id="2093f-202">有効期間</span><span class="sxs-lookup"><span data-stu-id="2093f-202">Validity period</span></span>|
|<span data-ttu-id="2093f-203">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="2093f-203">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="2093f-204">文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-204">String</span></span>|<span data-ttu-id="2093f-205">カスタムサブジェクト名の形式のサブジェクト名の書式指定文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-205">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="2093f-206">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="2093f-206">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="2093f-207">文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-207">String</span></span>|<span data-ttu-id="2093f-208">カスタム書式のサブジェクトの別名書式文字列</span><span class="sxs-lookup"><span data-stu-id="2093f-208">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="2093f-209">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="2093f-209">certificateIssuanceDateTime</span></span>|<span data-ttu-id="2093f-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2093f-210">DateTimeOffset</span></span>|<span data-ttu-id="2093f-211">発行日</span><span class="sxs-lookup"><span data-stu-id="2093f-211">Issuance date</span></span>|
|<span data-ttu-id="2093f-212">certificateerrorcode</span><span class="sxs-lookup"><span data-stu-id="2093f-212">certificateErrorCode</span></span>|<span data-ttu-id="2093f-213">Int32</span><span class="sxs-lookup"><span data-stu-id="2093f-213">Int32</span></span>|<span data-ttu-id="2093f-214">エラー コード</span><span class="sxs-lookup"><span data-stu-id="2093f-214">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="2093f-215">応答</span><span class="sxs-lookup"><span data-stu-id="2093f-215">Response</span></span>
<span data-ttu-id="2093f-216">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2093f-216">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2093f-217">例</span><span class="sxs-lookup"><span data-stu-id="2093f-217">Example</span></span>

### <a name="request"></a><span data-ttu-id="2093f-218">要求</span><span class="sxs-lookup"><span data-stu-id="2093f-218">Request</span></span>
<span data-ttu-id="2093f-219">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2093f-219">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosPkcsCertificateProfile/managedDeviceCertificateStates
Content-type: application/json
Content-length: 1517

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```

### <a name="response"></a><span data-ttu-id="2093f-220">応答</span><span class="sxs-lookup"><span data-stu-id="2093f-220">Response</span></span>
<span data-ttu-id="2093f-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2093f-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1566

{
  "@odata.type": "#microsoft.graph.managedDeviceCertificateState",
  "id": "d99bc884-c884-d99b-84c8-9bd984c89bd9",
  "devicePlatform": "androidForWork",
  "certificateKeyUsage": "digitalSignature",
  "certificateValidityPeriodUnits": "months",
  "certificateIssuanceState": "challengeIssued",
  "certificateKeyStorageProvider": "useTpmKspOtherwiseFail",
  "certificateSubjectNameFormat": "commonNameIncludingEmail",
  "certificateSubjectAlternativeNameFormat": "emailAddress",
  "certificateRevokeStatus": "pending",
  "certificateProfileDisplayName": "Certificate Profile Display Name value",
  "deviceDisplayName": "Device Display Name value",
  "userDisplayName": "User Display Name value",
  "certificateExpirationDateTime": "2017-01-01T00:02:14.9489247-08:00",
  "certificateLastIssuanceStateChangedDateTime": "2017-01-01T00:00:27.7468732-08:00",
  "lastCertificateStateChangeDateTime": "2017-01-01T00:01:10.7144639-08:00",
  "certificateIssuer": "Certificate Issuer value",
  "certificateThumbprint": "Certificate Thumbprint value",
  "certificateSerialNumber": "Certificate Serial Number value",
  "certificateKeyLength": 4,
  "certificateEnhancedKeyUsage": "Certificate Enhanced Key Usage value",
  "certificateValidityPeriod": 9,
  "certificateSubjectNameFormatString": "Certificate Subject Name Format String value",
  "certificateSubjectAlternativeNameFormatString": "Certificate Subject Alternative Name Format String value",
  "certificateIssuanceDateTime": "2016-12-31T23:59:41.5044473-08:00",
  "certificateErrorCode": 4
}
```





