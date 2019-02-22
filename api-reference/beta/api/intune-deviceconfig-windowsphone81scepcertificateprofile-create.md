---
title: windowsPhone81SCEPCertificateProfile を作成する
description: 新しい windowsPhone81SCEPCertificateProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4755179f8b659588ca8068f89735ce3637d92ef0
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144885"
---
# <a name="create-windowsphone81scepcertificateprofile"></a><span data-ttu-id="32f7a-103">windowsPhone81SCEPCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="32f7a-103">Create windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="32f7a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32f7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32f7a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32f7a-106">新しい[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="32f7a-106">Create a new [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="32f7a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="32f7a-107">Prerequisites</span></span>
<span data-ttu-id="32f7a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="32f7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="32f7a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="32f7a-110">Permission type</span></span>|<span data-ttu-id="32f7a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="32f7a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="32f7a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="32f7a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="32f7a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="32f7a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="32f7a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="32f7a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="32f7a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32f7a-115">Not supported.</span></span>|
|<span data-ttu-id="32f7a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="32f7a-116">Application</span></span>|<span data-ttu-id="32f7a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="32f7a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="32f7a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="32f7a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="32f7a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32f7a-119">Request headers</span></span>
|<span data-ttu-id="32f7a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="32f7a-120">Header</span></span>|<span data-ttu-id="32f7a-121">値</span><span class="sxs-lookup"><span data-stu-id="32f7a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="32f7a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="32f7a-122">Authorization</span></span>|<span data-ttu-id="32f7a-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="32f7a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="32f7a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="32f7a-124">Accept</span></span>|<span data-ttu-id="32f7a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="32f7a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="32f7a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="32f7a-126">Request body</span></span>
<span data-ttu-id="32f7a-127">要求本文で、windowsPhone81SCEPCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="32f7a-127">In the request body, supply a JSON representation for the windowsPhone81SCEPCertificateProfile object.</span></span>

<span data-ttu-id="32f7a-128">次の表に、windowsPhone81SCEPCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="32f7a-128">The following table shows the properties that are required when you create the windowsPhone81SCEPCertificateProfile.</span></span>

|<span data-ttu-id="32f7a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32f7a-129">Property</span></span>|<span data-ttu-id="32f7a-130">型</span><span class="sxs-lookup"><span data-stu-id="32f7a-130">Type</span></span>|<span data-ttu-id="32f7a-131">説明</span><span class="sxs-lookup"><span data-stu-id="32f7a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32f7a-132">id</span><span class="sxs-lookup"><span data-stu-id="32f7a-132">id</span></span>|<span data-ttu-id="32f7a-133">文字列</span><span class="sxs-lookup"><span data-stu-id="32f7a-133">String</span></span>|<span data-ttu-id="32f7a-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="32f7a-134">Key of the entity.</span></span> <span data-ttu-id="32f7a-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32f7a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f7a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="32f7a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="32f7a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32f7a-137">DateTimeOffset</span></span>|<span data-ttu-id="32f7a-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="32f7a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="32f7a-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32f7a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f7a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="32f7a-140">roleScopeTagIds</span></span>|<span data-ttu-id="32f7a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="32f7a-141">String collection</span></span>|<span data-ttu-id="32f7a-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="32f7a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="32f7a-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32f7a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f7a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="32f7a-144">supportsScopeTags</span></span>|<span data-ttu-id="32f7a-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="32f7a-145">Boolean</span></span>|<span data-ttu-id="32f7a-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="32f7a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="32f7a-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="32f7a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="32f7a-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="32f7a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="32f7a-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-149">This property is read-only.</span></span> <span data-ttu-id="32f7a-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32f7a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f7a-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="32f7a-151">createdDateTime</span></span>|<span data-ttu-id="32f7a-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32f7a-152">DateTimeOffset</span></span>|<span data-ttu-id="32f7a-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="32f7a-153">DateTime the object was created.</span></span> <span data-ttu-id="32f7a-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32f7a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f7a-155">説明</span><span class="sxs-lookup"><span data-stu-id="32f7a-155">description</span></span>|<span data-ttu-id="32f7a-156">String</span><span class="sxs-lookup"><span data-stu-id="32f7a-156">String</span></span>|<span data-ttu-id="32f7a-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="32f7a-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="32f7a-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32f7a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f7a-159">displayName</span><span class="sxs-lookup"><span data-stu-id="32f7a-159">displayName</span></span>|<span data-ttu-id="32f7a-160">String</span><span class="sxs-lookup"><span data-stu-id="32f7a-160">String</span></span>|<span data-ttu-id="32f7a-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="32f7a-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="32f7a-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32f7a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f7a-163">version</span><span class="sxs-lookup"><span data-stu-id="32f7a-163">version</span></span>|<span data-ttu-id="32f7a-164">Int32</span><span class="sxs-lookup"><span data-stu-id="32f7a-164">Int32</span></span>|<span data-ttu-id="32f7a-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="32f7a-165">Version of the device configuration.</span></span> <span data-ttu-id="32f7a-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="32f7a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="32f7a-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="32f7a-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="32f7a-168">Int32</span><span class="sxs-lookup"><span data-stu-id="32f7a-168">Int32</span></span>|<span data-ttu-id="32f7a-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="32f7a-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="32f7a-170">[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="32f7a-170">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="32f7a-171">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="32f7a-171">keyStorageProvider</span></span>|[<span data-ttu-id="32f7a-172">keystorageprovideroption</span><span class="sxs-lookup"><span data-stu-id="32f7a-172">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="32f7a-173">キーストレージプロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="32f7a-173">Key Storage Provider (KSP).</span></span> <span data-ttu-id="32f7a-174">[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="32f7a-174">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="32f7a-175">使用可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-175">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="32f7a-176">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="32f7a-176">subjectNameFormat</span></span>|[<span data-ttu-id="32f7a-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="32f7a-177">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="32f7a-178">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="32f7a-178">Certificate Subject Name Format.</span></span> <span data-ttu-id="32f7a-179">[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="32f7a-179">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="32f7a-180">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-180">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="32f7a-181">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="32f7a-181">subjectAlternativeNameType</span></span>|[<span data-ttu-id="32f7a-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="32f7a-182">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="32f7a-183">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="32f7a-183">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="32f7a-184">[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="32f7a-184">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="32f7a-185">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-185">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="32f7a-186">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="32f7a-186">certificateValidityPeriodValue</span></span>|<span data-ttu-id="32f7a-187">Int32</span><span class="sxs-lookup"><span data-stu-id="32f7a-187">Int32</span></span>|<span data-ttu-id="32f7a-188">証明書の validtiy の値。</span><span class="sxs-lookup"><span data-stu-id="32f7a-188">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="32f7a-189">[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="32f7a-189">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="32f7a-190">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="32f7a-190">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="32f7a-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="32f7a-191">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="32f7a-192">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="32f7a-192">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="32f7a-193">[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="32f7a-193">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="32f7a-194">可能な値は `days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-194">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="32f7a-195">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="32f7a-195">extendedKeyUsages</span></span>|<span data-ttu-id="32f7a-196">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="32f7a-196">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="32f7a-197">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="32f7a-197">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="32f7a-198">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="32f7a-198">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="32f7a-199">[windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="32f7a-199">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="32f7a-200">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="32f7a-200">scepServerUrls</span></span>|<span data-ttu-id="32f7a-201">String collection</span><span class="sxs-lookup"><span data-stu-id="32f7a-201">String collection</span></span>|<span data-ttu-id="32f7a-202">SCEP サーバーの Url。</span><span class="sxs-lookup"><span data-stu-id="32f7a-202">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="32f7a-203">subjectnameformatstring プロパティ</span><span class="sxs-lookup"><span data-stu-id="32f7a-203">subjectNameFormatString</span></span>|<span data-ttu-id="32f7a-204">String</span><span class="sxs-lookup"><span data-stu-id="32f7a-204">String</span></span>|<span data-ttu-id="32f7a-205">SubjectNameFormat = custom で使用するカスタム形式。</span><span class="sxs-lookup"><span data-stu-id="32f7a-205">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="32f7a-206">例: CN = {{EmailAddress}}, E = {{EmailAddress}}, OU = エンタープライズユーザー, O = Contoso Corporation, L = Redmond, ST = WA, C = US</span><span class="sxs-lookup"><span data-stu-id="32f7a-206">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="32f7a-207">keyusage</span><span class="sxs-lookup"><span data-stu-id="32f7a-207">keyUsage</span></span>|[<span data-ttu-id="32f7a-208">keyusages</span><span class="sxs-lookup"><span data-stu-id="32f7a-208">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="32f7a-209">SCEP キーの使用法。</span><span class="sxs-lookup"><span data-stu-id="32f7a-209">SCEP Key Usage.</span></span> <span data-ttu-id="32f7a-210">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-210">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="32f7a-211">keySize</span><span class="sxs-lookup"><span data-stu-id="32f7a-211">keySize</span></span>|[<span data-ttu-id="32f7a-212">keySize</span><span class="sxs-lookup"><span data-stu-id="32f7a-212">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="32f7a-213">SCEP キーのサイズ。</span><span class="sxs-lookup"><span data-stu-id="32f7a-213">SCEP Key Size.</span></span> <span data-ttu-id="32f7a-214">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-214">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="32f7a-215">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="32f7a-215">hashAlgorithm</span></span>|[<span data-ttu-id="32f7a-216">hashalgorithms</span><span class="sxs-lookup"><span data-stu-id="32f7a-216">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="32f7a-217">SCEP ハッシュアルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="32f7a-217">SCEP Hash Algorithm.</span></span> <span data-ttu-id="32f7a-218">使用可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-218">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="32f7a-219">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="32f7a-219">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="32f7a-220">String</span><span class="sxs-lookup"><span data-stu-id="32f7a-220">String</span></span>|<span data-ttu-id="32f7a-221">AAD 属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="32f7a-221">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="32f7a-222">応答</span><span class="sxs-lookup"><span data-stu-id="32f7a-222">Response</span></span>
<span data-ttu-id="32f7a-223">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="32f7a-223">If successful, this method returns a `201 Created` response code and a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="32f7a-224">例</span><span class="sxs-lookup"><span data-stu-id="32f7a-224">Example</span></span>

### <a name="request"></a><span data-ttu-id="32f7a-225">要求</span><span class="sxs-lookup"><span data-stu-id="32f7a-225">Request</span></span>
<span data-ttu-id="32f7a-226">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="32f7a-226">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1032

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```

### <a name="response"></a><span data-ttu-id="32f7a-227">応答</span><span class="sxs-lookup"><span data-stu-id="32f7a-227">Response</span></span>
<span data-ttu-id="32f7a-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="32f7a-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1204

{
  "@odata.type": "#microsoft.graph.windowsPhone81SCEPCertificateProfile",
  "id": "f070e30e-e30e-f070-0ee3-70f00ee370f0",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "keyStorageProvider": "useTpmKspOtherwiseFail",
  "subjectNameFormat": "commonNameIncludingEmail",
  "subjectAlternativeNameType": "emailAddress",
  "certificateValidityPeriodValue": 14,
  "certificateValidityPeriodScale": "months",
  "extendedKeyUsages": [
    {
      "@odata.type": "microsoft.graph.extendedKeyUsage",
      "name": "Name value",
      "objectIdentifier": "Object Identifier value"
    }
  ],
  "scepServerUrls": [
    "Scep Server Urls value"
  ],
  "subjectNameFormatString": "Subject Name Format String value",
  "keyUsage": "digitalSignature",
  "keySize": "size2048",
  "hashAlgorithm": "sha2",
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value"
}
```




