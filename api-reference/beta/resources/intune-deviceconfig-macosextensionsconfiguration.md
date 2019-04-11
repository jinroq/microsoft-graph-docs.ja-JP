---
title: macOSExtensionsConfiguration リソースの種類
description: MacOS extensions 構成プロファイル。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a8c4cd08f905189080a3ef56faa5a23f4f107853
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31809272"
---
# <a name="macosextensionsconfiguration-resource-type"></a><span data-ttu-id="75b24-103">macOSExtensionsConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="75b24-103">macOSExtensionsConfiguration resource type</span></span>

> <span data-ttu-id="75b24-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="75b24-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="75b24-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="75b24-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75b24-106">MacOS extensions 構成プロファイル。</span><span class="sxs-lookup"><span data-stu-id="75b24-106">MacOS extensions configuration profile.</span></span>


<span data-ttu-id="75b24-107">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-107">Inherits from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>

## <a name="methods"></a><span data-ttu-id="75b24-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="75b24-108">Methods</span></span>
|<span data-ttu-id="75b24-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="75b24-109">Method</span></span>|<span data-ttu-id="75b24-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="75b24-110">Return Type</span></span>|<span data-ttu-id="75b24-111">説明</span><span class="sxs-lookup"><span data-stu-id="75b24-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75b24-112">リスト macOSExtensionsConfigurations</span><span class="sxs-lookup"><span data-stu-id="75b24-112">List macOSExtensionsConfigurations</span></span>](../api/intune-deviceconfig-macosextensionsconfiguration-list.md)|<span data-ttu-id="75b24-113">[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-113">[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) collection</span></span>|<span data-ttu-id="75b24-114">[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="75b24-114">List properties and relationships of the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="75b24-115">macOSExtensionsConfiguration を取得する</span><span class="sxs-lookup"><span data-stu-id="75b24-115">Get macOSExtensionsConfiguration</span></span>](../api/intune-deviceconfig-macosextensionsconfiguration-get.md)|[<span data-ttu-id="75b24-116">macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="75b24-116">macOSExtensionsConfiguration</span></span>](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|<span data-ttu-id="75b24-117">[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="75b24-117">Read properties and relationships of the [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="75b24-118">macOSExtensionsConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="75b24-118">Create macOSExtensionsConfiguration</span></span>](../api/intune-deviceconfig-macosextensionsconfiguration-create.md)|[<span data-ttu-id="75b24-119">macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="75b24-119">macOSExtensionsConfiguration</span></span>](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|<span data-ttu-id="75b24-120">新しい[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="75b24-120">Create a new [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>|
|[<span data-ttu-id="75b24-121">macOSExtensionsConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="75b24-121">Delete macOSExtensionsConfiguration</span></span>](../api/intune-deviceconfig-macosextensionsconfiguration-delete.md)|<span data-ttu-id="75b24-122">なし</span><span class="sxs-lookup"><span data-stu-id="75b24-122">None</span></span>|<span data-ttu-id="75b24-123">[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="75b24-123">Deletes a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md).</span></span>|
|[<span data-ttu-id="75b24-124">macOSExtensionsConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="75b24-124">Update macOSExtensionsConfiguration</span></span>](../api/intune-deviceconfig-macosextensionsconfiguration-update.md)|[<span data-ttu-id="75b24-125">macOSExtensionsConfiguration</span><span class="sxs-lookup"><span data-stu-id="75b24-125">macOSExtensionsConfiguration</span></span>](../resources/intune-deviceconfig-macosextensionsconfiguration.md)|<span data-ttu-id="75b24-126">[macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="75b24-126">Update the properties of a [macOSExtensionsConfiguration](../resources/intune-deviceconfig-macosextensionsconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75b24-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75b24-127">Properties</span></span>
|<span data-ttu-id="75b24-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="75b24-128">Property</span></span>|<span data-ttu-id="75b24-129">型</span><span class="sxs-lookup"><span data-stu-id="75b24-129">Type</span></span>|<span data-ttu-id="75b24-130">説明</span><span class="sxs-lookup"><span data-stu-id="75b24-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b24-131">id</span><span class="sxs-lookup"><span data-stu-id="75b24-131">id</span></span>|<span data-ttu-id="75b24-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="75b24-132">String</span></span>|<span data-ttu-id="75b24-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="75b24-133">Key of the entity.</span></span> <span data-ttu-id="75b24-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="75b24-135">lastModifiedDateTime</span></span>|<span data-ttu-id="75b24-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b24-136">DateTimeOffset</span></span>|<span data-ttu-id="75b24-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="75b24-137">DateTime the object was last modified.</span></span> <span data-ttu-id="75b24-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="75b24-139">roleScopeTagIds</span></span>|<span data-ttu-id="75b24-140">String コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-140">String collection</span></span>|<span data-ttu-id="75b24-141">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="75b24-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="75b24-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-143">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="75b24-143">supportsScopeTags</span></span>|<span data-ttu-id="75b24-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="75b24-144">Boolean</span></span>|<span data-ttu-id="75b24-145">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="75b24-145">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="75b24-146">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="75b24-146">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="75b24-147">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="75b24-147">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="75b24-148">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="75b24-148">This property is read-only.</span></span> <span data-ttu-id="75b24-149">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-149">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="75b24-150">createdDateTime</span></span>|<span data-ttu-id="75b24-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="75b24-151">DateTimeOffset</span></span>|<span data-ttu-id="75b24-152">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="75b24-152">DateTime the object was created.</span></span> <span data-ttu-id="75b24-153">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-153">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-154">説明</span><span class="sxs-lookup"><span data-stu-id="75b24-154">description</span></span>|<span data-ttu-id="75b24-155">String</span><span class="sxs-lookup"><span data-stu-id="75b24-155">String</span></span>|<span data-ttu-id="75b24-156">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="75b24-156">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="75b24-157">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-157">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-158">displayName</span><span class="sxs-lookup"><span data-stu-id="75b24-158">displayName</span></span>|<span data-ttu-id="75b24-159">String</span><span class="sxs-lookup"><span data-stu-id="75b24-159">String</span></span>|<span data-ttu-id="75b24-160">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="75b24-160">Admin provided name of the device configuration.</span></span> <span data-ttu-id="75b24-161">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-161">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-162">version</span><span class="sxs-lookup"><span data-stu-id="75b24-162">version</span></span>|<span data-ttu-id="75b24-163">Int32</span><span class="sxs-lookup"><span data-stu-id="75b24-163">Int32</span></span>|<span data-ttu-id="75b24-164">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="75b24-164">Version of the device configuration.</span></span> <span data-ttu-id="75b24-165">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-165">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-166">kernelExtensionOverridesAllowed</span><span class="sxs-lookup"><span data-stu-id="75b24-166">kernelExtensionOverridesAllowed</span></span>|<span data-ttu-id="75b24-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="75b24-167">Boolean</span></span>|<span data-ttu-id="75b24-168">true に設定すると、ユーザーは、構成プロファイルで明示的に許可されていない追加のカーネル拡張機能を承認できます。</span><span class="sxs-lookup"><span data-stu-id="75b24-168">If set to true, users can approve additional kernel extensions not explicitly allowed by configurations profiles.</span></span>|
|<span data-ttu-id="75b24-169">カーネル識別子</span><span class="sxs-lookup"><span data-stu-id="75b24-169">kernelExtensionAllowedTeamIdentifiers</span></span>|<span data-ttu-id="75b24-170">String コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-170">String collection</span></span>|<span data-ttu-id="75b24-171">このリストのチーム識別子によって有効になっているすべてのカーネル拡張機能を読み込むことができます。</span><span class="sxs-lookup"><span data-stu-id="75b24-171">All kernel extensions validly signed by the team identifiers in this list will be allowed to load.</span></span>|
|<span data-ttu-id="75b24-172">kernelExtensionsAllowed</span><span class="sxs-lookup"><span data-stu-id="75b24-172">kernelExtensionsAllowed</span></span>|<span data-ttu-id="75b24-173">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-173">[macOSKernelExtension](../resources/intune-deviceconfig-macoskernelextension.md) collection</span></span>|<span data-ttu-id="75b24-174">読み込むことができるカーネル拡張機能の一覧。</span><span class="sxs-lookup"><span data-stu-id="75b24-174">A list of kernel extensions that will be allowed to load.</span></span> <span data-ttu-id="75b24-175">.</span><span class="sxs-lookup"><span data-stu-id="75b24-175"></span></span> <span data-ttu-id="75b24-176">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="75b24-176">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75b24-177">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75b24-177">Relationships</span></span>
|<span data-ttu-id="75b24-178">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="75b24-178">Relationship</span></span>|<span data-ttu-id="75b24-179">型</span><span class="sxs-lookup"><span data-stu-id="75b24-179">Type</span></span>|<span data-ttu-id="75b24-180">説明</span><span class="sxs-lookup"><span data-stu-id="75b24-180">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75b24-181">groupAssignments</span><span class="sxs-lookup"><span data-stu-id="75b24-181">groupAssignments</span></span>|<span data-ttu-id="75b24-182">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-182">[deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) collection</span></span>|<span data-ttu-id="75b24-183">デバイスの構成プロファイルのグループ割り当てのリストです。</span><span class="sxs-lookup"><span data-stu-id="75b24-183">The list of group assignments for the device configuration profile.</span></span> <span data-ttu-id="75b24-184">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-184">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-185">assignments</span><span class="sxs-lookup"><span data-stu-id="75b24-185">assignments</span></span>|<span data-ttu-id="75b24-186">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-186">[deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) collection</span></span>|<span data-ttu-id="75b24-187">デバイスの構成プロファイルの割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="75b24-187">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="75b24-188">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-188">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-189">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="75b24-189">deviceStatuses</span></span>|<span data-ttu-id="75b24-190">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-190">[deviceConfigurationDeviceStatus](../resources/intune-deviceconfig-deviceconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="75b24-191">デバイスごとのデバイス構成のインストール状況。</span><span class="sxs-lookup"><span data-stu-id="75b24-191">Device configuration installation status by device.</span></span> <span data-ttu-id="75b24-192">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-192">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-193">userStatuses</span><span class="sxs-lookup"><span data-stu-id="75b24-193">userStatuses</span></span>|<span data-ttu-id="75b24-194">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-194">[deviceConfigurationUserStatus](../resources/intune-deviceconfig-deviceconfigurationuserstatus.md) collection</span></span>|<span data-ttu-id="75b24-195">ユーザーごとのデバイス構成のインストール状態。</span><span class="sxs-lookup"><span data-stu-id="75b24-195">Device configuration installation status by user.</span></span> <span data-ttu-id="75b24-196">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="75b24-196">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-197">deviceStatusOverview</span><span class="sxs-lookup"><span data-stu-id="75b24-197">deviceStatusOverview</span></span>|[<span data-ttu-id="75b24-198">deviceConfigurationDeviceOverview</span><span class="sxs-lookup"><span data-stu-id="75b24-198">deviceConfigurationDeviceOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationdeviceoverview.md)|<span data-ttu-id="75b24-199">デバイス構成のデバイス状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="75b24-199">Device Configuration devices status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-200">userStatusOverview</span><span class="sxs-lookup"><span data-stu-id="75b24-200">userStatusOverview</span></span>|[<span data-ttu-id="75b24-201">deviceConfigurationUserOverview</span><span class="sxs-lookup"><span data-stu-id="75b24-201">deviceConfigurationUserOverview</span></span>](../resources/intune-deviceconfig-deviceconfigurationuseroverview.md)|<span data-ttu-id="75b24-202">デバイス構成のユーザー状態の概要 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="75b24-202">Device Configuration users status overview Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="75b24-203">deviceSettingStateSummaries</span><span class="sxs-lookup"><span data-stu-id="75b24-203">deviceSettingStateSummaries</span></span>|<span data-ttu-id="75b24-204">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="75b24-204">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) collection</span></span>|<span data-ttu-id="75b24-205">デバイス構成設定状態のデバイスの要約 ([deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="75b24-205">Device Configuration Setting State Device Summary Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="75b24-206">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="75b24-206">JSON Representation</span></span>
<span data-ttu-id="75b24-207">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="75b24-207">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.macOSExtensionsConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSExtensionsConfiguration",
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
  "kernelExtensionOverridesAllowed": true,
  "kernelExtensionAllowedTeamIdentifiers": [
    "String"
  ],
  "kernelExtensionsAllowed": [
    {
      "@odata.type": "microsoft.graph.macOSKernelExtension",
      "teamIdentifier": "String",
      "bundleId": "String"
    }
  ]
}
```




