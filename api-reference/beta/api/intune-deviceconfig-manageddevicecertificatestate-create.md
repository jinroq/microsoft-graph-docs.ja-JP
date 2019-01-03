---
title: ManagedDeviceCertificateState を作成します。
description: 新しい managedDeviceCertificateState オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 22b8a0db82e86b9136ee997a821223afe608b51a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305958"
---
# <a name="create-manageddevicecertificatestate"></a><span data-ttu-id="fe711-103">ManagedDeviceCertificateState を作成します。</span><span class="sxs-lookup"><span data-stu-id="fe711-103">Create managedDeviceCertificateState</span></span>

> <span data-ttu-id="fe711-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe711-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe711-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe711-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fe711-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fe711-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fe711-107">新しい[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fe711-107">Create a new [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fe711-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fe711-108">Prerequisites</span></span>
<span data-ttu-id="fe711-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe711-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe711-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fe711-111">Permission type</span></span>|<span data-ttu-id="fe711-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fe711-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fe711-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fe711-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fe711-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe711-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fe711-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fe711-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fe711-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe711-116">Not supported.</span></span>|
|<span data-ttu-id="fe711-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fe711-117">Application</span></span>|<span data-ttu-id="fe711-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe711-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe711-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fe711-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="fe711-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe711-120">Request headers</span></span>
|<span data-ttu-id="fe711-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fe711-121">Header</span></span>|<span data-ttu-id="fe711-122">値</span><span class="sxs-lookup"><span data-stu-id="fe711-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fe711-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe711-123">Authorization</span></span>|<span data-ttu-id="fe711-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fe711-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fe711-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fe711-125">Accept</span></span>|<span data-ttu-id="fe711-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fe711-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fe711-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fe711-127">Request body</span></span>
<span data-ttu-id="fe711-128">要求の本文に managedDeviceCertificateState オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="fe711-128">In the request body, supply a JSON representation for the managedDeviceCertificateState object.</span></span>

<span data-ttu-id="fe711-129">次の表は、managedDeviceCertificateState を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fe711-129">The following table shows the properties that are required when you create the managedDeviceCertificateState.</span></span>

|<span data-ttu-id="fe711-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe711-130">Property</span></span>|<span data-ttu-id="fe711-131">種類</span><span class="sxs-lookup"><span data-stu-id="fe711-131">Type</span></span>|<span data-ttu-id="fe711-132">説明</span><span class="sxs-lookup"><span data-stu-id="fe711-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe711-133">ID</span><span class="sxs-lookup"><span data-stu-id="fe711-133">id</span></span>|<span data-ttu-id="fe711-134">String</span><span class="sxs-lookup"><span data-stu-id="fe711-134">String</span></span>|<span data-ttu-id="fe711-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fe711-135">Key of the entity.</span></span>|
|<span data-ttu-id="fe711-136">devicePlatform</span><span class="sxs-lookup"><span data-stu-id="fe711-136">devicePlatform</span></span>|[<span data-ttu-id="fe711-137">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="fe711-137">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="fe711-138">デバイスのプラットフォームです。</span><span class="sxs-lookup"><span data-stu-id="fe711-138">Device platform.</span></span> <span data-ttu-id="fe711-139">可能な値は、`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile` です。</span><span class="sxs-lookup"><span data-stu-id="fe711-139">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="fe711-140">certificateKeyUsage</span><span class="sxs-lookup"><span data-stu-id="fe711-140">certificateKeyUsage</span></span>|[<span data-ttu-id="fe711-141">keyUsages</span><span class="sxs-lookup"><span data-stu-id="fe711-141">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="fe711-142">キーの使用法です。</span><span class="sxs-lookup"><span data-stu-id="fe711-142">Key usage.</span></span> <span data-ttu-id="fe711-143">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="fe711-143">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="fe711-144">certificateValidityPeriodUnits</span><span class="sxs-lookup"><span data-stu-id="fe711-144">certificateValidityPeriodUnits</span></span>|[<span data-ttu-id="fe711-145">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="fe711-145">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="fe711-146">有効期間の単位。</span><span class="sxs-lookup"><span data-stu-id="fe711-146">Validity period units.</span></span> <span data-ttu-id="fe711-147">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="fe711-147">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="fe711-148">certificateIssuanceState</span><span class="sxs-lookup"><span data-stu-id="fe711-148">certificateIssuanceState</span></span>|[<span data-ttu-id="fe711-149">certificateIssuanceStates</span><span class="sxs-lookup"><span data-stu-id="fe711-149">certificateIssuanceStates</span></span>](../resources/intune-deviceconfig-certificateissuancestates.md)|<span data-ttu-id="fe711-150">発行の状態です。</span><span class="sxs-lookup"><span data-stu-id="fe711-150">Issuance State.</span></span> <span data-ttu-id="fe711-151">使用可能な値: `unknown`、 `challengeIssued`、 `challengeIssueFailed`、 `requestCreationFailed`、 `requestSubmitFailed`、 `challengeValidationSucceeded`、 `challengeValidationFailed`、 `issueFailed`、 `issuePending`、 `issued`、 `responseProcessingFailed`、 `responsePending`、 `enrollmentSucceeded`、 `enrollmentNotNeeded`、 `revoked`、 `removedFromCollection`、 `renewVerified`、 `installFailed`、 `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span><span class="sxs-lookup"><span data-stu-id="fe711-151">Possible values are: `unknown`, `challengeIssued`, `challengeIssueFailed`, `requestCreationFailed`, `requestSubmitFailed`, `challengeValidationSucceeded`, `challengeValidationFailed`, `issueFailed`, `issuePending`, `issued`, `responseProcessingFailed`, `responsePending`, `enrollmentSucceeded`, `enrollmentNotNeeded`, `revoked`, `removedFromCollection`, `renewVerified`, `installFailed`, `installed`, `deleteFailed`, `deleted`, `renewalRequested`, `requested`.</span></span>|
|<span data-ttu-id="fe711-152">certificateKeyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="fe711-152">certificateKeyStorageProvider</span></span>|[<span data-ttu-id="fe711-153">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="fe711-153">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="fe711-154">キー記憶域プロバイダーです。</span><span class="sxs-lookup"><span data-stu-id="fe711-154">Key Storage Provider.</span></span> <span data-ttu-id="fe711-155">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="fe711-155">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="fe711-156">certificateSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fe711-156">certificateSubjectNameFormat</span></span>|[<span data-ttu-id="fe711-157">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="fe711-157">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="fe711-158">サブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="fe711-158">Subject name format.</span></span> <span data-ttu-id="fe711-159">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="fe711-159">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="fe711-160">certificateSubjectAlternativeNameFormat</span><span class="sxs-lookup"><span data-stu-id="fe711-160">certificateSubjectAlternativeNameFormat</span></span>|[<span data-ttu-id="fe711-161">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="fe711-161">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="fe711-162">サブジェクト代替名の形式です。</span><span class="sxs-lookup"><span data-stu-id="fe711-162">Subject alternative name format.</span></span> <span data-ttu-id="fe711-163">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="fe711-163">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="fe711-164">certificateRevokeStatus</span><span class="sxs-lookup"><span data-stu-id="fe711-164">certificateRevokeStatus</span></span>|[<span data-ttu-id="fe711-165">certificateRevocationStatus</span><span class="sxs-lookup"><span data-stu-id="fe711-165">certificateRevocationStatus</span></span>](../resources/intune-deviceconfig-certificaterevocationstatus.md)|<span data-ttu-id="fe711-166">状態を無効にします。</span><span class="sxs-lookup"><span data-stu-id="fe711-166">Revoke status.</span></span> <span data-ttu-id="fe711-167">可能な値は、`none`、`pending`、`issued`、`failed`、`revoked` です。</span><span class="sxs-lookup"><span data-stu-id="fe711-167">Possible values are: `none`, `pending`, `issued`, `failed`, `revoked`.</span></span>|
|<span data-ttu-id="fe711-168">certificateProfileDisplayName</span><span class="sxs-lookup"><span data-stu-id="fe711-168">certificateProfileDisplayName</span></span>|<span data-ttu-id="fe711-169">String</span><span class="sxs-lookup"><span data-stu-id="fe711-169">String</span></span>|<span data-ttu-id="fe711-170">証明書プロファイルの表示名</span><span class="sxs-lookup"><span data-stu-id="fe711-170">Certificate profile display name</span></span>|
|<span data-ttu-id="fe711-171">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fe711-171">deviceDisplayName</span></span>|<span data-ttu-id="fe711-172">String</span><span class="sxs-lookup"><span data-stu-id="fe711-172">String</span></span>|<span data-ttu-id="fe711-173">デバイスの表示名</span><span class="sxs-lookup"><span data-stu-id="fe711-173">Device display name</span></span>|
|<span data-ttu-id="fe711-174">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="fe711-174">userDisplayName</span></span>|<span data-ttu-id="fe711-175">String</span><span class="sxs-lookup"><span data-stu-id="fe711-175">String</span></span>|<span data-ttu-id="fe711-176">ユーザーの表示名</span><span class="sxs-lookup"><span data-stu-id="fe711-176">User display name</span></span>|
|<span data-ttu-id="fe711-177">certificateExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="fe711-177">certificateExpirationDateTime</span></span>|<span data-ttu-id="fe711-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe711-178">DateTimeOffset</span></span>|<span data-ttu-id="fe711-179">証明書の有効期限</span><span class="sxs-lookup"><span data-stu-id="fe711-179">Certificate expiry date</span></span>|
|<span data-ttu-id="fe711-180">certificateLastIssuanceStateChangedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe711-180">certificateLastIssuanceStateChangedDateTime</span></span>|<span data-ttu-id="fe711-181">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe711-181">DateTimeOffset</span></span>|<span data-ttu-id="fe711-182">最後の証明書の発行状態の変更</span><span class="sxs-lookup"><span data-stu-id="fe711-182">Last certificate issuance state change</span></span>|
|<span data-ttu-id="fe711-183">lastCertificateStateChangeDateTime</span><span class="sxs-lookup"><span data-stu-id="fe711-183">lastCertificateStateChangeDateTime</span></span>|<span data-ttu-id="fe711-184">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe711-184">DateTimeOffset</span></span>|<span data-ttu-id="fe711-185">最後の証明書の発行状態の変更</span><span class="sxs-lookup"><span data-stu-id="fe711-185">Last certificate issuance state change</span></span>|
|<span data-ttu-id="fe711-186">certificateIssuer</span><span class="sxs-lookup"><span data-stu-id="fe711-186">certificateIssuer</span></span>|<span data-ttu-id="fe711-187">String</span><span class="sxs-lookup"><span data-stu-id="fe711-187">String</span></span>|<span data-ttu-id="fe711-188">発行者</span><span class="sxs-lookup"><span data-stu-id="fe711-188">Issuer</span></span>|
|<span data-ttu-id="fe711-189">certificateThumbprint</span><span class="sxs-lookup"><span data-stu-id="fe711-189">certificateThumbprint</span></span>|<span data-ttu-id="fe711-190">String</span><span class="sxs-lookup"><span data-stu-id="fe711-190">String</span></span>|<span data-ttu-id="fe711-191">拇印</span><span class="sxs-lookup"><span data-stu-id="fe711-191">Thumbprint</span></span>|
|<span data-ttu-id="fe711-192">certificateSerialNumber</span><span class="sxs-lookup"><span data-stu-id="fe711-192">certificateSerialNumber</span></span>|<span data-ttu-id="fe711-193">String</span><span class="sxs-lookup"><span data-stu-id="fe711-193">String</span></span>|<span data-ttu-id="fe711-194">シリアル番号</span><span class="sxs-lookup"><span data-stu-id="fe711-194">Serial number</span></span>|
|<span data-ttu-id="fe711-195">certificateKeyLength</span><span class="sxs-lookup"><span data-stu-id="fe711-195">certificateKeyLength</span></span>|<span data-ttu-id="fe711-196">Int32</span><span class="sxs-lookup"><span data-stu-id="fe711-196">Int32</span></span>|<span data-ttu-id="fe711-197">キーの長さ</span><span class="sxs-lookup"><span data-stu-id="fe711-197">Key length</span></span>|
|<span data-ttu-id="fe711-198">certificateEnhancedKeyUsage</span><span class="sxs-lookup"><span data-stu-id="fe711-198">certificateEnhancedKeyUsage</span></span>|<span data-ttu-id="fe711-199">String</span><span class="sxs-lookup"><span data-stu-id="fe711-199">String</span></span>|<span data-ttu-id="fe711-200">拡張キー使用法</span><span class="sxs-lookup"><span data-stu-id="fe711-200">Extended key usage</span></span>|
|<span data-ttu-id="fe711-201">certificateValidityPeriod</span><span class="sxs-lookup"><span data-stu-id="fe711-201">certificateValidityPeriod</span></span>|<span data-ttu-id="fe711-202">Int32</span><span class="sxs-lookup"><span data-stu-id="fe711-202">Int32</span></span>|<span data-ttu-id="fe711-203">有効期間</span><span class="sxs-lookup"><span data-stu-id="fe711-203">Validity period</span></span>|
|<span data-ttu-id="fe711-204">certificateSubjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fe711-204">certificateSubjectNameFormatString</span></span>|<span data-ttu-id="fe711-205">String</span><span class="sxs-lookup"><span data-stu-id="fe711-205">String</span></span>|<span data-ttu-id="fe711-206">カスタム サブジェクト名の形式のサブジェクト名の形式の文字列</span><span class="sxs-lookup"><span data-stu-id="fe711-206">Subject name format string for custom subject name formats</span></span>|
|<span data-ttu-id="fe711-207">certificateSubjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="fe711-207">certificateSubjectAlternativeNameFormatString</span></span>|<span data-ttu-id="fe711-208">String</span><span class="sxs-lookup"><span data-stu-id="fe711-208">String</span></span>|<span data-ttu-id="fe711-209">カスタム書式のサブジェクト代替名の書式指定文字列</span><span class="sxs-lookup"><span data-stu-id="fe711-209">Subject alternative name format string for custom formats</span></span>|
|<span data-ttu-id="fe711-210">certificateIssuanceDateTime</span><span class="sxs-lookup"><span data-stu-id="fe711-210">certificateIssuanceDateTime</span></span>|<span data-ttu-id="fe711-211">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe711-211">DateTimeOffset</span></span>|<span data-ttu-id="fe711-212">発行日</span><span class="sxs-lookup"><span data-stu-id="fe711-212">Issuance date</span></span>|
|<span data-ttu-id="fe711-213">certificateErrorCode</span><span class="sxs-lookup"><span data-stu-id="fe711-213">certificateErrorCode</span></span>|<span data-ttu-id="fe711-214">Int32</span><span class="sxs-lookup"><span data-stu-id="fe711-214">Int32</span></span>|<span data-ttu-id="fe711-215">エラー コード</span><span class="sxs-lookup"><span data-stu-id="fe711-215">Error code</span></span>|



## <a name="response"></a><span data-ttu-id="fe711-216">応答</span><span class="sxs-lookup"><span data-stu-id="fe711-216">Response</span></span>
<span data-ttu-id="fe711-217">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="fe711-217">If successful, this method returns a `201 Created` response code and a [managedDeviceCertificateState](../resources/intune-deviceconfig-manageddevicecertificatestate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fe711-218">例</span><span class="sxs-lookup"><span data-stu-id="fe711-218">Example</span></span>
### <a name="request"></a><span data-ttu-id="fe711-219">要求</span><span class="sxs-lookup"><span data-stu-id="fe711-219">Request</span></span>
<span data-ttu-id="fe711-220">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fe711-220">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fe711-221">応答</span><span class="sxs-lookup"><span data-stu-id="fe711-221">Response</span></span>
<span data-ttu-id="fe711-p111">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fe711-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




