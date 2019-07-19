---
title: Update windows81GeneralConfiguration
description: windows81GeneralConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b1eb084192aac9ed7d8f8f2827cb979b8c3424d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34962233"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="08f48-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="08f48-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="08f48-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08f48-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08f48-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="08f48-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08f48-106">[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="08f48-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08f48-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="08f48-107">Prerequisites</span></span>
<span data-ttu-id="08f48-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="08f48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08f48-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="08f48-110">Permission type</span></span>|<span data-ttu-id="08f48-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="08f48-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08f48-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="08f48-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08f48-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f48-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08f48-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="08f48-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08f48-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08f48-115">Not supported.</span></span>|
|<span data-ttu-id="08f48-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="08f48-116">Application</span></span>|<span data-ttu-id="08f48-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08f48-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08f48-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="08f48-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="08f48-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08f48-119">Request headers</span></span>
|<span data-ttu-id="08f48-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="08f48-120">Header</span></span>|<span data-ttu-id="08f48-121">値</span><span class="sxs-lookup"><span data-stu-id="08f48-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08f48-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08f48-122">Authorization</span></span>|<span data-ttu-id="08f48-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="08f48-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08f48-124">承諾</span><span class="sxs-lookup"><span data-stu-id="08f48-124">Accept</span></span>|<span data-ttu-id="08f48-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08f48-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08f48-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="08f48-126">Request body</span></span>
<span data-ttu-id="08f48-127">要求本文で、[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="08f48-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="08f48-128">次の表に、[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="08f48-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08f48-129">Property</span></span>|<span data-ttu-id="08f48-130">型</span><span class="sxs-lookup"><span data-stu-id="08f48-130">Type</span></span>|<span data-ttu-id="08f48-131">説明</span><span class="sxs-lookup"><span data-stu-id="08f48-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08f48-132">id</span><span class="sxs-lookup"><span data-stu-id="08f48-132">id</span></span>|<span data-ttu-id="08f48-133">文字列</span><span class="sxs-lookup"><span data-stu-id="08f48-133">String</span></span>|<span data-ttu-id="08f48-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="08f48-134">Key of the entity.</span></span> <span data-ttu-id="08f48-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="08f48-136">lastModifiedDateTime</span></span>|<span data-ttu-id="08f48-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f48-137">DateTimeOffset</span></span>|<span data-ttu-id="08f48-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="08f48-138">DateTime the object was last modified.</span></span> <span data-ttu-id="08f48-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="08f48-140">roleScopeTagIds</span></span>|<span data-ttu-id="08f48-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="08f48-141">String collection</span></span>|<span data-ttu-id="08f48-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="08f48-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="08f48-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="08f48-144">supportsScopeTags</span></span>|<span data-ttu-id="08f48-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-145">Boolean</span></span>|<span data-ttu-id="08f48-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="08f48-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="08f48-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="08f48-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="08f48-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="08f48-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="08f48-149">This property is read-only.</span></span> <span data-ttu-id="08f48-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="08f48-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="08f48-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="08f48-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="08f48-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="08f48-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="08f48-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="08f48-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="08f48-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="08f48-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="08f48-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="08f48-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="08f48-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="08f48-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="08f48-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="08f48-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="08f48-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="08f48-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="08f48-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="08f48-163">createdDateTime</span></span>|<span data-ttu-id="08f48-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="08f48-164">DateTimeOffset</span></span>|<span data-ttu-id="08f48-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="08f48-165">DateTime the object was created.</span></span> <span data-ttu-id="08f48-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-167">description</span><span class="sxs-lookup"><span data-stu-id="08f48-167">description</span></span>|<span data-ttu-id="08f48-168">String</span><span class="sxs-lookup"><span data-stu-id="08f48-168">String</span></span>|<span data-ttu-id="08f48-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="08f48-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="08f48-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-171">displayName</span><span class="sxs-lookup"><span data-stu-id="08f48-171">displayName</span></span>|<span data-ttu-id="08f48-172">String</span><span class="sxs-lookup"><span data-stu-id="08f48-172">String</span></span>|<span data-ttu-id="08f48-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="08f48-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="08f48-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-175">version</span><span class="sxs-lookup"><span data-stu-id="08f48-175">version</span></span>|<span data-ttu-id="08f48-176">Int32</span><span class="sxs-lookup"><span data-stu-id="08f48-176">Int32</span></span>|<span data-ttu-id="08f48-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="08f48-177">Version of the device configuration.</span></span> <span data-ttu-id="08f48-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="08f48-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="08f48-179">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="08f48-179">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="08f48-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-180">Boolean</span></span>|<span data-ttu-id="08f48-181">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-181">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="08f48-182">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="08f48-182">applyOnlyToWindows81</span></span>|<span data-ttu-id="08f48-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-183">Boolean</span></span>|<span data-ttu-id="08f48-184">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="08f48-184">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="08f48-185">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="08f48-185">This property is read-only.</span></span>|
|<span data-ttu-id="08f48-186">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="08f48-186">browserBlockAutofill</span></span>|<span data-ttu-id="08f48-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-187">Boolean</span></span>|<span data-ttu-id="08f48-188">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-188">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="08f48-189">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="08f48-189">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="08f48-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-190">Boolean</span></span>|<span data-ttu-id="08f48-191">イントラネット サイトの自動検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-191">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="08f48-192">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="08f48-192">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="08f48-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-193">Boolean</span></span>|<span data-ttu-id="08f48-194">エンタープライズ モードのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-194">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="08f48-195">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="08f48-195">browserBlockJavaScript</span></span>|<span data-ttu-id="08f48-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-196">Boolean</span></span>|<span data-ttu-id="08f48-197">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-197">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="08f48-198">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="08f48-198">browserBlockPlugins</span></span>|<span data-ttu-id="08f48-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-199">Boolean</span></span>|<span data-ttu-id="08f48-200">プラグインを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-200">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="08f48-201">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="08f48-201">browserBlockPopups</span></span>|<span data-ttu-id="08f48-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-202">Boolean</span></span>|<span data-ttu-id="08f48-203">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-203">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="08f48-204">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="08f48-204">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="08f48-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-205">Boolean</span></span>|<span data-ttu-id="08f48-206">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-206">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="08f48-207">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="08f48-207">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="08f48-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-208">Boolean</span></span>|<span data-ttu-id="08f48-209">イントラネット サイトでの 1 単語のエントリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-209">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="08f48-210">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="08f48-210">browserRequireSmartScreen</span></span>|<span data-ttu-id="08f48-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-211">Boolean</span></span>|<span data-ttu-id="08f48-212">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-212">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="08f48-213">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="08f48-213">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="08f48-214">String</span><span class="sxs-lookup"><span data-stu-id="08f48-214">String</span></span>|<span data-ttu-id="08f48-215">エンタープライズ モードのサイト リストの場所。</span><span class="sxs-lookup"><span data-stu-id="08f48-215">The enterprise mode site list location.</span></span> <span data-ttu-id="08f48-216">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="08f48-216">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="08f48-217">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="08f48-217">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="08f48-218">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="08f48-218">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="08f48-219">インターネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="08f48-219">The internet security level.</span></span> <span data-ttu-id="08f48-220">可能な値は、`userDefined`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="08f48-220">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="08f48-221">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="08f48-221">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="08f48-222">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="08f48-222">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="08f48-223">イントラネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="08f48-223">The Intranet security level.</span></span> <span data-ttu-id="08f48-224">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="08f48-224">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="08f48-225">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="08f48-225">browserLoggingReportLocation</span></span>|<span data-ttu-id="08f48-226">String</span><span class="sxs-lookup"><span data-stu-id="08f48-226">String</span></span>|<span data-ttu-id="08f48-227">ログ レポートの場所。</span><span class="sxs-lookup"><span data-stu-id="08f48-227">The logging report location.</span></span>|
|<span data-ttu-id="08f48-228">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="08f48-228">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="08f48-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-229">Boolean</span></span>|<span data-ttu-id="08f48-230">制限付きサイトに対する高度なセキュリティを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-230">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="08f48-231">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="08f48-231">browserRequireFirewall</span></span>|<span data-ttu-id="08f48-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-232">Boolean</span></span>|<span data-ttu-id="08f48-233">ファイアウォールが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-233">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="08f48-234">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="08f48-234">browserRequireFraudWarning</span></span>|<span data-ttu-id="08f48-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-235">Boolean</span></span>|<span data-ttu-id="08f48-236">不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-236">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="08f48-237">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="08f48-237">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="08f48-238">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="08f48-238">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="08f48-239">信頼済みサイトのセキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="08f48-239">The trusted sites security level.</span></span> <span data-ttu-id="08f48-240">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="08f48-240">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="08f48-241">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="08f48-241">cellularBlockDataRoaming</span></span>|<span data-ttu-id="08f48-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-242">Boolean</span></span>|<span data-ttu-id="08f48-243">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-243">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="08f48-244">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="08f48-244">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="08f48-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-245">Boolean</span></span>|<span data-ttu-id="08f48-246">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-246">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="08f48-247">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="08f48-247">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="08f48-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-248">Boolean</span></span>|<span data-ttu-id="08f48-249">ユーザーがピクチャ パスワードおよび暗証番号 (PIN) を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-249">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="08f48-250">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="08f48-250">passwordExpirationDays</span></span>|<span data-ttu-id="08f48-251">Int32</span><span class="sxs-lookup"><span data-stu-id="08f48-251">Int32</span></span>|<span data-ttu-id="08f48-252">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="08f48-252">Password expiration in days.</span></span>|
|<span data-ttu-id="08f48-253">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="08f48-253">passwordMinimumLength</span></span>|<span data-ttu-id="08f48-254">Int32</span><span class="sxs-lookup"><span data-stu-id="08f48-254">Int32</span></span>|<span data-ttu-id="08f48-255">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="08f48-255">The minimum password length.</span></span>|
|<span data-ttu-id="08f48-256">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="08f48-256">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="08f48-257">Int32</span><span class="sxs-lookup"><span data-stu-id="08f48-257">Int32</span></span>|<span data-ttu-id="08f48-258">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="08f48-258">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="08f48-259">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="08f48-259">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="08f48-260">Int32</span><span class="sxs-lookup"><span data-stu-id="08f48-260">Int32</span></span>|<span data-ttu-id="08f48-261">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="08f48-261">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="08f48-262">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="08f48-262">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="08f48-263">Int32</span><span class="sxs-lookup"><span data-stu-id="08f48-263">Int32</span></span>|<span data-ttu-id="08f48-264">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="08f48-264">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="08f48-265">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="08f48-265">Valid values 0 to 24</span></span>|
|<span data-ttu-id="08f48-266">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="08f48-266">passwordRequiredType</span></span>|[<span data-ttu-id="08f48-267">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="08f48-267">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="08f48-268">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="08f48-268">The required password type.</span></span> <span data-ttu-id="08f48-269">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="08f48-269">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="08f48-270">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="08f48-270">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="08f48-271">Int32</span><span class="sxs-lookup"><span data-stu-id="08f48-271">Int32</span></span>|<span data-ttu-id="08f48-272">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="08f48-272">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="08f48-273">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="08f48-273">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="08f48-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-274">Boolean</span></span>|<span data-ttu-id="08f48-275">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-275">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="08f48-276">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="08f48-276">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="08f48-277">updateClassification</span><span class="sxs-lookup"><span data-stu-id="08f48-277">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="08f48-278">自動的にインストールする最小更新プログラムの分類。</span><span class="sxs-lookup"><span data-stu-id="08f48-278">The minimum update classification to install automatically.</span></span> <span data-ttu-id="08f48-279">使用可能な値は、`userDefined`、`recommendedAndImportant`、`important`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="08f48-279">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="08f48-280">Minimumautoinstall分類の更新</span><span class="sxs-lookup"><span data-stu-id="08f48-280">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="08f48-281">updateClassification</span><span class="sxs-lookup"><span data-stu-id="08f48-281">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="08f48-282">自動的にインストールする最小更新プログラムの分類。</span><span class="sxs-lookup"><span data-stu-id="08f48-282">The minimum update classification to install automatically.</span></span> <span data-ttu-id="08f48-283">使用可能な値は、`userDefined`、`recommendedAndImportant`、`important`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="08f48-283">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="08f48-284">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="08f48-284">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="08f48-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="08f48-285">Boolean</span></span>|<span data-ttu-id="08f48-286">自動更新が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="08f48-286">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="08f48-287">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="08f48-287">userAccountControlSettings</span></span>|[<span data-ttu-id="08f48-288">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="08f48-288">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="08f48-289">ユーザー アカウント制御の設定。</span><span class="sxs-lookup"><span data-stu-id="08f48-289">The user account control settings.</span></span> <span data-ttu-id="08f48-290">可能な値は、`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify` です。</span><span class="sxs-lookup"><span data-stu-id="08f48-290">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="08f48-291">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="08f48-291">workFoldersUrl</span></span>|<span data-ttu-id="08f48-292">String</span><span class="sxs-lookup"><span data-stu-id="08f48-292">String</span></span>|<span data-ttu-id="08f48-293">作業フォルダーの URL。</span><span class="sxs-lookup"><span data-stu-id="08f48-293">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="08f48-294">応答</span><span class="sxs-lookup"><span data-stu-id="08f48-294">Response</span></span>
<span data-ttu-id="08f48-295">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="08f48-295">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08f48-296">例</span><span class="sxs-lookup"><span data-stu-id="08f48-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="08f48-297">要求</span><span class="sxs-lookup"><span data-stu-id="08f48-297">Request</span></span>
<span data-ttu-id="08f48-298">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="08f48-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2697

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="08f48-299">応答</span><span class="sxs-lookup"><span data-stu-id="08f48-299">Response</span></span>
<span data-ttu-id="08f48-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="08f48-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2869

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```





