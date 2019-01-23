---
title: AndroidForWorkScepCertificateProfile を更新します。
description: AndroidForWorkScepCertificateProfile オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2e0950227f9280c0f3c0a641b82929daf320897
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402497"
---
# <a name="update-androidforworkscepcertificateprofile"></a><span data-ttu-id="afc3a-103">AndroidForWorkScepCertificateProfile を更新します。</span><span class="sxs-lookup"><span data-stu-id="afc3a-103">Update androidForWorkScepCertificateProfile</span></span>

> <span data-ttu-id="afc3a-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="afc3a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="afc3a-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afc3a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="afc3a-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afc3a-107">[AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="afc3a-107">Update the properties of a [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afc3a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="afc3a-108">Prerequisites</span></span>
<span data-ttu-id="afc3a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="afc3a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="afc3a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="afc3a-111">Permission type</span></span>|<span data-ttu-id="afc3a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="afc3a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afc3a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="afc3a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afc3a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afc3a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afc3a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="afc3a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afc3a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afc3a-116">Not supported.</span></span>|
|<span data-ttu-id="afc3a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="afc3a-117">Application</span></span>|<span data-ttu-id="afc3a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afc3a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="afc3a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="afc3a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="afc3a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afc3a-120">Request headers</span></span>
|<span data-ttu-id="afc3a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="afc3a-121">Header</span></span>|<span data-ttu-id="afc3a-122">値</span><span class="sxs-lookup"><span data-stu-id="afc3a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afc3a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afc3a-123">Authorization</span></span>|<span data-ttu-id="afc3a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="afc3a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afc3a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="afc3a-125">Accept</span></span>|<span data-ttu-id="afc3a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afc3a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afc3a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="afc3a-127">Request body</span></span>
<span data-ttu-id="afc3a-128">要求の本文に[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="afc3a-128">In the request body, supply a JSON representation for the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object.</span></span>

<span data-ttu-id="afc3a-129">[AndroidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="afc3a-129">The following table shows the properties that are required when you create the [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md).</span></span>

|<span data-ttu-id="afc3a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afc3a-130">Property</span></span>|<span data-ttu-id="afc3a-131">型</span><span class="sxs-lookup"><span data-stu-id="afc3a-131">Type</span></span>|<span data-ttu-id="afc3a-132">説明</span><span class="sxs-lookup"><span data-stu-id="afc3a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afc3a-133">id</span><span class="sxs-lookup"><span data-stu-id="afc3a-133">id</span></span>|<span data-ttu-id="afc3a-134">String</span><span class="sxs-lookup"><span data-stu-id="afc3a-134">String</span></span>|<span data-ttu-id="afc3a-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="afc3a-135">Key of the entity.</span></span> <span data-ttu-id="afc3a-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="afc3a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afc3a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="afc3a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="afc3a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afc3a-138">DateTimeOffset</span></span>|<span data-ttu-id="afc3a-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="afc3a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="afc3a-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="afc3a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afc3a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="afc3a-141">roleScopeTagIds</span></span>|<span data-ttu-id="afc3a-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="afc3a-142">String collection</span></span>|<span data-ttu-id="afc3a-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="afc3a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="afc3a-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="afc3a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afc3a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="afc3a-145">supportsScopeTags</span></span>|<span data-ttu-id="afc3a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="afc3a-146">Boolean</span></span>|<span data-ttu-id="afc3a-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="afc3a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="afc3a-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="afc3a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="afc3a-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="afc3a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="afc3a-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-150">This property is read-only.</span></span> <span data-ttu-id="afc3a-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="afc3a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afc3a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="afc3a-152">createdDateTime</span></span>|<span data-ttu-id="afc3a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afc3a-153">DateTimeOffset</span></span>|<span data-ttu-id="afc3a-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="afc3a-154">DateTime the object was created.</span></span> <span data-ttu-id="afc3a-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="afc3a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afc3a-156">説明</span><span class="sxs-lookup"><span data-stu-id="afc3a-156">description</span></span>|<span data-ttu-id="afc3a-157">String</span><span class="sxs-lookup"><span data-stu-id="afc3a-157">String</span></span>|<span data-ttu-id="afc3a-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="afc3a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="afc3a-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="afc3a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afc3a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="afc3a-160">displayName</span></span>|<span data-ttu-id="afc3a-161">String</span><span class="sxs-lookup"><span data-stu-id="afc3a-161">String</span></span>|<span data-ttu-id="afc3a-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="afc3a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="afc3a-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="afc3a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afc3a-164">version</span><span class="sxs-lookup"><span data-stu-id="afc3a-164">version</span></span>|<span data-ttu-id="afc3a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="afc3a-165">Int32</span></span>|<span data-ttu-id="afc3a-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="afc3a-166">Version of the device configuration.</span></span> <span data-ttu-id="afc3a-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="afc3a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="afc3a-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="afc3a-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="afc3a-169">Int32</span><span class="sxs-lookup"><span data-stu-id="afc3a-169">Int32</span></span>|<span data-ttu-id="afc3a-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="afc3a-171">有効な値は[androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="afc3a-171">Valid values 1 to 99 Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="afc3a-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="afc3a-172">subjectNameFormat</span></span>|[<span data-ttu-id="afc3a-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="afc3a-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="afc3a-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="afc3a-175">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="afc3a-175">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="afc3a-176">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="afc3a-177">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="afc3a-177">certificateValidityPeriodValue</span></span>|<span data-ttu-id="afc3a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="afc3a-178">Int32</span></span>|<span data-ttu-id="afc3a-179">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-179">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="afc3a-180">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="afc3a-180">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="afc3a-181">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="afc3a-181">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="afc3a-182">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="afc3a-182">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="afc3a-183">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="afc3a-183">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="afc3a-184">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="afc3a-184">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md).</span></span> <span data-ttu-id="afc3a-185">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-185">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="afc3a-186">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="afc3a-186">extendedKeyUsages</span></span>|<span data-ttu-id="afc3a-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="afc3a-187">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="afc3a-188">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="afc3a-188">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="afc3a-189">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="afc3a-189">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="afc3a-190">[AndroidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="afc3a-190">Inherited from [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="afc3a-191">scepServerUrls</span><span class="sxs-lookup"><span data-stu-id="afc3a-191">scepServerUrls</span></span>|<span data-ttu-id="afc3a-192">String コレクション</span><span class="sxs-lookup"><span data-stu-id="afc3a-192">String collection</span></span>|<span data-ttu-id="afc3a-193">SCEP サーバー個の url</span><span class="sxs-lookup"><span data-stu-id="afc3a-193">SCEP Server Url(s)</span></span>|
|<span data-ttu-id="afc3a-194">subjectNameFormatString</span><span class="sxs-lookup"><span data-stu-id="afc3a-194">subjectNameFormatString</span></span>|<span data-ttu-id="afc3a-195">String</span><span class="sxs-lookup"><span data-stu-id="afc3a-195">String</span></span>|<span data-ttu-id="afc3a-196">SubjectNameFormat で使用するカスタム書式指定 = カスタムです。</span><span class="sxs-lookup"><span data-stu-id="afc3a-196">Custom format to use with SubjectNameFormat = Custom.</span></span> <span data-ttu-id="afc3a-197">例: CN = EmailAddress {{}}、E = EmailAddress {{}}、OU = エンタープライズ ユーザーの場合は、O = コントソ株式会社、L = Redmond、ST = ワシントン州 C = u. s.</span><span class="sxs-lookup"><span data-stu-id="afc3a-197">Example: CN={{EmailAddress}},E={{EmailAddress}},OU=Enterprise Users,O=Contoso Corporation,L=Redmond,ST=WA,C=US</span></span>|
|<span data-ttu-id="afc3a-198">keyUsage</span><span class="sxs-lookup"><span data-stu-id="afc3a-198">keyUsage</span></span>|[<span data-ttu-id="afc3a-199">keyUsages</span><span class="sxs-lookup"><span data-stu-id="afc3a-199">keyUsages</span></span>](../resources/intune-deviceconfig-keyusages.md)|<span data-ttu-id="afc3a-200">SCEP のキー使用法です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-200">SCEP Key Usage.</span></span> <span data-ttu-id="afc3a-201">使用可能な値は、`keyEncipherment`、`digitalSignature` です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-201">Possible values are: `keyEncipherment`, `digitalSignature`.</span></span>|
|<span data-ttu-id="afc3a-202">キー長</span><span class="sxs-lookup"><span data-stu-id="afc3a-202">keySize</span></span>|[<span data-ttu-id="afc3a-203">キー長</span><span class="sxs-lookup"><span data-stu-id="afc3a-203">keySize</span></span>](../resources/intune-deviceconfig-keysize.md)|<span data-ttu-id="afc3a-204">SCEP のキー サイズ。</span><span class="sxs-lookup"><span data-stu-id="afc3a-204">SCEP Key Size.</span></span> <span data-ttu-id="afc3a-205">使用可能な値は、`size1024`、`size2048` です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-205">Possible values are: `size1024`, `size2048`.</span></span>|
|<span data-ttu-id="afc3a-206">hashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="afc3a-206">hashAlgorithm</span></span>|[<span data-ttu-id="afc3a-207">hashAlgorithms</span><span class="sxs-lookup"><span data-stu-id="afc3a-207">hashAlgorithms</span></span>](../resources/intune-deviceconfig-hashalgorithms.md)|<span data-ttu-id="afc3a-208">SCEP ハッシュ アルゴリズム。</span><span class="sxs-lookup"><span data-stu-id="afc3a-208">SCEP Hash Algorithm.</span></span> <span data-ttu-id="afc3a-209">使用可能な値は、`sha1`、`sha2` です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-209">Possible values are: `sha1`, `sha2`.</span></span>|
|<span data-ttu-id="afc3a-210">subjectAlternativeNameFormatString</span><span class="sxs-lookup"><span data-stu-id="afc3a-210">subjectAlternativeNameFormatString</span></span>|<span data-ttu-id="afc3a-211">String</span><span class="sxs-lookup"><span data-stu-id="afc3a-211">String</span></span>|<span data-ttu-id="afc3a-212">AAD の属性を定義するカスタム文字列。</span><span class="sxs-lookup"><span data-stu-id="afc3a-212">Custom String that defines the AAD Attribute.</span></span>|
|<span data-ttu-id="afc3a-213">certificateStore</span><span class="sxs-lookup"><span data-stu-id="afc3a-213">certificateStore</span></span>|[<span data-ttu-id="afc3a-214">certificateStore</span><span class="sxs-lookup"><span data-stu-id="afc3a-214">certificateStore</span></span>](../resources/intune-deviceconfig-certificatestore.md)|<span data-ttu-id="afc3a-215">ターゲット ストアの証明書です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-215">Target store certificate.</span></span> <span data-ttu-id="afc3a-216">使用可能な値は、`user`、`machine` です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-216">Possible values are: `user`, `machine`.</span></span>|
|<span data-ttu-id="afc3a-217">customSubjectAlternativeNames</span><span class="sxs-lookup"><span data-stu-id="afc3a-217">customSubjectAlternativeNames</span></span>|<span data-ttu-id="afc3a-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="afc3a-218">[customSubjectAlternativeName](../resources/intune-deviceconfig-customsubjectalternativename.md) collection</span></span>|<span data-ttu-id="afc3a-219">Alterantive 名の設定をカスタムの件名です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-219">Custom Subject Alterantive Name Settings.</span></span> <span data-ttu-id="afc3a-220">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="afc3a-220">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="afc3a-221">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="afc3a-221">subjectAlternativeNameType</span></span>|[<span data-ttu-id="afc3a-222">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="afc3a-222">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="afc3a-223">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-223">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="afc3a-224">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-224">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|



## <a name="response"></a><span data-ttu-id="afc3a-225">応答</span><span class="sxs-lookup"><span data-stu-id="afc3a-225">Response</span></span>
<span data-ttu-id="afc3a-226">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="afc3a-226">If successful, this method returns a `200 OK` response code and an updated [androidForWorkScepCertificateProfile](../resources/intune-deviceconfig-androidforworkscepcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afc3a-227">例</span><span class="sxs-lookup"><span data-stu-id="afc3a-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="afc3a-228">要求</span><span class="sxs-lookup"><span data-stu-id="afc3a-228">Request</span></span>
<span data-ttu-id="afc3a-229">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="afc3a-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1205

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "renewalThresholdPercentage": 10,
  "subjectNameFormat": "commonNameIncludingEmail",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```

### <a name="response"></a><span data-ttu-id="afc3a-230">応答</span><span class="sxs-lookup"><span data-stu-id="afc3a-230">Response</span></span>
<span data-ttu-id="afc3a-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="afc3a-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1377

{
  "@odata.type": "#microsoft.graph.androidForWorkScepCertificateProfile",
  "id": "09e532af-32af-09e5-af32-e509af32e509",
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
  "subjectAlternativeNameFormatString": "Subject Alternative Name Format String value",
  "certificateStore": "machine",
  "customSubjectAlternativeNames": [
    {
      "@odata.type": "microsoft.graph.customSubjectAlternativeName",
      "sanType": "emailAddress",
      "name": "Name value"
    }
  ],
  "subjectAlternativeNameType": "emailAddress"
}
```




