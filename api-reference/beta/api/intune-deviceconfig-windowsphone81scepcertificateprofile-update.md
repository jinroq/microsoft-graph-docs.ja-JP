---
title: WindowsPhone81SCEPCertificateProfile を更新します。
description: WindowsPhone81SCEPCertificateProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e41cd55846cf5a87bfa8b43aaef31e6a7b1eb245
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29404695"
---
# <a name="update-windowsphone81scepcertificateprofile"></a><span data-ttu-id="23c5f-103">WindowsPhone81SCEPCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="23c5f-103">Update windowsPhone81SCEPCertificateProfile</span></span>

> <span data-ttu-id="23c5f-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23c5f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23c5f-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23c5f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23c5f-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23c5f-107">[WindowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="23c5f-107">Update the properties of a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="23c5f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="23c5f-108">Prerequisites</span></span>
<span data-ttu-id="23c5f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23c5f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="23c5f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23c5f-111">Permission type</span></span>|<span data-ttu-id="23c5f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="23c5f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23c5f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23c5f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23c5f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23c5f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="23c5f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23c5f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23c5f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23c5f-116">Not supported.</span></span>|
|<span data-ttu-id="23c5f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23c5f-117">Application</span></span>|<span data-ttu-id="23c5f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23c5f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23c5f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23c5f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="23c5f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23c5f-120">Request headers</span></span>
|<span data-ttu-id="23c5f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23c5f-121">Header</span></span>|<span data-ttu-id="23c5f-122">値</span><span class="sxs-lookup"><span data-stu-id="23c5f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23c5f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23c5f-123">Authorization</span></span>|<span data-ttu-id="23c5f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="23c5f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23c5f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="23c5f-125">Accept</span></span>|<span data-ttu-id="23c5f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="23c5f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23c5f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="23c5f-127">Request body</span></span>
<span data-ttu-id="23c5f-128">要求の本文に[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="23c5f-128">In the request body, supply a JSON representation for the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object.</span></span>

<span data-ttu-id="23c5f-129">[WindowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="23c5f-129">The following table shows the properties that are required when you create the [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

|<span data-ttu-id="23c5f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23c5f-130">Property</span></span>|<span data-ttu-id="23c5f-131">型</span><span class="sxs-lookup"><span data-stu-id="23c5f-131">Type</span></span>|<span data-ttu-id="23c5f-132">説明</span><span class="sxs-lookup"><span data-stu-id="23c5f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23c5f-133">id</span><span class="sxs-lookup"><span data-stu-id="23c5f-133">id</span></span>|<span data-ttu-id="23c5f-134">String</span><span class="sxs-lookup"><span data-stu-id="23c5f-134">String</span></span>|<span data-ttu-id="23c5f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="23c5f-135">Key of the entity.</span></span> <span data-ttu-id="23c5f-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23c5f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23c5f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="23c5f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="23c5f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23c5f-138">DateTimeOffset</span></span>|<span data-ttu-id="23c5f-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="23c5f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="23c5f-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23c5f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23c5f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="23c5f-141">roleScopeTagIds</span></span>|<span data-ttu-id="23c5f-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="23c5f-142">String collection</span></span>|<span data-ttu-id="23c5f-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="23c5f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="23c5f-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23c5f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23c5f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="23c5f-145">supportsScopeTags</span></span>|<span data-ttu-id="23c5f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="23c5f-146">Boolean</span></span>|<span data-ttu-id="23c5f-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="23c5f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="23c5f-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="23c5f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="23c5f-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="23c5f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="23c5f-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-150">This property is read-only.</span></span> <span data-ttu-id="23c5f-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23c5f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23c5f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="23c5f-152">createdDateTime</span></span>|<span data-ttu-id="23c5f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23c5f-153">DateTimeOffset</span></span>|<span data-ttu-id="23c5f-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="23c5f-154">DateTime the object was created.</span></span> <span data-ttu-id="23c5f-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23c5f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23c5f-156">説明</span><span class="sxs-lookup"><span data-stu-id="23c5f-156">description</span></span>|<span data-ttu-id="23c5f-157">String</span><span class="sxs-lookup"><span data-stu-id="23c5f-157">String</span></span>|<span data-ttu-id="23c5f-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="23c5f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="23c5f-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23c5f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23c5f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="23c5f-160">displayName</span></span>|<span data-ttu-id="23c5f-161">String</span><span class="sxs-lookup"><span data-stu-id="23c5f-161">String</span></span>|<span data-ttu-id="23c5f-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="23c5f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="23c5f-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23c5f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23c5f-164">version</span><span class="sxs-lookup"><span data-stu-id="23c5f-164">version</span></span>|<span data-ttu-id="23c5f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="23c5f-165">Int32</span></span>|<span data-ttu-id="23c5f-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="23c5f-166">Version of the device configuration.</span></span> <span data-ttu-id="23c5f-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="23c5f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="23c5f-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="23c5f-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="23c5f-169">Int32</span><span class="sxs-lookup"><span data-stu-id="23c5f-169">Int32</span></span>|<span data-ttu-id="23c5f-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="23c5f-171">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="23c5f-171">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="23c5f-172">keyStorageProvider</span><span class="sxs-lookup"><span data-stu-id="23c5f-172">keyStorageProvider</span></span>|[<span data-ttu-id="23c5f-173">keyStorageProviderOption</span><span class="sxs-lookup"><span data-stu-id="23c5f-173">keyStorageProviderOption</span></span>](../resources/intune-deviceconfig-keystorageprovideroption.md)|<span data-ttu-id="23c5f-174">キー記憶域プロバイダー (KSP)。</span><span class="sxs-lookup"><span data-stu-id="23c5f-174">Key Storage Provider (KSP).</span></span> <span data-ttu-id="23c5f-175">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="23c5f-175">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="23c5f-176">可能な値は、`useTpmKspOtherwiseUseSoftwareKsp`、`useTpmKspOtherwiseFail`、`usePassportForWorkKspOtherwiseFail`、`useSoftwareKsp` です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-176">Possible values are: `useTpmKspOtherwiseUseSoftwareKsp`, `useTpmKspOtherwiseFail`, `usePassportForWorkKspOtherwiseFail`, `useSoftwareKsp`.</span></span>|
|<span data-ttu-id="23c5f-177">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="23c5f-177">subjectNameFormat</span></span>|[<span data-ttu-id="23c5f-178">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="23c5f-178">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="23c5f-179">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-179">Certificate Subject Name Format.</span></span> <span data-ttu-id="23c5f-180">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="23c5f-180">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="23c5f-181">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-181">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="23c5f-182">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="23c5f-182">subjectAlternativeNameType</span></span>|[<span data-ttu-id="23c5f-183">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="23c5f-183">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="23c5f-184">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-184">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="23c5f-185">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="23c5f-185">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="23c5f-186">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-186">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="23c5f-187">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="23c5f-187">certificateValidityPeriodValue</span></span>|<span data-ttu-id="23c5f-188">Int32</span><span class="sxs-lookup"><span data-stu-id="23c5f-188">Int32</span></span>|<span data-ttu-id="23c5f-189">証明書 Validtiy の期間の値です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-189">Value for the Certificate Validtiy Period.</span></span> <span data-ttu-id="23c5f-190">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="23c5f-190">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="23c5f-191">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="23c5f-191">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="23c5f-192">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="23c5f-192">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="23c5f-193">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="23c5f-193">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="23c5f-194">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="23c5f-194">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md).</span></span> <span data-ttu-id="23c5f-195">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-195">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="23c5f-196">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="23c5f-196">extendedKeyUsages</span></span>|<span data-ttu-id="23c5f-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="23c5f-197">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="23c5f-198">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="23c5f-198">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="23c5f-199">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="23c5f-199">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="23c5f-200">[WindowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="23c5f-200">Inherited from [windowsPhone81CertificateProfileBase](../resources/intune-deviceconfig-windowsphone81certificateprofilebase.md)</span></span>|
|<span data-ttu-id="23c5f-201">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="23c5f-201">scepServerUrls</span></span>|<span data-ttu-id="23c5f-202">String コレクション</span><span class="sxs-lookup"><span data-stu-id="23c5f-202">String collection</span></span>|<span data-ttu-id="23c5f-203">SCEP サーバー個の url。</span><span class="sxs-lookup"><span data-stu-id="23c5f-203">SCEP Server Url(s).</span></span>|
|<span data-ttu-id="23c5f-204">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="23c5f-204">subjectNameFormatString</span></span>|<span data-ttu-id="23c5f-205">String</span><span class="sxs-lookup"><span data-stu-id="23c5f-205">String</span></span>|<span data-ttu-id="23c5f-206">SubjectNameFormat で使用するカスタム書式指定 = カスタムです。</span><span class="sxs-lookup"><span data-stu-id="23c5f-206">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="23c5f-207">例: CN = EmailAddress {{}}、E = EmailAddress {{}}、OU = エンタープライズ ユーザーの場合は、O = コントソ株式会社、L = Redmond、ST = ワシントン州 C = u. s.</span><span class="sxs-lookup"><span data-stu-id="23c5f-207">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="23c5f-208">keyUsage</span><span class="sxs-lookup"><span data-stu-id="23c5f-208">keyUsage</span></span>|[<span data-ttu-id="23c5f-209">keyUsages</span><span class="sxs-lookup"><span data-stu-id="23c5f-209">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="23c5f-210">SCEP のキー使用法です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-210">SCEP Key Usage.</span></span> <span data-ttu-id="23c5f-211">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-211">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="23c5f-212">キー長</span><span class="sxs-lookup"><span data-stu-id="23c5f-212">keySize</span></span>|[<span data-ttu-id="23c5f-213">キー長</span><span class="sxs-lookup"><span data-stu-id="23c5f-213">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="23c5f-214">SCEP のキー サイズ。</span><span class="sxs-lookup"><span data-stu-id="23c5f-214">SCEP Key Size.</span></span> <span data-ttu-id="23c5f-215">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-215">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="23c5f-216">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="23c5f-216">hashAlgorithm</span></span>|[<span data-ttu-id="23c5f-217">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="23c5f-217">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="23c5f-218">SCEP ハッシュ アルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="23c5f-218">SCEP Hash Algorithm.</span></span> <span data-ttu-id="23c5f-219">使用可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-219">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="23c5f-220">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="23c5f-220">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="23c5f-221">String</span><span class="sxs-lookup"><span data-stu-id="23c5f-221">String</span></span>|<span data-ttu-id="23c5f-222">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="23c5f-222">Custom String that defines the AAD Attribute.</span></span>|



## <a name="response"></a><span data-ttu-id="23c5f-223">応答</span><span class="sxs-lookup"><span data-stu-id="23c5f-223">Response</span></span>
<span data-ttu-id="23c5f-224">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="23c5f-224">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23c5f-225">例</span><span class="sxs-lookup"><span data-stu-id="23c5f-225">Example</span></span>

### <a name="request"></a><span data-ttu-id="23c5f-226">要求</span><span class="sxs-lookup"><span data-stu-id="23c5f-226">Request</span></span>
<span data-ttu-id="23c5f-227">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23c5f-227">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="23c5f-228">応答</span><span class="sxs-lookup"><span data-stu-id="23c5f-228">Response</span></span>
<span data-ttu-id="23c5f-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="23c5f-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




