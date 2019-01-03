---
title: iosEduDeviceConfiguration リソースの種類
description: iOS 教育デバイスの構成
author: tfitzmac
ms.openlocfilehash: 6ec5619f28d75e97080cdea81d547bf0a1a94a2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313588"
---
# <a name="iosedudeviceconfiguration-resource-type"></a><span data-ttu-id="dfe45-103">iosEduDeviceConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dfe45-103">iosEduDeviceConfiguration resource type</span></span>

> <span data-ttu-id="dfe45-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="dfe45-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dfe45-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dfe45-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="dfe45-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dfe45-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfe45-107">iOS 教育デバイスの構成</span><span class="sxs-lookup"><span data-stu-id="dfe45-107">iOS Education device configuration</span></span>

<span data-ttu-id="dfe45-108">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-108">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="dfe45-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfe45-109">Methods</span></span>
|<span data-ttu-id="dfe45-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="dfe45-110">Method</span></span>|<span data-ttu-id="dfe45-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="dfe45-111">Return Type</span></span>|<span data-ttu-id="dfe45-112">説明</span><span class="sxs-lookup"><span data-stu-id="dfe45-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dfe45-113">リスト iosEduDeviceConfigurations</span><span class="sxs-lookup"><span data-stu-id="dfe45-113">List iosEduDeviceConfigurations</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-list.md)|<span data-ttu-id="dfe45-114">[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dfe45-114">[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) collection</span></span>|<span data-ttu-id="dfe45-115">[IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-115">List properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="dfe45-116">IosEduDeviceConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-116">Get iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-get.md)|[<span data-ttu-id="dfe45-117">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dfe45-117">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="dfe45-118">[IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dfe45-118">Read properties and relationships of the [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="dfe45-119">IosEduDeviceConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-119">Create iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-create.md)|[<span data-ttu-id="dfe45-120">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dfe45-120">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="dfe45-121">新しい[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-121">Create a new [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|
|[<span data-ttu-id="dfe45-122">IosEduDeviceConfiguration を削除します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-122">Delete iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-delete.md)|<span data-ttu-id="dfe45-123">なし</span><span class="sxs-lookup"><span data-stu-id="dfe45-123">None</span></span>|<span data-ttu-id="dfe45-124">の[iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-124">Deletes a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md).</span></span>|
|[<span data-ttu-id="dfe45-125">IosEduDeviceConfiguration を更新します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-125">Update iosEduDeviceConfiguration</span></span>](../api/intune-deviceconfig-iosedudeviceconfiguration-update.md)|[<span data-ttu-id="dfe45-126">iosEduDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dfe45-126">iosEduDeviceConfiguration</span></span>](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)|<span data-ttu-id="dfe45-127">[IosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-127">Update the properties of a [iosEduDeviceConfiguration](../resources/intune-deviceconfig-iosedudeviceconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dfe45-128">Properties</span><span class="sxs-lookup"><span data-stu-id="dfe45-128">Properties</span></span>
|<span data-ttu-id="dfe45-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dfe45-129">Property</span></span>|<span data-ttu-id="dfe45-130">種類</span><span class="sxs-lookup"><span data-stu-id="dfe45-130">Type</span></span>|<span data-ttu-id="dfe45-131">説明</span><span class="sxs-lookup"><span data-stu-id="dfe45-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfe45-132">ID</span><span class="sxs-lookup"><span data-stu-id="dfe45-132">id</span></span>|<span data-ttu-id="dfe45-133">String</span><span class="sxs-lookup"><span data-stu-id="dfe45-133">String</span></span>|<span data-ttu-id="dfe45-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dfe45-134">Key of the entity.</span></span> <span data-ttu-id="dfe45-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfe45-136">lastModifiedDateTime</span></span>|<span data-ttu-id="dfe45-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfe45-137">DateTimeOffset</span></span>|<span data-ttu-id="dfe45-138">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="dfe45-138">DateTime the object was last modified.</span></span> <span data-ttu-id="dfe45-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dfe45-140">roleScopeTagIds</span></span>|<span data-ttu-id="dfe45-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dfe45-141">String collection</span></span>|<span data-ttu-id="dfe45-142">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="dfe45-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dfe45-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dfe45-144">supportsScopeTags</span></span>|<span data-ttu-id="dfe45-145">ブール型</span><span class="sxs-lookup"><span data-stu-id="dfe45-145">Boolean</span></span>|<span data-ttu-id="dfe45-146">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dfe45-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dfe45-147">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="dfe45-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dfe45-148">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="dfe45-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dfe45-149">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="dfe45-149">This property is read-only.</span></span> <span data-ttu-id="dfe45-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfe45-151">createdDateTime</span></span>|<span data-ttu-id="dfe45-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfe45-152">DateTimeOffset</span></span>|<span data-ttu-id="dfe45-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="dfe45-153">DateTime the object was created.</span></span> <span data-ttu-id="dfe45-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-155">説明</span><span class="sxs-lookup"><span data-stu-id="dfe45-155">description</span></span>|<span data-ttu-id="dfe45-156">String</span><span class="sxs-lookup"><span data-stu-id="dfe45-156">String</span></span>|<span data-ttu-id="dfe45-157">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="dfe45-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dfe45-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-159">displayName</span><span class="sxs-lookup"><span data-stu-id="dfe45-159">displayName</span></span>|<span data-ttu-id="dfe45-160">String</span><span class="sxs-lookup"><span data-stu-id="dfe45-160">String</span></span>|<span data-ttu-id="dfe45-161">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="dfe45-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dfe45-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-163">version</span><span class="sxs-lookup"><span data-stu-id="dfe45-163">version</span></span>|<span data-ttu-id="dfe45-164">Int32</span><span class="sxs-lookup"><span data-stu-id="dfe45-164">Int32</span></span>|<span data-ttu-id="dfe45-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="dfe45-165">Version of the device configuration.</span></span> <span data-ttu-id="dfe45-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-167">teacherCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="dfe45-167">teacherCertificateSettings</span></span>|[<span data-ttu-id="dfe45-168">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="dfe45-168">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="dfe45-169">教師の証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="dfe45-169">The Trusted Root and PFX certificates for Teacher</span></span>|
|<span data-ttu-id="dfe45-170">studentCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="dfe45-170">studentCertificateSettings</span></span>|[<span data-ttu-id="dfe45-171">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="dfe45-171">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="dfe45-172">受講者用の証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="dfe45-172">The Trusted Root and PFX certificates for Student</span></span>|
|<span data-ttu-id="dfe45-173">deviceCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="dfe45-173">deviceCertificateSettings</span></span>|[<span data-ttu-id="dfe45-174">iosEduCertificateSettings</span><span class="sxs-lookup"><span data-stu-id="dfe45-174">iosEduCertificateSettings</span></span>](../resources/intune-deviceconfig-ioseducertificatesettings.md)|<span data-ttu-id="dfe45-175">デバイスの証明書が信頼されたルートと PFX</span><span class="sxs-lookup"><span data-stu-id="dfe45-175">The Trusted Root and PFX certificates for Device</span></span>|

## <a name="relationships"></a><span data-ttu-id="dfe45-176">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfe45-176">Relationships</span></span>
|<span data-ttu-id="dfe45-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dfe45-177">Relationship</span></span>|<span data-ttu-id="dfe45-178">型</span><span class="sxs-lookup"><span data-stu-id="dfe45-178">Type</span></span>|<span data-ttu-id="dfe45-179">説明</span><span class="sxs-lookup"><span data-stu-id="dfe45-179">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfe45-180">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="dfe45-180">groupAssignments</span></span>|<span data-ttu-id="dfe45-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="dfe45-181">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="dfe45-182">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="dfe45-182">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="dfe45-183">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-183">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-184">assignments</span><span class="sxs-lookup"><span data-stu-id="dfe45-184">assignments</span></span>|<span data-ttu-id="dfe45-185">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dfe45-185">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="dfe45-186">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="dfe45-186">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="dfe45-187">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-187">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-188">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="dfe45-188">deviceStatuses</span></span>|<span data-ttu-id="dfe45-189">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dfe45-189">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="dfe45-190">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="dfe45-190">Device configuration installation status by device.</span></span> <span data-ttu-id="dfe45-191">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-191">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-192">userStatuses</span><span class="sxs-lookup"><span data-stu-id="dfe45-192">userStatuses</span></span>|<span data-ttu-id="dfe45-193">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dfe45-193">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="dfe45-194">ユーザーごとのデバイス構成のインストール状態です。</span><span class="sxs-lookup"><span data-stu-id="dfe45-194">Device configuration installation status by user.</span></span> <span data-ttu-id="dfe45-195">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dfe45-195">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-196">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="dfe45-196">deviceStatusOverview</span></span>|[<span data-ttu-id="dfe45-197">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="dfe45-197">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="dfe45-198">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="dfe45-198">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-199">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="dfe45-199">userStatusOverview</span></span>|[<span data-ttu-id="dfe45-200">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="dfe45-200">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="dfe45-201">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="dfe45-201">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfe45-202">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="dfe45-202">deviceSettingStateSummaries</span></span>|<span data-ttu-id="dfe45-203">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dfe45-203">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="dfe45-204">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="dfe45-204">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dfe45-205">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dfe45-205">JSON Representation</span></span>
<span data-ttu-id="dfe45-206">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dfe45-206">Here is a JSON representation of the resource.</span></span>
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




