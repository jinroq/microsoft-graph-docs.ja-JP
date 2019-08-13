---
title: Update iosGeneralDeviceConfiguration
description: iosGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 614f61d9ed3c627fdf57e39481b1ed7ba677d2ec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36315892"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="b5717-103">Update iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b5717-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="b5717-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5717-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5717-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5717-106">[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b5717-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5717-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b5717-107">Prerequisites</span></span>
<span data-ttu-id="b5717-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5717-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5717-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b5717-110">Permission type</span></span>|<span data-ttu-id="b5717-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b5717-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5717-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b5717-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b5717-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5717-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5717-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b5717-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5717-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b5717-115">Not supported.</span></span>|
|<span data-ttu-id="b5717-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b5717-116">Application</span></span>|<span data-ttu-id="b5717-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5717-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5717-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b5717-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b5717-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5717-119">Request headers</span></span>
|<span data-ttu-id="b5717-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b5717-120">Header</span></span>|<span data-ttu-id="b5717-121">値</span><span class="sxs-lookup"><span data-stu-id="b5717-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5717-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5717-122">Authorization</span></span>|<span data-ttu-id="b5717-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5717-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b5717-124">Accept</span></span>|<span data-ttu-id="b5717-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b5717-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5717-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b5717-126">Request body</span></span>
<span data-ttu-id="b5717-127">要求本文で、[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b5717-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="b5717-128">次の表に、[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="b5717-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5717-129">Property</span></span>|<span data-ttu-id="b5717-130">型</span><span class="sxs-lookup"><span data-stu-id="b5717-130">Type</span></span>|<span data-ttu-id="b5717-131">説明</span><span class="sxs-lookup"><span data-stu-id="b5717-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5717-132">id</span><span class="sxs-lookup"><span data-stu-id="b5717-132">id</span></span>|<span data-ttu-id="b5717-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b5717-133">String</span></span>|<span data-ttu-id="b5717-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b5717-134">Key of the entity.</span></span> <span data-ttu-id="b5717-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5717-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b5717-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5717-137">DateTimeOffset</span></span>|<span data-ttu-id="b5717-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="b5717-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b5717-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b5717-140">roleScopeTagIds</span></span>|<span data-ttu-id="b5717-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b5717-141">String collection</span></span>|<span data-ttu-id="b5717-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b5717-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b5717-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b5717-144">supportsScopeTags</span></span>|<span data-ttu-id="b5717-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-145">Boolean</span></span>|<span data-ttu-id="b5717-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b5717-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="b5717-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b5717-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="b5717-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b5717-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-149">This property is read-only.</span></span> <span data-ttu-id="b5717-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5717-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b5717-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b5717-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b5717-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="b5717-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b5717-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5717-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b5717-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b5717-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b5717-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b5717-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b5717-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b5717-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b5717-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="b5717-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b5717-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="b5717-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b5717-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5717-163">createdDateTime</span></span>|<span data-ttu-id="b5717-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5717-164">DateTimeOffset</span></span>|<span data-ttu-id="b5717-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="b5717-165">DateTime the object was created.</span></span> <span data-ttu-id="b5717-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-167">description</span><span class="sxs-lookup"><span data-stu-id="b5717-167">description</span></span>|<span data-ttu-id="b5717-168">String</span><span class="sxs-lookup"><span data-stu-id="b5717-168">String</span></span>|<span data-ttu-id="b5717-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="b5717-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b5717-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b5717-171">displayName</span></span>|<span data-ttu-id="b5717-172">String</span><span class="sxs-lookup"><span data-stu-id="b5717-172">String</span></span>|<span data-ttu-id="b5717-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="b5717-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b5717-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-175">version</span><span class="sxs-lookup"><span data-stu-id="b5717-175">version</span></span>|<span data-ttu-id="b5717-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-176">Int32</span></span>|<span data-ttu-id="b5717-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="b5717-177">Version of the device configuration.</span></span> <span data-ttu-id="b5717-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b5717-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b5717-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="b5717-179">accountBlockModification</span></span>|<span data-ttu-id="b5717-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-180">Boolean</span></span>|<span data-ttu-id="b5717-181">デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="b5717-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="b5717-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-183">Boolean</span></span>|<span data-ttu-id="b5717-184">デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="b5717-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-185">airDropBlocked</span></span>|<span data-ttu-id="b5717-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-186">Boolean</span></span>|<span data-ttu-id="b5717-187">デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="b5717-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="b5717-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-189">Boolean</span></span>|<span data-ttu-id="b5717-190">AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b5717-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="b5717-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="b5717-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-192">Boolean</span></span>|<span data-ttu-id="b5717-193">ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="b5717-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="b5717-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="b5717-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-195">Boolean</span></span>|<span data-ttu-id="b5717-196">デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b5717-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="b5717-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="b5717-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-198">Boolean</span></span>|<span data-ttu-id="b5717-199">ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="b5717-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-200">appleNewsBlocked</span></span>|<span data-ttu-id="b5717-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-201">Boolean</span></span>|<span data-ttu-id="b5717-202">デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b5717-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="b5717-203">appsSingleAppModeList</span></span>|<span data-ttu-id="b5717-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5717-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b5717-205">単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="b5717-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="b5717-206">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="b5717-206">Supervised only.</span></span> <span data-ttu-id="b5717-207">iOS 7.0 以降。</span><span class="sxs-lookup"><span data-stu-id="b5717-207">iOS 7.0 and later.</span></span> <span data-ttu-id="b5717-208">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b5717-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="b5717-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="b5717-209">appsVisibilityList</span></span>|<span data-ttu-id="b5717-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5717-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b5717-211">可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。</span><span class="sxs-lookup"><span data-stu-id="b5717-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="b5717-212">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b5717-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b5717-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="b5717-213">appsVisibilityListType</span></span>|[<span data-ttu-id="b5717-214">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="b5717-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b5717-215">AppsVisibilityList 内にあるリストの種類です。</span><span class="sxs-lookup"><span data-stu-id="b5717-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="b5717-216">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="b5717-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b5717-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="b5717-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="b5717-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-218">Boolean</span></span>|<span data-ttu-id="b5717-219">デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b5717-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-220">appStoreBlocked</span></span>|<span data-ttu-id="b5717-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-221">Boolean</span></span>|<span data-ttu-id="b5717-222">ユーザーによる App Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-222">Indicates whether or not to block the user from using the App Store.</span></span> <span data-ttu-id="b5717-223">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-223">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-224">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="b5717-224">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="b5717-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-225">Boolean</span></span>|<span data-ttu-id="b5717-226">ユーザーによるアプリの購入を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-226">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="b5717-227">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="b5717-227">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="b5717-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-228">Boolean</span></span>|<span data-ttu-id="b5717-229">ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-229">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="b5717-230">監視モードのみに適用されます (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-230">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b5717-231">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="b5717-231">appStoreRequirePassword</span></span>|<span data-ttu-id="b5717-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-232">Boolean</span></span>|<span data-ttu-id="b5717-233">App Store 使用時に、パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b5717-233">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="b5717-234">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="b5717-234">autoFillForceAuthentication</span></span>|<span data-ttu-id="b5717-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-235">Boolean</span></span>|<span data-ttu-id="b5717-236">Safari や、監視対象デバイスの他のアプリで、パスワードとクレジットカード情報を自動入力する前に、ユーザー認証を強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-236">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="b5717-237">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="b5717-237">bluetoothBlockModification</span></span>|<span data-ttu-id="b5717-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-238">Boolean</span></span>|<span data-ttu-id="b5717-239">デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-239">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="b5717-240">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-240">cameraBlocked</span></span>|<span data-ttu-id="b5717-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-241">Boolean</span></span>|<span data-ttu-id="b5717-242">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-242">Indicates whether or not to block the user from accessing the camera of the device.</span></span> <span data-ttu-id="b5717-243">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-243">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-244">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="b5717-244">cellularBlockDataRoaming</span></span>|<span data-ttu-id="b5717-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-245">Boolean</span></span>|<span data-ttu-id="b5717-246">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-246">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="b5717-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="b5717-247">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="b5717-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-248">Boolean</span></span>|<span data-ttu-id="b5717-249">ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-249">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="b5717-250">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="b5717-250">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="b5717-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-251">Boolean</span></span>|<span data-ttu-id="b5717-252">デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-252">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-253">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="b5717-253">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="b5717-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-254">Boolean</span></span>|<span data-ttu-id="b5717-255">個人用ホットスポットをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-255">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="b5717-256">Cellularblockplan の変更</span><span class="sxs-lookup"><span data-stu-id="b5717-256">cellularBlockPlanModification</span></span>|<span data-ttu-id="b5717-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-257">Boolean</span></span>|<span data-ttu-id="b5717-258">ユーザーが、監視対象デバイスの携帯電話プランの設定を変更することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-258">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="b5717-259">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="b5717-259">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="b5717-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-260">Boolean</span></span>|<span data-ttu-id="b5717-261">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-261">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="b5717-262">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="b5717-262">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="b5717-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-263">Boolean</span></span>|<span data-ttu-id="b5717-264">信頼されていない TLS の証明書をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-264">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="b5717-265">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b5717-265">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="b5717-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-266">Boolean</span></span>|<span data-ttu-id="b5717-267">デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-267">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b5717-268">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="b5717-268">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="b5717-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-269">Boolean</span></span>|<span data-ttu-id="b5717-270">デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-270">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-271">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="b5717-271">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="b5717-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-272">Boolean</span></span>|<span data-ttu-id="b5717-273">デバイスが監視モードのときに、学生に確認せずに教師の要求に対して自動的にアクセス許可を付与するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-273">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-274">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="b5717-274">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="b5717-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-275">Boolean</span></span>|<span data-ttu-id="b5717-276">学生にメッセージを表示せずに、アプリまたはデバイスのロックを教師に許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-276">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="b5717-277">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="b5717-277">Supervised only.</span></span>|
|<span data-ttu-id="b5717-278">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="b5717-278">compliantAppsList</span></span>|<span data-ttu-id="b5717-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5717-279">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="b5717-280">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="b5717-280">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="b5717-281">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b5717-281">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="b5717-282">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="b5717-282">compliantAppListType</span></span>|[<span data-ttu-id="b5717-283">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="b5717-283">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="b5717-284">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="b5717-284">List that is in the AppComplianceList.</span></span> <span data-ttu-id="b5717-285">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="b5717-285">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="b5717-286">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="b5717-286">configurationProfileBlockChanges</span></span>|<span data-ttu-id="b5717-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-287">Boolean</span></span>|<span data-ttu-id="b5717-288">デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-288">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-289">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-289">definitionLookupBlocked</span></span>|<span data-ttu-id="b5717-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-290">Boolean</span></span>|<span data-ttu-id="b5717-291">デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-291">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="b5717-292">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="b5717-292">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="b5717-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-293">Boolean</span></span>|<span data-ttu-id="b5717-294">デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-294">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-295">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="b5717-295">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="b5717-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-296">Boolean</span></span>|<span data-ttu-id="b5717-297">デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-297">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-298">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="b5717-298">deviceBlockNameModification</span></span>|<span data-ttu-id="b5717-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-299">Boolean</span></span>|<span data-ttu-id="b5717-300">デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-300">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b5717-301">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="b5717-301">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="b5717-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-302">Boolean</span></span>|<span data-ttu-id="b5717-303">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-303">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="b5717-304">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="b5717-304">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="b5717-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-305">Boolean</span></span>|<span data-ttu-id="b5717-306">デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-306">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="b5717-307">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="b5717-307">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="b5717-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-308">Boolean</span></span>|<span data-ttu-id="b5717-309">ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-309">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="b5717-310">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="b5717-310">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="b5717-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-311">Boolean</span></span>|<span data-ttu-id="b5717-312">ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-312">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="b5717-313">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="b5717-313">emailInDomainSuffixes</span></span>|<span data-ttu-id="b5717-314">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b5717-314">String collection</span></span>|<span data-ttu-id="b5717-315">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="b5717-315">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="b5717-316">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="b5717-316">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="b5717-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-317">Boolean</span></span>|<span data-ttu-id="b5717-318">ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-318">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="b5717-319">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="b5717-319">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="b5717-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-320">Boolean</span></span>|<span data-ttu-id="b5717-321">ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-321">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="b5717-322">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="b5717-322">esimBlockModification</span></span>|<span data-ttu-id="b5717-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-323">Boolean</span></span>|<span data-ttu-id="b5717-324">監視対象デバイスの eSIM での携帯電話プランの追加または削除を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-324">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="b5717-325">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-325">faceTimeBlocked</span></span>|<span data-ttu-id="b5717-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-326">Boolean</span></span>|<span data-ttu-id="b5717-327">ユーザーによる FaceTime の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-327">Indicates whether or not to block the user from using FaceTime.</span></span> <span data-ttu-id="b5717-328">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-328">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-329">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-329">findMyFriendsBlocked</span></span>|<span data-ttu-id="b5717-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-330">Boolean</span></span>|<span data-ttu-id="b5717-331">デバイスが監視モードのときに、友人を検索するための変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-331">Indicates whether or not to block changes to Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-332">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="b5717-332">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="b5717-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-333">Boolean</span></span>|<span data-ttu-id="b5717-334">ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-334">Indicates whether or not to block the user from having friends in Game Center.</span></span> <span data-ttu-id="b5717-335">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-335">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-336">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="b5717-336">gamingBlockMultiplayer</span></span>|<span data-ttu-id="b5717-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-337">Boolean</span></span>|<span data-ttu-id="b5717-338">ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-338">Indicates whether or not to block the user from using multiplayer gaming.</span></span> <span data-ttu-id="b5717-339">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-339">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-340">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-340">gameCenterBlocked</span></span>|<span data-ttu-id="b5717-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-341">Boolean</span></span>|<span data-ttu-id="b5717-342">デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-342">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-343">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-343">hostPairingBlocked</span></span>|<span data-ttu-id="b5717-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-344">Boolean</span></span>|<span data-ttu-id="b5717-345">iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-345">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-346">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-346">iBooksStoreBlocked</span></span>|<span data-ttu-id="b5717-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-347">Boolean</span></span>|<span data-ttu-id="b5717-348">デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-348">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-349">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="b5717-349">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="b5717-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-350">Boolean</span></span>|<span data-ttu-id="b5717-351">アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-351">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="b5717-352">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="b5717-352">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="b5717-353">ブール型</span><span class="sxs-lookup"><span data-stu-id="b5717-353">Boolean</span></span>|<span data-ttu-id="b5717-354">ユーザーが iOS デバイスで開始された作業を別の iOS デバイスまたは macOS デバイスに継続して実行することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-354">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="b5717-355">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b5717-355">iCloudBlockBackup</span></span>|<span data-ttu-id="b5717-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-356">Boolean</span></span>|<span data-ttu-id="b5717-357">iCloud バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-357">Indicates whether or not to block iCloud backup.</span></span> <span data-ttu-id="b5717-358">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-358">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-359">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="b5717-359">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="b5717-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-360">Boolean</span></span>|<span data-ttu-id="b5717-361">ICloud ドキュメントの同期をブロックするかどうかを示します。IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-361">Indicates whether or not to block iCloud document sync. Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-362">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="b5717-362">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="b5717-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-363">Boolean</span></span>|<span data-ttu-id="b5717-364">管理対象アプリのクラウドの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-364">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="b5717-365">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="b5717-365">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="b5717-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-366">Boolean</span></span>|<span data-ttu-id="b5717-367">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-367">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="b5717-368">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="b5717-368">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="b5717-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-369">Boolean</span></span>|<span data-ttu-id="b5717-370">iCloud フォトのストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-370">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="b5717-371">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="b5717-371">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="b5717-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-372">Boolean</span></span>|<span data-ttu-id="b5717-373">共有フォト ストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-373">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="b5717-374">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="b5717-374">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="b5717-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-375">Boolean</span></span>|<span data-ttu-id="b5717-376">iCloud のバックアップを暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-376">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="b5717-377">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="b5717-377">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="b5717-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-378">Boolean</span></span>|<span data-ttu-id="b5717-379">ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b5717-379">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span> <span data-ttu-id="b5717-380">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-380">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-381">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="b5717-381">iTunesBlockMusicService</span></span>|<span data-ttu-id="b5717-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-382">Boolean</span></span>|<span data-ttu-id="b5717-383">デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-383">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="b5717-384">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="b5717-384">iTunesBlockRadio</span></span>|<span data-ttu-id="b5717-385">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-385">Boolean</span></span>|<span data-ttu-id="b5717-386">デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-386">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b5717-387">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="b5717-387">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="b5717-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-388">Boolean</span></span>|<span data-ttu-id="b5717-389">デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-389">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b5717-390">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="b5717-390">keyboardBlockDictation</span></span>|<span data-ttu-id="b5717-391">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-391">Boolean</span></span>|<span data-ttu-id="b5717-392">デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-392">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-393">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="b5717-393">keyboardBlockPredictive</span></span>|<span data-ttu-id="b5717-394">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-394">Boolean</span></span>|<span data-ttu-id="b5717-395">デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-395">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b5717-396">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="b5717-396">keyboardBlockShortcuts</span></span>|<span data-ttu-id="b5717-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-397">Boolean</span></span>|<span data-ttu-id="b5717-398">デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-398">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b5717-399">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="b5717-399">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="b5717-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-400">Boolean</span></span>|<span data-ttu-id="b5717-401">デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-401">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="b5717-402">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="b5717-402">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="b5717-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-403">Boolean</span></span>|<span data-ttu-id="b5717-404">キオスク モード時の補助音声を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-404">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-405">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="b5717-405">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="b5717-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-406">Boolean</span></span>|<span data-ttu-id="b5717-407">キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-407">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-408">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="b5717-408">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="b5717-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-409">Boolean</span></span>|<span data-ttu-id="b5717-410">キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-410">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="b5717-411">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="b5717-411">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b5717-412">代わりに KioskModeBlockAutoLock を使用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-412">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="b5717-413">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="b5717-413">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="b5717-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-414">Boolean</span></span>|<span data-ttu-id="b5717-415">キオスクモード時にデバイスの自動ロックをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-415">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-416">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="b5717-416">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="b5717-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-417">Boolean</span></span>|<span data-ttu-id="b5717-418">キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-418">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-419">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="b5717-419">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="b5717-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-420">Boolean</span></span>|<span data-ttu-id="b5717-421">キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-421">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="b5717-422">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="b5717-422">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b5717-423">代わりに KioskModeBlockRingerSwitch を使用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-423">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="b5717-424">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="b5717-424">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="b5717-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-425">Boolean</span></span>|<span data-ttu-id="b5717-426">キオスクモード時の着信音スイッチの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-426">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-427">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="b5717-427">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="b5717-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-428">Boolean</span></span>|<span data-ttu-id="b5717-429">キオスク モード時の画面の回転を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-429">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="b5717-430">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="b5717-430">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b5717-431">代わりに KioskModeBlockScreenRotation を使用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-431">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="b5717-432">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="b5717-432">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="b5717-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-433">Boolean</span></span>|<span data-ttu-id="b5717-434">キオスクモード時の画面の回転を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-434">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-435">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="b5717-435">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="b5717-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-436">Boolean</span></span>|<span data-ttu-id="b5717-437">キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-437">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="b5717-438">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="b5717-438">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b5717-439">代わりに KioskModeBlockSleepButton を使用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-439">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="b5717-440">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="b5717-440">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="b5717-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-441">Boolean</span></span>|<span data-ttu-id="b5717-442">キオスクモード時のスリープボタンの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-442">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-443">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="b5717-443">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="b5717-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-444">Boolean</span></span>|<span data-ttu-id="b5717-445">キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-445">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="b5717-446">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="b5717-446">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b5717-447">代わりに KioskModeBlockTouchscreen を使用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-447">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="b5717-448">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="b5717-448">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="b5717-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-449">Boolean</span></span>|<span data-ttu-id="b5717-450">キオスクモード時のタッチスクリーンの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-450">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-451">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="b5717-451">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="b5717-452">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-452">Boolean</span></span>|<span data-ttu-id="b5717-453">キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-453">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-454">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b5717-454">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="b5717-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-455">Boolean</span></span>|<span data-ttu-id="b5717-456">キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-456">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="b5717-457">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="b5717-457">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="b5717-458">代わりに KioskModeBlockVolumeButtons を使用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-458">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="b5717-459">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="b5717-459">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="b5717-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-460">Boolean</span></span>|<span data-ttu-id="b5717-461">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-461">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="b5717-462">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="b5717-462">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="b5717-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-463">Boolean</span></span>|<span data-ttu-id="b5717-464">キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-464">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-465">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b5717-465">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="b5717-466">String</span><span class="sxs-lookup"><span data-stu-id="b5717-466">String</span></span>|<span data-ttu-id="b5717-467">キオスク モード用に使用するアプリへの、App Store 内の URL。</span><span class="sxs-lookup"><span data-stu-id="b5717-467">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="b5717-468">KioskModeManagedAppId が不明な場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-468">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="b5717-469">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="b5717-469">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="b5717-470">String</span><span class="sxs-lookup"><span data-stu-id="b5717-470">String</span></span>|<span data-ttu-id="b5717-471">キオスクモード用に使用する組み込みアプリの ID。</span><span class="sxs-lookup"><span data-stu-id="b5717-471">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="b5717-472">KioskModeManagedAppId および KioskModeAppStoreUrl が設定されていない場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="b5717-472">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="b5717-473">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="b5717-473">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="b5717-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-474">Boolean</span></span>|<span data-ttu-id="b5717-475">キオスク モード時に Assistive Touch が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-475">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-476">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="b5717-476">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="b5717-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-477">Boolean</span></span>|<span data-ttu-id="b5717-478">キオスク モード時に色反転が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-478">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-479">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="b5717-479">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="b5717-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-480">Boolean</span></span>|<span data-ttu-id="b5717-481">キオスク モード時にモノラル オーディオが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-481">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-482">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="b5717-482">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="b5717-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-483">Boolean</span></span>|<span data-ttu-id="b5717-484">キオスク モード時にボイス オーバーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-484">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-485">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="b5717-485">kioskModeRequireZoom</span></span>|<span data-ttu-id="b5717-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-486">Boolean</span></span>|<span data-ttu-id="b5717-487">キオスク モード時にズームが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-487">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="b5717-488">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="b5717-488">kioskModeManagedAppId</span></span>|<span data-ttu-id="b5717-489">String</span><span class="sxs-lookup"><span data-stu-id="b5717-489">String</span></span>|<span data-ttu-id="b5717-490">キオスク モード用に使用するアプリの管理対象アプリ ID。</span><span class="sxs-lookup"><span data-stu-id="b5717-490">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="b5717-491">KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。</span><span class="sxs-lookup"><span data-stu-id="b5717-491">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="b5717-492">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="b5717-492">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="b5717-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-493">Boolean</span></span>|<span data-ttu-id="b5717-494">ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-494">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="b5717-495">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="b5717-495">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="b5717-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-496">Boolean</span></span>|<span data-ttu-id="b5717-497">ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-497">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="b5717-498">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="b5717-498">lockScreenBlockPassbook</span></span>|<span data-ttu-id="b5717-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-499">Boolean</span></span>|<span data-ttu-id="b5717-500">デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-500">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="b5717-501">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="b5717-501">lockScreenBlockTodayView</span></span>|<span data-ttu-id="b5717-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-502">Boolean</span></span>|<span data-ttu-id="b5717-503">ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-503">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="b5717-504">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b5717-504">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="b5717-505">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="b5717-505">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="b5717-506">メディア コンテンツの評価の設定 (オーストラリア向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-506">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="b5717-507">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b5717-507">mediaContentRatingCanada</span></span>|[<span data-ttu-id="b5717-508">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="b5717-508">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="b5717-509">メディア コンテンツの評価の設定 (カナダ向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-509">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="b5717-510">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b5717-510">mediaContentRatingFrance</span></span>|[<span data-ttu-id="b5717-511">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="b5717-511">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="b5717-512">メディア コンテンツの評価の設定 (フランス向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-512">Media content rating settings for France</span></span>|
|<span data-ttu-id="b5717-513">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b5717-513">mediaContentRatingGermany</span></span>|[<span data-ttu-id="b5717-514">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="b5717-514">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="b5717-515">メディア コンテンツの評価の設定 (ドイツ向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-515">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="b5717-516">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b5717-516">mediaContentRatingIreland</span></span>|[<span data-ttu-id="b5717-517">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="b5717-517">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="b5717-518">メディア コンテンツの評価の設定 (アイルランド向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-518">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="b5717-519">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b5717-519">mediaContentRatingJapan</span></span>|[<span data-ttu-id="b5717-520">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="b5717-520">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="b5717-521">メディア コンテンツの評価の設定 (日本向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-521">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="b5717-522">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b5717-522">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="b5717-523">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="b5717-523">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="b5717-524">メディア コンテンツの評価の設定 (ニュージーランド向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-524">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="b5717-525">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b5717-525">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="b5717-526">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="b5717-526">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="b5717-527">メディア コンテンツの評価の設定 (英国向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-527">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="b5717-528">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b5717-528">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="b5717-529">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="b5717-529">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="b5717-530">メディア コンテンツの評価の設定 (米国向け)</span><span class="sxs-lookup"><span data-stu-id="b5717-530">Media content rating settings for United States</span></span>|
|<span data-ttu-id="b5717-531">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="b5717-531">networkUsageRules</span></span>|<span data-ttu-id="b5717-532">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5717-532">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="b5717-533">管理対象アプリと、それらに適用されるネットワーク ルールのリストです。</span><span class="sxs-lookup"><span data-stu-id="b5717-533">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="b5717-534">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b5717-534">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="b5717-535">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="b5717-535">mediaContentRatingApps</span></span>|[<span data-ttu-id="b5717-536">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="b5717-536">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="b5717-537">アプリのメディアコンテンツの評価の設定。</span><span class="sxs-lookup"><span data-stu-id="b5717-537">Media content rating settings for Apps.</span></span> <span data-ttu-id="b5717-538">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="b5717-538">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="b5717-539">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-539">messagesBlocked</span></span>|<span data-ttu-id="b5717-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-540">Boolean</span></span>|<span data-ttu-id="b5717-541">ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-541">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="b5717-542">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="b5717-542">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="b5717-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-543">Boolean</span></span>|<span data-ttu-id="b5717-544">通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-544">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b5717-545">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="b5717-545">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="b5717-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-546">Boolean</span></span>|<span data-ttu-id="b5717-547">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-547">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="b5717-548">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="b5717-548">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="b5717-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-549">Boolean</span></span>|<span data-ttu-id="b5717-550">監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。</span><span class="sxs-lookup"><span data-stu-id="b5717-550">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="b5717-551">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="b5717-551">passcodeBlockModification</span></span>|<span data-ttu-id="b5717-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-552">Boolean</span></span>|<span data-ttu-id="b5717-553">監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-553">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="b5717-554">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b5717-554">passcodeBlockSimple</span></span>|<span data-ttu-id="b5717-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-555">Boolean</span></span>|<span data-ttu-id="b5717-556">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-556">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="b5717-557">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b5717-557">passcodeExpirationDays</span></span>|<span data-ttu-id="b5717-558">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-558">Int32</span></span>|<span data-ttu-id="b5717-559">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="b5717-559">Number of days before the passcode expires.</span></span> <span data-ttu-id="b5717-560">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="b5717-560">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b5717-561">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b5717-561">passcodeMinimumLength</span></span>|<span data-ttu-id="b5717-562">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-562">Int32</span></span>|<span data-ttu-id="b5717-563">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="b5717-563">Minimum length of passcode.</span></span> <span data-ttu-id="b5717-564">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="b5717-564">Valid values 4 to 14</span></span>|
|<span data-ttu-id="b5717-565">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="b5717-565">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="b5717-566">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-566">Int32</span></span>|<span data-ttu-id="b5717-567">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="b5717-567">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="b5717-568">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b5717-568">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b5717-569">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-569">Int32</span></span>|<span data-ttu-id="b5717-570">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="b5717-570">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b5717-571">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b5717-571">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="b5717-572">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-572">Int32</span></span>|<span data-ttu-id="b5717-573">パスコードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="b5717-573">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="b5717-574">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="b5717-574">Valid values 0 to 4</span></span>|
|<span data-ttu-id="b5717-575">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="b5717-575">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="b5717-576">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-576">Int32</span></span>|<span data-ttu-id="b5717-577">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="b5717-577">Number of previous passcodes to block.</span></span> <span data-ttu-id="b5717-578">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="b5717-578">Valid values 1 to 24</span></span>|
|<span data-ttu-id="b5717-579">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="b5717-579">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="b5717-580">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-580">Int32</span></span>|<span data-ttu-id="b5717-581">デバイスをワイプするまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="b5717-581">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="b5717-582">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="b5717-582">Valid values 4 to 11</span></span>|
|<span data-ttu-id="b5717-583">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="b5717-583">passcodeRequiredType</span></span>|[<span data-ttu-id="b5717-584">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b5717-584">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b5717-585">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="b5717-585">Type of passcode that is required.</span></span> <span data-ttu-id="b5717-586">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="b5717-586">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b5717-587">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="b5717-587">passcodeRequired</span></span>|<span data-ttu-id="b5717-588">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-588">Boolean</span></span>|<span data-ttu-id="b5717-589">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b5717-589">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="b5717-590">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-590">podcastsBlocked</span></span>|<span data-ttu-id="b5717-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-591">Boolean</span></span>|<span data-ttu-id="b5717-592">ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-592">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="b5717-593">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="b5717-593">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="b5717-594">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-594">Boolean</span></span>|<span data-ttu-id="b5717-595">監視対象デバイスで近くのデバイスをセットアップするためのプロンプトを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-595">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="b5717-596">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b5717-596">safariBlockAutofill</span></span>|<span data-ttu-id="b5717-597">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-597">Boolean</span></span>|<span data-ttu-id="b5717-598">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-598">Indicates whether or not to block the user from using Auto fill in Safari.</span></span> <span data-ttu-id="b5717-599">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-599">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-600">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b5717-600">safariBlockJavaScript</span></span>|<span data-ttu-id="b5717-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-601">Boolean</span></span>|<span data-ttu-id="b5717-602">Safari 内で JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-602">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="b5717-603">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b5717-603">safariBlockPopups</span></span>|<span data-ttu-id="b5717-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-604">Boolean</span></span>|<span data-ttu-id="b5717-605">Safari 内でポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-605">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="b5717-606">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-606">safariBlocked</span></span>|<span data-ttu-id="b5717-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-607">Boolean</span></span>|<span data-ttu-id="b5717-608">ユーザーによる Safari の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-608">Indicates whether or not to block the user from using Safari.</span></span> <span data-ttu-id="b5717-609">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-609">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-610">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b5717-610">safariCookieSettings</span></span>|[<span data-ttu-id="b5717-611">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="b5717-611">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="b5717-612">Safari の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="b5717-612">Cookie settings for Safari.</span></span> <span data-ttu-id="b5717-613">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="b5717-613">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="b5717-614">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="b5717-614">safariManagedDomains</span></span>|<span data-ttu-id="b5717-615">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b5717-615">String collection</span></span>|<span data-ttu-id="b5717-616">ここに記載されているパターンに一致する URL は管理対象と見なされます。</span><span class="sxs-lookup"><span data-stu-id="b5717-616">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="b5717-617">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="b5717-617">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="b5717-618">String コレクション</span><span class="sxs-lookup"><span data-stu-id="b5717-618">String collection</span></span>|<span data-ttu-id="b5717-619">ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。</span><span class="sxs-lookup"><span data-stu-id="b5717-619">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="b5717-620">監視モードのデバイスに適用されます (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-620">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="b5717-621">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="b5717-621">safariRequireFraudWarning</span></span>|<span data-ttu-id="b5717-622">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-622">Boolean</span></span>|<span data-ttu-id="b5717-623">Safari での不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-623">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="b5717-624">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-624">screenCaptureBlocked</span></span>|<span data-ttu-id="b5717-625">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-625">Boolean</span></span>|<span data-ttu-id="b5717-626">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-626">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b5717-627">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-627">siriBlocked</span></span>|<span data-ttu-id="b5717-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-628">Boolean</span></span>|<span data-ttu-id="b5717-629">ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-629">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="b5717-630">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="b5717-630">siriBlockedWhenLocked</span></span>|<span data-ttu-id="b5717-631">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-631">Boolean</span></span>|<span data-ttu-id="b5717-632">ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-632">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="b5717-633">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="b5717-633">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="b5717-634">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-634">Boolean</span></span>|<span data-ttu-id="b5717-635">監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-635">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="b5717-636">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="b5717-636">siriRequireProfanityFilter</span></span>|<span data-ttu-id="b5717-637">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-637">Boolean</span></span>|<span data-ttu-id="b5717-638">Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-638">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="b5717-639">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="b5717-639">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="b5717-640">Int32</span><span class="sxs-lookup"><span data-stu-id="b5717-640">Int32</span></span>|<span data-ttu-id="b5717-641">監視対象デバイスに対してソフトウェア更新プログラムが delyed される日数を設定します。</span><span class="sxs-lookup"><span data-stu-id="b5717-641">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="b5717-642">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="b5717-642">Valid values 0 to 90</span></span>|
|<span data-ttu-id="b5717-643">ソフトウェアの更新 Force延期</span><span class="sxs-lookup"><span data-stu-id="b5717-643">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="b5717-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-644">Boolean</span></span>|<span data-ttu-id="b5717-645">デバイスが監視モードのときに、ユーザーのソフトウェア更新プログラムの表示を延期するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-645">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-646">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="b5717-646">spotlightBlockInternetResults</span></span>|<span data-ttu-id="b5717-647">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-647">Boolean</span></span>|<span data-ttu-id="b5717-648">監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-648">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="b5717-649">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-649">voiceDialingBlocked</span></span>|<span data-ttu-id="b5717-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-650">Boolean</span></span>|<span data-ttu-id="b5717-651">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-651">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="b5717-652">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="b5717-652">wallpaperBlockModification</span></span>|<span data-ttu-id="b5717-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-653">Boolean</span></span>|<span data-ttu-id="b5717-654">監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-654">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="b5717-655">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="b5717-655">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="b5717-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-656">Boolean</span></span>|<span data-ttu-id="b5717-657">デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-657">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="b5717-658">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="b5717-658">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="b5717-659">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-659">Boolean</span></span>|<span data-ttu-id="b5717-660">教室経由で管理されていないコースに登録された学生が、コースを離れるときに教師にアクセス許可を要求するかどうかを示します (iOS 11.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-660">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="b5717-661">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="b5717-661">keychainBlockCloudSync</span></span>|<span data-ttu-id="b5717-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-662">Boolean</span></span>|<span data-ttu-id="b5717-663">ICloud のキーチェーン同期がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-663">Indicates whether or not iCloud keychain synchronization is blocked.</span></span> <span data-ttu-id="b5717-664">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-664">Requires a supervised device for iOS 13 and later.</span></span>|
|<span data-ttu-id="b5717-665">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="b5717-665">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="b5717-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-666">Boolean</span></span>|<span data-ttu-id="b5717-667">空軍の PKI 更新がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-667">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="b5717-668">この制限を false に設定しても、CRL および OCSP チェック (iOS 7.0 以降) は無効になりません。</span><span class="sxs-lookup"><span data-stu-id="b5717-668">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="b5717-669">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="b5717-669">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="b5717-670">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-670">Boolean</span></span>|<span data-ttu-id="b5717-671">Ad の追跡が制限されているかどうかを示します。(iOS 7.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-671">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="b5717-672">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="b5717-672">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="b5717-673">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-673">Boolean</span></span>|<span data-ttu-id="b5717-674">エンタープライズブックのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-674">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="b5717-675">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="b5717-675">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="b5717-676">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-676">Boolean</span></span>|<span data-ttu-id="b5717-677">エンタープライズブックのメモと強調表示の同期がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-677">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="b5717-678">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-678">airPrintBlocked</span></span>|<span data-ttu-id="b5717-679">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-679">Boolean</span></span>|<span data-ttu-id="b5717-680">放映印刷をブロックするかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-680">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b5717-681">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="b5717-681">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="b5717-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-682">Boolean</span></span>|<span data-ttu-id="b5717-683">放映された印刷に対して、ユーザー名とパスワードのキーチェーンストレージをブロックするかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-683">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b5717-684">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="b5717-684">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="b5717-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-685">Boolean</span></span>|<span data-ttu-id="b5717-686">TLS 印刷通信 (iOS 11.0 以降) に対して信頼できる証明書が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-686">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b5717-687">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="b5717-687">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="b5717-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-688">Boolean</span></span>|<span data-ttu-id="b5717-689">放映された印刷プリンターの iBeacon 検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-689">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="b5717-690">これにより、ネットワークトラフィック (iOS 11.0 以降) では、フィッシングからの Bluetooth ビーコンを誤って印刷することがなくなります。</span><span class="sxs-lookup"><span data-stu-id="b5717-690">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b5717-691">blockSystemAppRemoval 削除</span><span class="sxs-lookup"><span data-stu-id="b5717-691">blockSystemAppRemoval</span></span>|<span data-ttu-id="b5717-692">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-692">Boolean</span></span>|<span data-ttu-id="b5717-693">デバイスからのシステムアプリの削除が、監視対象デバイスでブロックされているかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-693">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b5717-694">vpnBlockCreation 作成</span><span class="sxs-lookup"><span data-stu-id="b5717-694">vpnBlockCreation</span></span>|<span data-ttu-id="b5717-695">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-695">Boolean</span></span>|<span data-ttu-id="b5717-696">VPN 構成の作成がブロックされるかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-696">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="b5717-697">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-697">appRemovalBlocked</span></span>|<span data-ttu-id="b5717-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-698">Boolean</span></span>|<span data-ttu-id="b5717-699">アプリの削除が許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-699">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="b5717-700">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-700">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="b5717-701">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-701">Boolean</span></span>|<span data-ttu-id="b5717-702">デバイスがロックされているときに USB アクセサリへの接続が許可されるかどうかを示します (iOS 11.4.1 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-702">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="b5717-703">passwordBlockAutoFill フィル</span><span class="sxs-lookup"><span data-stu-id="b5717-703">passwordBlockAutoFill</span></span>|<span data-ttu-id="b5717-704">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-704">Boolean</span></span>|<span data-ttu-id="b5717-705">パスワードのオートフィル機能が許可されているかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-705">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b5717-706">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="b5717-706">passwordBlockProximityRequests</span></span>|<span data-ttu-id="b5717-707">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-707">Boolean</span></span>|<span data-ttu-id="b5717-708">近くのデバイスからのパスワードの要求をブロックするかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-708">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b5717-709">Passwordblockエア Drop共有</span><span class="sxs-lookup"><span data-stu-id="b5717-709">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="b5717-710">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-710">Boolean</span></span>|<span data-ttu-id="b5717-711">通話ドロップパスワード機能 iOS 12.0 以降) でのパスワードの共有を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-711">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b5717-712">dateAndTimeForceSetAutomatically に</span><span class="sxs-lookup"><span data-stu-id="b5717-712">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="b5717-713">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-713">Boolean</span></span>|<span data-ttu-id="b5717-714">ユーザーが日付と時刻を自動的に設定する機能が有効であるかどうか、およびユーザーが無効にすることができないかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-714">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b5717-715">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="b5717-715">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="b5717-716">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-716">Boolean</span></span>|<span data-ttu-id="b5717-717">管理対象アプリが、管理されていない連絡先アカウントに連絡先を書き込むことができるかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-717">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="b5717-718">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="b5717-718">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="b5717-719">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-719">Boolean</span></span>|<span data-ttu-id="b5717-720">管理対象外アプリが管理された連絡先から読み取ることができるかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-720">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="b5717-721">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="b5717-721">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="b5717-722">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-722">Boolean</span></span>|<span data-ttu-id="b5717-723">ユーザーが個人用ホットスポットの設定を変更することを禁止するかどうかを示します (iOS 12.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-723">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="b5717-724">siriDisableServerLogging</span><span class="sxs-lookup"><span data-stu-id="b5717-724">siriDisableServerLogging</span></span>|<span data-ttu-id="b5717-725">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-725">Boolean</span></span>|<span data-ttu-id="b5717-726">サーバー側の Siri ログが無効かどうかを示します (iOS 12.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-726">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="b5717-727">continuousPathKeyboardBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-727">continuousPathKeyboardBlocked</span></span>|<span data-ttu-id="b5717-728">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-728">Boolean</span></span>|<span data-ttu-id="b5717-729">デバイスの監視時に連続したパスキーボードをブロックするかどうかを示します (iOS 13 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-729">Indicates whether or not to block the continuous path keyboard when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="b5717-730">findMyDeviceInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-730">findMyDeviceInFindMyAppBlocked</span></span>|<span data-ttu-id="b5717-731">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-731">Boolean</span></span>|<span data-ttu-id="b5717-732">デバイスの監視時にデバイスの検索をブロックするかどうかを示します (iOS 13 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-732">Indicates whether or not to block Find My Device when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="b5717-733">findMyFriendsInFindMyAppBlocked</span><span class="sxs-lookup"><span data-stu-id="b5717-733">findMyFriendsInFindMyAppBlocked</span></span>|<span data-ttu-id="b5717-734">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-734">Boolean</span></span>|<span data-ttu-id="b5717-735">デバイスの監視時に友人を検索するかどうかを示します (iOS 13 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-735">Indicates whether or not to block Find My Friends when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="b5717-736">wiFiBlockPowerModification</span><span class="sxs-lookup"><span data-stu-id="b5717-736">wiFiBlockPowerModification</span></span>|<span data-ttu-id="b5717-737">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-737">Boolean</span></span>|<span data-ttu-id="b5717-738">デバイスの監視時に WiFi 電源変更をブロックするかどうかを示します (iOS 13 以降)。</span><span class="sxs-lookup"><span data-stu-id="b5717-738">Indicates whether or not to block WiFi power modification when the device is supervised (iOS 13 or later).</span></span>|
|<span data-ttu-id="b5717-739">ブロック</span><span class="sxs-lookup"><span data-stu-id="b5717-739">iTunesBlocked</span></span>|<span data-ttu-id="b5717-740">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5717-740">Boolean</span></span>|<span data-ttu-id="b5717-741">ITunes アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="b5717-741">Indicates whether or not to block the iTunes app.</span></span> <span data-ttu-id="b5717-742">IOS 13 以降の監視デバイスが必要です。</span><span class="sxs-lookup"><span data-stu-id="b5717-742">Requires a supervised device for iOS 13 and later.</span></span>|



## <a name="response"></a><span data-ttu-id="b5717-743">応答</span><span class="sxs-lookup"><span data-stu-id="b5717-743">Response</span></span>
<span data-ttu-id="b5717-744">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b5717-744">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5717-745">例</span><span class="sxs-lookup"><span data-stu-id="b5717-745">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5717-746">要求</span><span class="sxs-lookup"><span data-stu-id="b5717-746">Request</span></span>
<span data-ttu-id="b5717-747">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b5717-747">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 10353

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "wiFiBlockPowerModification": true,
  "iTunesBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="b5717-748">応答</span><span class="sxs-lookup"><span data-stu-id="b5717-748">Response</span></span>
<span data-ttu-id="b5717-p153">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b5717-p153">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 10525

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
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
  "accountBlockModification": true,
  "activationLockAllowWhenSupervised": true,
  "airDropBlocked": true,
  "airDropForceUnmanagedDropTarget": true,
  "airPlayForcePairingPasswordForOutgoingRequests": true,
  "appleWatchBlockPairing": true,
  "appleWatchForceWristDetection": true,
  "appleNewsBlocked": true,
  "appsSingleAppModeList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "appsVisibilityListType": "appsInListCompliant",
  "appStoreBlockAutomaticDownloads": true,
  "appStoreBlocked": true,
  "appStoreBlockInAppPurchases": true,
  "appStoreBlockUIAppInstallation": true,
  "appStoreRequirePassword": true,
  "autoFillForceAuthentication": true,
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockPlanModification": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "configurationProfileBlockChanges": true,
  "definitionLookupBlocked": true,
  "deviceBlockEnableRestrictions": true,
  "deviceBlockEraseContentAndSettings": true,
  "deviceBlockNameModification": true,
  "diagnosticDataBlockSubmission": true,
  "diagnosticDataBlockSubmissionModification": true,
  "documentsBlockManagedDocumentsInUnmanagedApps": true,
  "documentsBlockUnmanagedDocumentsInManagedApps": true,
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "enterpriseAppBlockTrust": true,
  "enterpriseAppBlockTrustModification": true,
  "esimBlockModification": true,
  "faceTimeBlocked": true,
  "findMyFriendsBlocked": true,
  "gamingBlockGameCenterFriends": true,
  "gamingBlockMultiplayer": true,
  "gameCenterBlocked": true,
  "hostPairingBlocked": true,
  "iBooksStoreBlocked": true,
  "iBooksStoreBlockErotica": true,
  "iCloudBlockActivityContinuation": true,
  "iCloudBlockBackup": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockManagedAppsSync": true,
  "iCloudBlockPhotoLibrary": true,
  "iCloudBlockPhotoStreamSync": true,
  "iCloudBlockSharedPhotoStream": true,
  "iCloudRequireEncryptedBackup": true,
  "iTunesBlockExplicitContent": true,
  "iTunesBlockMusicService": true,
  "iTunesBlockRadio": true,
  "keyboardBlockAutoCorrect": true,
  "keyboardBlockDictation": true,
  "keyboardBlockPredictive": true,
  "keyboardBlockShortcuts": true,
  "keyboardBlockSpellCheck": true,
  "kioskModeAllowAssistiveSpeak": true,
  "kioskModeAllowAssistiveTouchSettings": true,
  "kioskModeAllowAutoLock": true,
  "kioskModeBlockAutoLock": true,
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeBlockRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeBlockScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeBlockSleepButton": true,
  "kioskModeAllowTouchscreen": true,
  "kioskModeBlockTouchscreen": true,
  "kioskModeAllowVoiceOverSettings": true,
  "kioskModeAllowVolumeButtons": true,
  "kioskModeBlockVolumeButtons": true,
  "kioskModeAllowZoomSettings": true,
  "kioskModeAppStoreUrl": "https://example.com/kioskModeAppStoreUrl/",
  "kioskModeBuiltInAppId": "Kiosk Mode Built In App Id value",
  "kioskModeRequireAssistiveTouch": true,
  "kioskModeRequireColorInversion": true,
  "kioskModeRequireMonoAudio": true,
  "kioskModeRequireVoiceOver": true,
  "kioskModeRequireZoom": true,
  "kioskModeManagedAppId": "Kiosk Mode Managed App Id value",
  "lockScreenBlockControlCenter": true,
  "lockScreenBlockNotificationView": true,
  "lockScreenBlockPassbook": true,
  "lockScreenBlockTodayView": true,
  "mediaContentRatingAustralia": {
    "@odata.type": "microsoft.graph.mediaContentRatingAustralia",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingCanada": {
    "@odata.type": "microsoft.graph.mediaContentRatingCanada",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingFrance": {
    "@odata.type": "microsoft.graph.mediaContentRatingFrance",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingGermany": {
    "@odata.type": "microsoft.graph.mediaContentRatingGermany",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingIreland": {
    "@odata.type": "microsoft.graph.mediaContentRatingIreland",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingJapan": {
    "@odata.type": "microsoft.graph.mediaContentRatingJapan",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingNewZealand": {
    "@odata.type": "microsoft.graph.mediaContentRatingNewZealand",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedKingdom": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedKingdom",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "mediaContentRatingUnitedStates": {
    "@odata.type": "microsoft.graph.mediaContentRatingUnitedStates",
    "movieRating": "allBlocked",
    "tvRating": "allBlocked"
  },
  "networkUsageRules": [
    {
      "@odata.type": "microsoft.graph.iosNetworkUsageRule",
      "managedApps": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "cellularDataBlockWhenRoaming": true,
      "cellularDataBlocked": true
    }
  ],
  "mediaContentRatingApps": "allBlocked",
  "messagesBlocked": true,
  "notificationsBlockSettingsModification": true,
  "passcodeBlockFingerprintUnlock": true,
  "passcodeBlockFingerprintModification": true,
  "passcodeBlockModification": true,
  "passcodeBlockSimple": true,
  "passcodeExpirationDays": 6,
  "passcodeMinimumLength": 5,
  "passcodeMinutesOfInactivityBeforeLock": 5,
  "passcodeMinutesOfInactivityBeforeScreenTimeout": 14,
  "passcodeMinimumCharacterSetCount": 0,
  "passcodePreviousPasscodeBlockCount": 2,
  "passcodeSignInFailureCountBeforeWipe": 4,
  "passcodeRequiredType": "alphanumeric",
  "passcodeRequired": true,
  "podcastsBlocked": true,
  "proximityBlockSetupToNewDevice": true,
  "safariBlockAutofill": true,
  "safariBlockJavaScript": true,
  "safariBlockPopups": true,
  "safariBlocked": true,
  "safariCookieSettings": "blockAlways",
  "safariManagedDomains": [
    "Safari Managed Domains value"
  ],
  "safariPasswordAutoFillDomains": [
    "Safari Password Auto Fill Domains value"
  ],
  "safariRequireFraudWarning": true,
  "screenCaptureBlocked": true,
  "siriBlocked": true,
  "siriBlockedWhenLocked": true,
  "siriBlockUserGeneratedContent": true,
  "siriRequireProfanityFilter": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "softwareUpdatesForceDelayed": true,
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "keychainBlockCloudSync": true,
  "pkiBlockOTAUpdates": true,
  "privacyForceLimitAdTracking": true,
  "enterpriseBookBlockBackup": true,
  "enterpriseBookBlockMetadataSync": true,
  "airPrintBlocked": true,
  "airPrintBlockCredentialsStorage": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "blockSystemAppRemoval": true,
  "vpnBlockCreation": true,
  "appRemovalBlocked": true,
  "usbRestrictedModeBlocked": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "dateAndTimeForceSetAutomatically": true,
  "contactsAllowManagedToUnmanagedWrite": true,
  "contactsAllowUnmanagedToManagedRead": true,
  "cellularBlockPersonalHotspotModification": true,
  "siriDisableServerLogging": true,
  "continuousPathKeyboardBlocked": true,
  "findMyDeviceInFindMyAppBlocked": true,
  "findMyFriendsInFindMyAppBlocked": true,
  "wiFiBlockPowerModification": true,
  "iTunesBlocked": true
}
```






