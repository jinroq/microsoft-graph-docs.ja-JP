---
title: androidForWorkImportedPFXCertificateProfile を作成する
description: 新しい androidForWorkImportedPFXCertificateProfile オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b4c2ffde1683ab2a7100604405d4b35a85d6931
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166900"
---
# <a name="create-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="1ac1c-103">androidForWorkImportedPFXCertificateProfile を作成する</span><span class="sxs-lookup"><span data-stu-id="1ac1c-103">Create androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="1ac1c-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ac1c-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ac1c-106">新しい[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-106">Create a new [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ac1c-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1ac1c-107">Prerequisites</span></span>
<span data-ttu-id="1ac1c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1ac1c-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ac1c-110">Permission type</span></span>|<span data-ttu-id="1ac1c-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ac1c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ac1c-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ac1c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ac1c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ac1c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ac1c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ac1c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ac1c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-115">Not supported.</span></span>|
|<span data-ttu-id="1ac1c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ac1c-116">Application</span></span>|<span data-ttu-id="1ac1c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ac1c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ac1c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1ac1c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ac1c-119">Request headers</span></span>
|<span data-ttu-id="1ac1c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ac1c-120">Header</span></span>|<span data-ttu-id="1ac1c-121">値</span><span class="sxs-lookup"><span data-stu-id="1ac1c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ac1c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ac1c-122">Authorization</span></span>|<span data-ttu-id="1ac1c-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ac1c-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1ac1c-124">Accept</span></span>|<span data-ttu-id="1ac1c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ac1c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ac1c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ac1c-126">Request body</span></span>
<span data-ttu-id="1ac1c-127">要求本文で、androidForWorkImportedPFXCertificateProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-127">In the request body, supply a JSON representation for the androidForWorkImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="1ac1c-128">次の表に、androidForWorkImportedPFXCertificateProfile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-128">The following table shows the properties that are required when you create the androidForWorkImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="1ac1c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ac1c-129">Property</span></span>|<span data-ttu-id="1ac1c-130">型</span><span class="sxs-lookup"><span data-stu-id="1ac1c-130">Type</span></span>|<span data-ttu-id="1ac1c-131">説明</span><span class="sxs-lookup"><span data-stu-id="1ac1c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ac1c-132">id</span><span class="sxs-lookup"><span data-stu-id="1ac1c-132">id</span></span>|<span data-ttu-id="1ac1c-133">文字列</span><span class="sxs-lookup"><span data-stu-id="1ac1c-133">String</span></span>|<span data-ttu-id="1ac1c-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-134">Key of the entity.</span></span> <span data-ttu-id="1ac1c-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ac1c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ac1c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="1ac1c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ac1c-137">DateTimeOffset</span></span>|<span data-ttu-id="1ac1c-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="1ac1c-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ac1c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ac1c-140">roleScopeTagIds</span></span>|<span data-ttu-id="1ac1c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="1ac1c-141">String collection</span></span>|<span data-ttu-id="1ac1c-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1ac1c-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ac1c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1ac1c-144">supportsScopeTags</span></span>|<span data-ttu-id="1ac1c-145">ブール値</span><span class="sxs-lookup"><span data-stu-id="1ac1c-145">Boolean</span></span>|<span data-ttu-id="1ac1c-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1ac1c-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1ac1c-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1ac1c-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-149">This property is read-only.</span></span> <span data-ttu-id="1ac1c-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ac1c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ac1c-151">createdDateTime</span></span>|<span data-ttu-id="1ac1c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ac1c-152">DateTimeOffset</span></span>|<span data-ttu-id="1ac1c-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-153">DateTime the object was created.</span></span> <span data-ttu-id="1ac1c-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ac1c-155">説明</span><span class="sxs-lookup"><span data-stu-id="1ac1c-155">description</span></span>|<span data-ttu-id="1ac1c-156">String</span><span class="sxs-lookup"><span data-stu-id="1ac1c-156">String</span></span>|<span data-ttu-id="1ac1c-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1ac1c-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ac1c-159">displayName</span><span class="sxs-lookup"><span data-stu-id="1ac1c-159">displayName</span></span>|<span data-ttu-id="1ac1c-160">String</span><span class="sxs-lookup"><span data-stu-id="1ac1c-160">String</span></span>|<span data-ttu-id="1ac1c-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1ac1c-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ac1c-163">version</span><span class="sxs-lookup"><span data-stu-id="1ac1c-163">version</span></span>|<span data-ttu-id="1ac1c-164">Int32</span><span class="sxs-lookup"><span data-stu-id="1ac1c-164">Int32</span></span>|<span data-ttu-id="1ac1c-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-165">Version of the device configuration.</span></span> <span data-ttu-id="1ac1c-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1ac1c-167">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1ac1c-167">renewalThresholdPercentage</span></span>|<span data-ttu-id="1ac1c-168">Int32</span><span class="sxs-lookup"><span data-stu-id="1ac1c-168">Int32</span></span>|<span data-ttu-id="1ac1c-169">証明書の更新しきい値の割合。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-169">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="1ac1c-170">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承される有効な値は1から99。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-170">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1ac1c-171">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1ac1c-171">subjectNameFormat</span></span>|[<span data-ttu-id="1ac1c-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1ac1c-172">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="1ac1c-173">証明書のサブジェクト名の形式。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-173">Certificate Subject Name Format.</span></span> <span data-ttu-id="1ac1c-174">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-174">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1ac1c-175">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-175">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="1ac1c-176">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1ac1c-176">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1ac1c-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1ac1c-177">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="1ac1c-178">証明書のサブジェクトの別名の種類。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-178">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="1ac1c-179">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-179">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1ac1c-180">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-180">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="1ac1c-181">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1ac1c-181">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1ac1c-182">Int32</span><span class="sxs-lookup"><span data-stu-id="1ac1c-182">Int32</span></span>|<span data-ttu-id="1ac1c-183">証明書の有効期間の値。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-183">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="1ac1c-184">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-184">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1ac1c-185">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1ac1c-185">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1ac1c-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1ac1c-186">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1ac1c-187">証明書の有効期間のスケール。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-187">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="1ac1c-188">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-188">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="1ac1c-189">可能な値は `days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-189">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="1ac1c-190">extendedkeyusages</span><span class="sxs-lookup"><span data-stu-id="1ac1c-190">extendedKeyUsages</span></span>|<span data-ttu-id="1ac1c-191">[extendedkeyusage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ac1c-191">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="1ac1c-192">拡張キー使用法 (EKU) の設定。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-192">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="1ac1c-193">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-193">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="1ac1c-194">[androidcertificateprofilebase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承します</span><span class="sxs-lookup"><span data-stu-id="1ac1c-194">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="1ac1c-195">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1ac1c-195">intendedPurpose</span></span>|[<span data-ttu-id="1ac1c-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="1ac1c-196">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="1ac1c-197">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-197">Not yet documented.</span></span> <span data-ttu-id="1ac1c-198">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-198">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="1ac1c-199">応答</span><span class="sxs-lookup"><span data-stu-id="1ac1c-199">Response</span></span>
<span data-ttu-id="1ac1c-200">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-200">If successful, this method returns a `201 Created` response code and a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ac1c-201">例</span><span class="sxs-lookup"><span data-stu-id="1ac1c-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ac1c-202">要求</span><span class="sxs-lookup"><span data-stu-id="1ac1c-202">Request</span></span>
<span data-ttu-id="1ac1c-203">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 726

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
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
  "intendedPurpose": "smimeEncryption"
}
```

### <a name="response"></a><span data-ttu-id="1ac1c-204">応答</span><span class="sxs-lookup"><span data-stu-id="1ac1c-204">Response</span></span>
<span data-ttu-id="1ac1c-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ac1c-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 898

{
  "@odata.type": "#microsoft.graph.androidForWorkImportedPFXCertificateProfile",
  "id": "a0bfd7bc-d7bc-a0bf-bcd7-bfa0bcd7bfa0",
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
  "intendedPurpose": "smimeEncryption"
}
```




