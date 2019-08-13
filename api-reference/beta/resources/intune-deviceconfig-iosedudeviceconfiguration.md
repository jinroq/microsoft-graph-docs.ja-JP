---
title: iosEduDeviceConfiguration リソースの種類
description: iOS エデュケーションデバイスの構成
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 23c1d8a9e6f414af9dc448099fb46c3f72522d53
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36357069"
---
# <a name="iosedudeviceconfiguration-resource-type"></a><span data-ttu-id="0606f-103">iosEduDeviceConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0606f-103">iosEduDeviceConfiguration resource type</span></span>

> <span data-ttu-id="0606f-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0606f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0606f-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0606f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0606f-106">iOS エデュケーションデバイスの構成</span><span class="sxs-lookup"><span data-stu-id="0606f-106">iOS Education device configuration</span></span>


<span data-ttu-id="0606f-107">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="0606f-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="0606f-108">Methods</span></span>
|<span data-ttu-id="0606f-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="0606f-109">Method</span></span>|<span data-ttu-id="0606f-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0606f-110">Return Type</span></span>|<span data-ttu-id="0606f-111">説明</span><span class="sxs-lookup"><span data-stu-id="0606f-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0606f-112">Iosedudeviceconfigurduを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="0606f-112">List iosEduDeviceConfigurations</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-list.md)|<span data-ttu-id="0606f-113">[Iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0606f-113">[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) collection</span></span>|<span data-ttu-id="0606f-114">[Iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0606f-114">List properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="0606f-115">IosEduDeviceConfiguration 取得する</span><span class="sxs-lookup"><span data-stu-id="0606f-115">Get iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-get.md)|[<span data-ttu-id="0606f-116">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0606f-116">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="0606f-117">[Iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0606f-117">Read properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0606f-118">IosEduDeviceConfiguration 作成する</span><span class="sxs-lookup"><span data-stu-id="0606f-118">Create iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-create.md)|[<span data-ttu-id="0606f-119">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0606f-119">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="0606f-120">新しい[Iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0606f-120">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="0606f-121">IosEduDeviceConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="0606f-121">Delete iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-delete.md)|<span data-ttu-id="0606f-122">None</span><span class="sxs-lookup"><span data-stu-id="0606f-122">None</span></span>|<span data-ttu-id="0606f-123">[Iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)削除します。</span><span class="sxs-lookup"><span data-stu-id="0606f-123">Deletes a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>|
|[<span data-ttu-id="0606f-124">IosEduDeviceConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="0606f-124">Update iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-update.md)|[<span data-ttu-id="0606f-125">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0606f-125">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="0606f-126">[Iosedudeviceconfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0606f-126">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0606f-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0606f-127">Properties</span></span>
|<span data-ttu-id="0606f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0606f-128">Property</span></span>|<span data-ttu-id="0606f-129">型</span><span class="sxs-lookup"><span data-stu-id="0606f-129">Type</span></span>|<span data-ttu-id="0606f-130">説明</span><span class="sxs-lookup"><span data-stu-id="0606f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0606f-131">id</span><span class="sxs-lookup"><span data-stu-id="0606f-131">id</span></span>|<span data-ttu-id="0606f-132">文字列</span><span class="sxs-lookup"><span data-stu-id="0606f-132">String</span></span>|<span data-ttu-id="0606f-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0606f-133">Key of the entity.</span></span> <span data-ttu-id="0606f-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0606f-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0606f-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0606f-136">DateTimeOffset</span></span>|<span data-ttu-id="0606f-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="0606f-137">DateTime the object was last modified.</span></span> <span data-ttu-id="0606f-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0606f-139">roleScopeTagIds</span></span>|<span data-ttu-id="0606f-140">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0606f-140">String collection</span></span>|<span data-ttu-id="0606f-141">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0606f-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0606f-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-143">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0606f-143">supportsScopeTags</span></span>|<span data-ttu-id="0606f-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="0606f-144">Boolean</span></span>|<span data-ttu-id="0606f-145">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0606f-145">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0606f-146">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="0606f-146">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0606f-147">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="0606f-147">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0606f-148">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="0606f-148">This property is read-only.</span></span> <span data-ttu-id="0606f-149">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-150">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0606f-150">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="0606f-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="0606f-151">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="0606f-152">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="0606f-152">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="0606f-153">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-154">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0606f-154">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="0606f-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="0606f-155">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="0606f-156">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="0606f-156">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="0606f-157">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-158">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="0606f-158">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="0606f-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="0606f-159">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="0606f-160">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="0606f-160">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="0606f-161">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-162">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0606f-162">createdDateTime</span></span>|<span data-ttu-id="0606f-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0606f-163">DateTimeOffset</span></span>|<span data-ttu-id="0606f-164">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="0606f-164">DateTime the object was created.</span></span> <span data-ttu-id="0606f-165">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-165">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-166">description</span><span class="sxs-lookup"><span data-stu-id="0606f-166">description</span></span>|<span data-ttu-id="0606f-167">String</span><span class="sxs-lookup"><span data-stu-id="0606f-167">String</span></span>|<span data-ttu-id="0606f-168">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="0606f-168">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0606f-169">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-169">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-170">displayName</span><span class="sxs-lookup"><span data-stu-id="0606f-170">displayName</span></span>|<span data-ttu-id="0606f-171">String</span><span class="sxs-lookup"><span data-stu-id="0606f-171">String</span></span>|<span data-ttu-id="0606f-172">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="0606f-172">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0606f-173">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-173">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-174">version</span><span class="sxs-lookup"><span data-stu-id="0606f-174">version</span></span>|<span data-ttu-id="0606f-175">Int32</span><span class="sxs-lookup"><span data-stu-id="0606f-175">Int32</span></span>|<span data-ttu-id="0606f-176">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="0606f-176">Version of the device configuration.</span></span> <span data-ttu-id="0606f-177">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-177">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-178">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="0606f-178">teacherCertificateSettings</span></span>|[<span data-ttu-id="0606f-179">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="0606f-179">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="0606f-180">教師の信頼されたルートと PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="0606f-180">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="0606f-181">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="0606f-181">studentCertificateSettings</span></span>|[<span data-ttu-id="0606f-182">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="0606f-182">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="0606f-183">学生の信頼できるルート証明書と PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="0606f-183">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="0606f-184">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="0606f-184">deviceCertificateSettings</span></span>|[<span data-ttu-id="0606f-185">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="0606f-185">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="0606f-186">デバイスの信頼されたルートと PFX 証明書</span><span class="sxs-lookup"><span data-stu-id="0606f-186">The Trusted Root and PFX certificates for Device</span></span>|

## <a name="relationships"></a><span data-ttu-id="0606f-187">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0606f-187">Relationships</span></span>
|<span data-ttu-id="0606f-188">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0606f-188">Relationship</span></span>|<span data-ttu-id="0606f-189">型</span><span class="sxs-lookup"><span data-stu-id="0606f-189">Type</span></span>|<span data-ttu-id="0606f-190">説明</span><span class="sxs-lookup"><span data-stu-id="0606f-190">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0606f-191">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="0606f-191">groupAssignments</span></span>|<span data-ttu-id="0606f-192">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0606f-192">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="0606f-193">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="0606f-193">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="0606f-194">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-194">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-195">assignments</span><span class="sxs-lookup"><span data-stu-id="0606f-195">assignments</span></span>|<span data-ttu-id="0606f-196">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0606f-196">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="0606f-197">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="0606f-197">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="0606f-198">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-198">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-199">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="0606f-199">deviceStatuses</span></span>|<span data-ttu-id="0606f-200">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0606f-200">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="0606f-201">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="0606f-201">Device configuration installation status by device.</span></span> <span data-ttu-id="0606f-202">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-202">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-203">userStatuses</span><span class="sxs-lookup"><span data-stu-id="0606f-203">userStatuses</span></span>|<span data-ttu-id="0606f-204">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0606f-204">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="0606f-205">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="0606f-205">Device configuration installation status by user.</span></span> <span data-ttu-id="0606f-206">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0606f-206">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-207">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0606f-207">deviceStatusOverview</span></span>|[<span data-ttu-id="0606f-208">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="0606f-208">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="0606f-209">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="0606f-209">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-210">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="0606f-210">userStatusOverview</span></span>|[<span data-ttu-id="0606f-211">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="0606f-211">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="0606f-212">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="0606f-212">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0606f-213">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="0606f-213">deviceSettingStateSummaries</span></span>|<span data-ttu-id="0606f-214">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0606f-214">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="0606f-215">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="0606f-215">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0606f-216">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0606f-216">JSON Representation</span></span>
<span data-ttu-id="0606f-217">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0606f-217">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosEduDeviceConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosEduDeviceConfiguration",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "String"
    ],
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "String",
    "maxOSVersion": "String",
    "name": "String",
    "ruleType": "String"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "String",
    "name": "String",
    "ruleType": "String"
  },
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "displayName": "String",
  "version": 1024,
  "teacherCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  },
  "studentCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  },
  "deviceCertificateSettings": {
    "@odata.type": "microsoft.graph.iosEduCertificateSettings",
    "trustedRootCertificate": "binary",
    "certFileName": "String",
    "certificationAuthority": "String",
    "certificationAuthorityName": "String",
    "certificateTemplateName": "String",
    "renewalThresholdPercentage": 1024,
    "certificateValidityPeriodValue": 1024,
    "certificateValidityPeriodScale": "String"
  }
}
```



