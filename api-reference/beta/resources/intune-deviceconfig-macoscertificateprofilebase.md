---
title: macOSCertificateProfileBase リソースの種類
description: Mac OS の証明書のプロファイルです。
author: tfitzmac
ms.openlocfilehash: fded8f604afc5d4121cc7d1865db0de2ddb4ee27
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308772"
---
# <a name="macoscertificateprofilebase-resource-type"></a><span data-ttu-id="1a658-103">macOSCertificateProfileBase リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1a658-103">macOSCertificateProfileBase resource type</span></span>

> <span data-ttu-id="1a658-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1a658-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1a658-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a658-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1a658-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1a658-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1a658-107">Mac OS の証明書のプロファイルです。</span><span class="sxs-lookup"><span data-stu-id="1a658-107">Mac OS certificate profile.</span></span>

<span data-ttu-id="1a658-108">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1a658-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a658-109">Methods</span></span>
|<span data-ttu-id="1a658-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="1a658-110">Method</span></span>|<span data-ttu-id="1a658-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1a658-111">Return Type</span></span>|<span data-ttu-id="1a658-112">説明</span><span class="sxs-lookup"><span data-stu-id="1a658-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1a658-113">リスト macOSCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="1a658-113">List macOSCertificateProfileBases</span></span>](../api/intune-deviceconfig-macoscertificateprofilebase-list.md)|<span data-ttu-id="1a658-114">[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a658-114">[macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md) collection</span></span>|<span data-ttu-id="1a658-115">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="1a658-115">List properties and relationships of the [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md) objects.</span></span>|
|[<span data-ttu-id="1a658-116">MacOSCertificateProfileBase を取得します。</span><span class="sxs-lookup"><span data-stu-id="1a658-116">Get macOSCertificateProfileBase</span></span>](../api/intune-deviceconfig-macoscertificateprofilebase-get.md)|[<span data-ttu-id="1a658-117">macOSCertificateProfileBase</span><span class="sxs-lookup"><span data-stu-id="1a658-117">macOSCertificateProfileBase</span></span>](../resources/intune-deviceconfig-macoscertificateprofilebase.md)|<span data-ttu-id="1a658-118">[MacOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a658-118">Read properties and relationships of the [macOSCertificateProfileBase](../resources/intune-deviceconfig-macoscertificateprofilebase.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1a658-119">Properties</span><span class="sxs-lookup"><span data-stu-id="1a658-119">Properties</span></span>
|<span data-ttu-id="1a658-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a658-120">Property</span></span>|<span data-ttu-id="1a658-121">種類</span><span class="sxs-lookup"><span data-stu-id="1a658-121">Type</span></span>|<span data-ttu-id="1a658-122">説明</span><span class="sxs-lookup"><span data-stu-id="1a658-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a658-123">ID</span><span class="sxs-lookup"><span data-stu-id="1a658-123">id</span></span>|<span data-ttu-id="1a658-124">String</span><span class="sxs-lookup"><span data-stu-id="1a658-124">String</span></span>|<span data-ttu-id="1a658-125">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1a658-125">Key of the entity.</span></span> <span data-ttu-id="1a658-126">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-126">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a658-127">lastModifiedDateTime</span></span>|<span data-ttu-id="1a658-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a658-128">DateTimeOffset</span></span>|<span data-ttu-id="1a658-129">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a658-129">DateTime the object was last modified.</span></span> <span data-ttu-id="1a658-130">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-130">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-131">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1a658-131">roleScopeTagIds</span></span>|<span data-ttu-id="1a658-132">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1a658-132">String collection</span></span>|<span data-ttu-id="1a658-133">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="1a658-133">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1a658-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-135">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1a658-135">supportsScopeTags</span></span>|<span data-ttu-id="1a658-136">ブール型</span><span class="sxs-lookup"><span data-stu-id="1a658-136">Boolean</span></span>|<span data-ttu-id="1a658-137">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1a658-137">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1a658-138">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="1a658-138">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1a658-139">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="1a658-139">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1a658-140">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="1a658-140">This property is read-only.</span></span> <span data-ttu-id="1a658-141">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-141">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a658-142">createdDateTime</span></span>|<span data-ttu-id="1a658-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a658-143">DateTimeOffset</span></span>|<span data-ttu-id="1a658-144">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="1a658-144">DateTime the object was created.</span></span> <span data-ttu-id="1a658-145">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-145">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-146">説明</span><span class="sxs-lookup"><span data-stu-id="1a658-146">description</span></span>|<span data-ttu-id="1a658-147">String</span><span class="sxs-lookup"><span data-stu-id="1a658-147">String</span></span>|<span data-ttu-id="1a658-148">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="1a658-148">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1a658-149">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-150">displayName</span><span class="sxs-lookup"><span data-stu-id="1a658-150">displayName</span></span>|<span data-ttu-id="1a658-151">String</span><span class="sxs-lookup"><span data-stu-id="1a658-151">String</span></span>|<span data-ttu-id="1a658-152">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="1a658-152">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1a658-153">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-154">version</span><span class="sxs-lookup"><span data-stu-id="1a658-154">version</span></span>|<span data-ttu-id="1a658-155">Int32</span><span class="sxs-lookup"><span data-stu-id="1a658-155">Int32</span></span>|<span data-ttu-id="1a658-156">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1a658-156">Version of the device configuration.</span></span> <span data-ttu-id="1a658-157">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-158">renewalThresholdPercentage</span><span class="sxs-lookup"><span data-stu-id="1a658-158">renewalThresholdPercentage</span></span>|<span data-ttu-id="1a658-159">Int32</span><span class="sxs-lookup"><span data-stu-id="1a658-159">Int32</span></span>|<span data-ttu-id="1a658-160">証明書の書き換えのしきい値の割合です。</span><span class="sxs-lookup"><span data-stu-id="1a658-160">Certificate renewal threshold percentage.</span></span>|
|<span data-ttu-id="1a658-161">subjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1a658-161">subjectNameFormat</span></span>|[<span data-ttu-id="1a658-162">appleSubjectNameFormat</span><span class="sxs-lookup"><span data-stu-id="1a658-162">appleSubjectNameFormat</span></span>](../resources/intune-deviceconfig-applesubjectnameformat.md)|<span data-ttu-id="1a658-163">証明書のサブジェクト名の形式です。</span><span class="sxs-lookup"><span data-stu-id="1a658-163">Certificate Subject Name Format.</span></span> <span data-ttu-id="1a658-164">使用可能な値: `commonName`、`commonNameAsEmail`、`custom`、`commonNameIncludingEmail`、`commonNameAsIMEI`、`commonNameAsSerialNumber`。</span><span class="sxs-lookup"><span data-stu-id="1a658-164">Possible values are: `commonName`, `commonNameAsEmail`, `custom`, `commonNameIncludingEmail`, `commonNameAsIMEI`, `commonNameAsSerialNumber`.</span></span>|
|<span data-ttu-id="1a658-165">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1a658-165">subjectAlternativeNameType</span></span>|[<span data-ttu-id="1a658-166">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="1a658-166">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="1a658-167">証明書サブジェクト代替名の種類です。</span><span class="sxs-lookup"><span data-stu-id="1a658-167">Certificate Subject Alternative Name Type.</span></span> <span data-ttu-id="1a658-168">可能な値は、`none`、`emailAddress`、`userPrincipalName`、`customAzureADAttribute`、`domainNameService` です。</span><span class="sxs-lookup"><span data-stu-id="1a658-168">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="1a658-169">certificateValidityPeriodValue</span><span class="sxs-lookup"><span data-stu-id="1a658-169">certificateValidityPeriodValue</span></span>|<span data-ttu-id="1a658-170">Int32</span><span class="sxs-lookup"><span data-stu-id="1a658-170">Int32</span></span>|<span data-ttu-id="1a658-171">証明書の有効期間の値です。</span><span class="sxs-lookup"><span data-stu-id="1a658-171">Value for the Certificate Validity Period.</span></span>|
|<span data-ttu-id="1a658-172">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1a658-172">certificateValidityPeriodScale</span></span>|[<span data-ttu-id="1a658-173">certificateValidityPeriodScale</span><span class="sxs-lookup"><span data-stu-id="1a658-173">certificateValidityPeriodScale</span></span>](../resources/intune-deviceconfig-certificatevalidityperiodscale.md)|<span data-ttu-id="1a658-174">証明書の有効期間のスケールです。</span><span class="sxs-lookup"><span data-stu-id="1a658-174">Scale for the Certificate Validity Period.</span></span> <span data-ttu-id="1a658-175">可能な値は、`days`、`months`、`years` です。</span><span class="sxs-lookup"><span data-stu-id="1a658-175">Possible values are: `days`, `months`, `years`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a658-176">関係</span><span class="sxs-lookup"><span data-stu-id="1a658-176">Relationships</span></span>
|<span data-ttu-id="1a658-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1a658-177">Relationship</span></span>|<span data-ttu-id="1a658-178">型</span><span class="sxs-lookup"><span data-stu-id="1a658-178">Type</span></span>|<span data-ttu-id="1a658-179">説明</span><span class="sxs-lookup"><span data-stu-id="1a658-179">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a658-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="1a658-180">groupAssignments</span></span>|<span data-ttu-id="1a658-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1a658-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="1a658-182">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="1a658-182">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="1a658-183">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-184">assignments</span><span class="sxs-lookup"><span data-stu-id="1a658-184">assignments</span></span>|<span data-ttu-id="1a658-185">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1a658-185">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="1a658-186">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="1a658-186">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="1a658-187">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-188">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="1a658-188">deviceStatuses</span></span>|<span data-ttu-id="1a658-189">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1a658-189">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="1a658-190">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="1a658-190">Device configuration installation status by device.</span></span> <span data-ttu-id="1a658-191">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-191">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-192">userStatuses</span><span class="sxs-lookup"><span data-stu-id="1a658-192">userStatuses</span></span>|<span data-ttu-id="1a658-193">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1a658-193">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="1a658-194">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="1a658-194">Device configuration installation status by user.</span></span> <span data-ttu-id="1a658-195">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a658-195">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-196">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1a658-196">deviceStatusOverview</span></span>|[<span data-ttu-id="1a658-197">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="1a658-197">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="1a658-198">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1a658-198">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-199">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="1a658-199">userStatusOverview</span></span>|[<span data-ttu-id="1a658-200">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="1a658-200">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="1a658-201">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1a658-201">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1a658-202">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="1a658-202">deviceSettingStateSummaries</span></span>|<span data-ttu-id="1a658-203">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1a658-203">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="1a658-204">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1a658-204">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1a658-205">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1a658-205">JSON Representation</span></span>
<span data-ttu-id="1a658-206">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1a658-206">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSCertificateProfileBase"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSCertificateProfileBase",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "renewalThresholdPercentage": 1024,
  "subjectNameFormat": "String",
  "subjectAlternativeNameType": "String",
  "certificateValidityPeriodValue": 1024,
  "certificateValidityPeriodScale": "String"
}
```




