---
title: AndroidForWorkImportedPFXCertificateProfile を作成します。
description: 新しい androidForWorkImportedPFXCertificateProfile オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bb85e846645b5187e4f6feb8af78e2c624821a70
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414516"
---
# <a name="create-androidforworkimportedpfxcertificateprofile"></a><span data-ttu-id="04e59-103">AndroidForWorkImportedPFXCertificateProfile を作成します。</span><span class="sxs-lookup"><span data-stu-id="04e59-103">Create androidForWorkImportedPFXCertificateProfile</span></span>

> <span data-ttu-id="04e59-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="04e59-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="04e59-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e59-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="04e59-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="04e59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04e59-107">新しい[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="04e59-107">Create a new [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04e59-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="04e59-108">Prerequisites</span></span>
<span data-ttu-id="04e59-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="04e59-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04e59-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="04e59-111">Permission type</span></span>|<span data-ttu-id="04e59-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="04e59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e59-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="04e59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="04e59-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e59-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04e59-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="04e59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e59-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e59-116">Not supported.</span></span>|
|<span data-ttu-id="04e59-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="04e59-117">Application</span></span>|<span data-ttu-id="04e59-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="04e59-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e59-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="04e59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="04e59-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04e59-120">Request headers</span></span>
|<span data-ttu-id="04e59-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="04e59-121">Header</span></span>|<span data-ttu-id="04e59-122">値</span><span class="sxs-lookup"><span data-stu-id="04e59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04e59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e59-123">Authorization</span></span>|<span data-ttu-id="04e59-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="04e59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04e59-125">Accept</span><span class="sxs-lookup"><span data-stu-id="04e59-125">Accept</span></span>|<span data-ttu-id="04e59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04e59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e59-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="04e59-127">Request body</span></span>
<span data-ttu-id="04e59-128">要求の本文に androidForWorkImportedPFXCertificateProfile オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="04e59-128">In the request body, supply a JSON representation for the androidForWorkImportedPFXCertificateProfile object.</span></span>

<span data-ttu-id="04e59-129">次の表は、androidForWorkImportedPFXCertificateProfile を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="04e59-129">The following table shows the properties that are required when you create the androidForWorkImportedPFXCertificateProfile.</span></span>

|<span data-ttu-id="04e59-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="04e59-130">Property</span></span>|<span data-ttu-id="04e59-131">型</span><span class="sxs-lookup"><span data-stu-id="04e59-131">Type</span></span>|<span data-ttu-id="04e59-132">説明</span><span class="sxs-lookup"><span data-stu-id="04e59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e59-133">id</span><span class="sxs-lookup"><span data-stu-id="04e59-133">id</span></span>|<span data-ttu-id="04e59-134">String</span><span class="sxs-lookup"><span data-stu-id="04e59-134">String</span></span>|<span data-ttu-id="04e59-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="04e59-135">Key of the entity.</span></span> <span data-ttu-id="04e59-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e59-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e59-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04e59-137">lastModifiedDateTime</span></span>|<span data-ttu-id="04e59-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e59-138">DateTimeOffset</span></span>|<span data-ttu-id="04e59-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="04e59-139">DateTime the object was last modified.</span></span> <span data-ttu-id="04e59-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e59-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e59-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04e59-141">roleScopeTagIds</span></span>|<span data-ttu-id="04e59-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="04e59-142">String collection</span></span>|<span data-ttu-id="04e59-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="04e59-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="04e59-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e59-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e59-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="04e59-145">supportsScopeTags</span></span>|<span data-ttu-id="04e59-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="04e59-146">Boolean</span></span>|<span data-ttu-id="04e59-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="04e59-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="04e59-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="04e59-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="04e59-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="04e59-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="04e59-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="04e59-150">This property is read-only.</span></span> <span data-ttu-id="04e59-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e59-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e59-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04e59-152">createdDateTime</span></span>|<span data-ttu-id="04e59-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e59-153">DateTimeOffset</span></span>|<span data-ttu-id="04e59-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="04e59-154">DateTime the object was created.</span></span> <span data-ttu-id="04e59-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e59-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e59-156">説明</span><span class="sxs-lookup"><span data-stu-id="04e59-156">description</span></span>|<span data-ttu-id="04e59-157">String</span><span class="sxs-lookup"><span data-stu-id="04e59-157">String</span></span>|<span data-ttu-id="04e59-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="04e59-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="04e59-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e59-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e59-160">displayName</span><span class="sxs-lookup"><span data-stu-id="04e59-160">displayName</span></span>|<span data-ttu-id="04e59-161">String</span><span class="sxs-lookup"><span data-stu-id="04e59-161">String</span></span>|<span data-ttu-id="04e59-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="04e59-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="04e59-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e59-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e59-164">version</span><span class="sxs-lookup"><span data-stu-id="04e59-164">version</span></span>|<span data-ttu-id="04e59-165">Int32</span><span class="sxs-lookup"><span data-stu-id="04e59-165">Int32</span></span>|<span data-ttu-id="04e59-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="04e59-166">Version of the device configuration.</span></span> <span data-ttu-id="04e59-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="04e59-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04e59-168">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="04e59-168">renewalThresholdPercentage</span></span>|<span data-ttu-id="04e59-169">Int32</span><span class="sxs-lookup"><span data-stu-id="04e59-169">Int32</span></span>|<span data-ttu-id="04e59-170">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="04e59-170">Certificate renewal threshold percentage.</span></span> <span data-ttu-id="04e59-171">有効な値は[androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)からの 1 から 99 までの継承</span><span class="sxs-lookup"><span data-stu-id="04e59-171">Valid values 1 to 99 Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="04e59-172">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="04e59-172">subjectNameFormat</span></span>|[<span data-ttu-id="04e59-173">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="04e59-173">subjectNameFormat</span></span>](../resources/intune-deviceconfig-subjectnameformat.md)|<span data-ttu-id="04e59-174">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="04e59-174">Certificate Subject Name Format.</span></span> <span data-ttu-id="04e59-175">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="04e59-175">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="04e59-176">可能な値は、`commonName`、`commonNameIncludingEmail`、`commonNameAsEmail`、`custom`、`commonNameAsIMEI`、`commonNameAsSerialNumber`、`commonNameAsAadDeviceId`、`commonNameAsIntuneDeviceId`、`commonNameAsDurableDeviceId` です。</span><span class="sxs-lookup"><span data-stu-id="04e59-176">Possible values are: `commonName`, `commonNameIncludingEmail`, `commonNameAsEmail`, `custom`, `commonNameAsIMEI`, `commonNameAsSerialNumber`, `commonNameAsAadDeviceId`, `commonNameAsIntuneDeviceId`, `commonNameAsDurableDeviceId`.</span></span>|
|<span data-ttu-id="04e59-177">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="04e59-177">subjectAlternativeNameType</span></span>|[<span data-ttu-id="04e59-178">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="04e59-178">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="04e59-179">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="04e59-179">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="04e59-180">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="04e59-180">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="04e59-181">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="04e59-181">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="04e59-182">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="04e59-182">certificateValidityPeriodValue</span></span>|<span data-ttu-id="04e59-183">Int32</span><span class="sxs-lookup"><span data-stu-id="04e59-183">Int32</span></span>|<span data-ttu-id="04e59-184">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="04e59-184">Value for the Certificate Validity Period.</span></span> <span data-ttu-id="04e59-185">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="04e59-185">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="04e59-186">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="04e59-186">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="04e59-187">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="04e59-187">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="04e59-188">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="04e59-188">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="04e59-189">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="04e59-189">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md).</span></span> <span data-ttu-id="04e59-190">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="04e59-190">Possible values are: `days`, `months`, `years`.</span></span>|
|<span data-ttu-id="04e59-191">extendedKeyUsages</span><span class="sxs-lookup"><span data-stu-id="04e59-191">extendedKeyUsages</span></span>|<span data-ttu-id="04e59-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="04e59-192">[extendedKeyUsage](../resources/intune-deviceconfig-extendedkeyusage.md) collection</span></span>|<span data-ttu-id="04e59-193">拡張キー使用法 (EKU) 設定します。</span><span class="sxs-lookup"><span data-stu-id="04e59-193">Extended Key Usage (EKU) settings.</span></span> <span data-ttu-id="04e59-194">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="04e59-194">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="04e59-195">[AndroidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="04e59-195">Inherited from [androidCertificateProfileBase](../resources/intune-deviceconfig-androidcertificateprofilebase.md)</span></span>|
|<span data-ttu-id="04e59-196">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="04e59-196">intendedPurpose</span></span>|[<span data-ttu-id="04e59-197">intendedPurpose</span><span class="sxs-lookup"><span data-stu-id="04e59-197">intendedPurpose</span></span>](../resources/intune-deviceconfig-intendedpurpose.md)|<span data-ttu-id="04e59-198">まだ記載されていません。</span><span class="sxs-lookup"><span data-stu-id="04e59-198">Not yet documented.</span></span> <span data-ttu-id="04e59-199">可能な値は、`unassigned`、`smimeEncryption`、`smimeSigning`、`vpn`、`wifi` です。</span><span class="sxs-lookup"><span data-stu-id="04e59-199">Possible values are: `unassigned`, `smimeEncryption`, `smimeSigning`, `vpn`, `wifi`.</span></span>|



## <a name="response"></a><span data-ttu-id="04e59-200">応答</span><span class="sxs-lookup"><span data-stu-id="04e59-200">Response</span></span>
<span data-ttu-id="04e59-201">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="04e59-201">If successful, this method returns a `201 Created` response code and a [androidForWorkImportedPFXCertificateProfile](../resources/intune-deviceconfig-androidforworkimportedpfxcertificateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e59-202">例</span><span class="sxs-lookup"><span data-stu-id="04e59-202">Example</span></span>

### <a name="request"></a><span data-ttu-id="04e59-203">要求</span><span class="sxs-lookup"><span data-stu-id="04e59-203">Request</span></span>
<span data-ttu-id="04e59-204">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="04e59-204">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04e59-205">応答</span><span class="sxs-lookup"><span data-stu-id="04e59-205">Response</span></span>
<span data-ttu-id="04e59-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="04e59-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




