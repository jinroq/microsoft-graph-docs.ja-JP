---
title: Create iosGeneralDeviceConfiguration
description: 新しい iosGeneralDeviceConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18e7f464317481346dd2ba0933f90607de8c3635
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34966727"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="05972-103">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="05972-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="05972-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05972-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="05972-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="05972-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="05972-106">新しい [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="05972-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="05972-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="05972-107">Prerequisites</span></span>
<span data-ttu-id="05972-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05972-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05972-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05972-110">Permission type</span></span>|<span data-ttu-id="05972-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="05972-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05972-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05972-112">Delegated (work or school account)</span></span>|<span data-ttu-id="05972-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05972-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="05972-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05972-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05972-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05972-115">Not supported.</span></span>|
|<span data-ttu-id="05972-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05972-116">Application</span></span>|<span data-ttu-id="05972-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05972-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05972-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05972-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="05972-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05972-119">Request headers</span></span>
|<span data-ttu-id="05972-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05972-120">Header</span></span>|<span data-ttu-id="05972-121">値</span><span class="sxs-lookup"><span data-stu-id="05972-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05972-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="05972-122">Authorization</span></span>|<span data-ttu-id="05972-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="05972-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05972-124">承諾</span><span class="sxs-lookup"><span data-stu-id="05972-124">Accept</span></span>|<span data-ttu-id="05972-125">application/json</span><span class="sxs-lookup"><span data-stu-id="05972-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05972-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="05972-126">Request body</span></span>
<span data-ttu-id="05972-127">要求本文で、iosGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="05972-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="05972-128">次の表に、iosGeneralDeviceConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="05972-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05972-129">Property</span></span>|<span data-ttu-id="05972-130">型</span><span class="sxs-lookup"><span data-stu-id="05972-130">Type</span></span>|<span data-ttu-id="05972-131">説明</span><span class="sxs-lookup"><span data-stu-id="05972-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05972-132">id</span><span class="sxs-lookup"><span data-stu-id="05972-132">id</span></span>|<span data-ttu-id="05972-133">文字列</span><span class="sxs-lookup"><span data-stu-id="05972-133">String</span></span>|<span data-ttu-id="05972-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="05972-134">Key of the entity.</span></span> <span data-ttu-id="05972-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="05972-136">lastModifiedDateTime</span></span>|<span data-ttu-id="05972-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05972-137">DateTimeOffset</span></span>|<span data-ttu-id="05972-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="05972-138">DateTime the object was last modified.</span></span> <span data-ttu-id="05972-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="05972-140">roleScopeTagIds</span></span>|<span data-ttu-id="05972-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="05972-141">String collection</span></span>|<span data-ttu-id="05972-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="05972-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="05972-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="05972-144">supportsScopeTags</span></span>|<span data-ttu-id="05972-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-145">Boolean</span></span>|<span data-ttu-id="05972-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="05972-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="05972-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="05972-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="05972-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="05972-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="05972-149">This property is read-only.</span></span> <span data-ttu-id="05972-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="05972-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="05972-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="05972-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="05972-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="05972-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="05972-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="05972-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="05972-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="05972-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="05972-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="05972-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="05972-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="05972-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="05972-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="05972-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="05972-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="05972-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="05972-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="05972-163">createdDateTime</span></span>|<span data-ttu-id="05972-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="05972-164">DateTimeOffset</span></span>|<span data-ttu-id="05972-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="05972-165">DateTime the object was created.</span></span> <span data-ttu-id="05972-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-167">description</span><span class="sxs-lookup"><span data-stu-id="05972-167">description</span></span>|<span data-ttu-id="05972-168">String</span><span class="sxs-lookup"><span data-stu-id="05972-168">String</span></span>|<span data-ttu-id="05972-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="05972-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="05972-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-171">displayName</span><span class="sxs-lookup"><span data-stu-id="05972-171">displayName</span></span>|<span data-ttu-id="05972-172">String</span><span class="sxs-lookup"><span data-stu-id="05972-172">String</span></span>|<span data-ttu-id="05972-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="05972-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="05972-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-175">version</span><span class="sxs-lookup"><span data-stu-id="05972-175">version</span></span>|<span data-ttu-id="05972-176">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-176">Int32</span></span>|<span data-ttu-id="05972-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="05972-177">Version of the device configuration.</span></span> <span data-ttu-id="05972-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="05972-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="05972-179">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="05972-179">accountBlockModification</span></span>|<span data-ttu-id="05972-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-180">Boolean</span></span>|<span data-ttu-id="05972-181">デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-181">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-182">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="05972-182">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="05972-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-183">Boolean</span></span>|<span data-ttu-id="05972-184">デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-184">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="05972-185">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-185">airDropBlocked</span></span>|<span data-ttu-id="05972-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-186">Boolean</span></span>|<span data-ttu-id="05972-187">デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-187">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-188">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="05972-188">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="05972-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-189">Boolean</span></span>|<span data-ttu-id="05972-190">AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-190">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="05972-191">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="05972-191">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="05972-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-192">Boolean</span></span>|<span data-ttu-id="05972-193">ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-193">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="05972-194">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="05972-194">appleWatchBlockPairing</span></span>|<span data-ttu-id="05972-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-195">Boolean</span></span>|<span data-ttu-id="05972-196">デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-196">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="05972-197">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="05972-197">appleWatchForceWristDetection</span></span>|<span data-ttu-id="05972-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-198">Boolean</span></span>|<span data-ttu-id="05972-199">ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-199">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="05972-200">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-200">appleNewsBlocked</span></span>|<span data-ttu-id="05972-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-201">Boolean</span></span>|<span data-ttu-id="05972-202">デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-202">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="05972-203">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="05972-203">appsSingleAppModeList</span></span>|<span data-ttu-id="05972-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="05972-204">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05972-205">単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="05972-205">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="05972-206">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="05972-206">Supervised only.</span></span> <span data-ttu-id="05972-207">iOS 7.0 以降。</span><span class="sxs-lookup"><span data-stu-id="05972-207">iOS 7.0 and later.</span></span> <span data-ttu-id="05972-208">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="05972-208">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="05972-209">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="05972-209">appsVisibilityList</span></span>|<span data-ttu-id="05972-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="05972-210">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05972-211">可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。</span><span class="sxs-lookup"><span data-stu-id="05972-211">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="05972-212">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="05972-212">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="05972-213">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="05972-213">appsVisibilityListType</span></span>|[<span data-ttu-id="05972-214">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="05972-214">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="05972-215">AppsVisibilityList 内にあるリストの種類です。</span><span class="sxs-lookup"><span data-stu-id="05972-215">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="05972-216">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="05972-216">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="05972-217">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="05972-217">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="05972-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-218">Boolean</span></span>|<span data-ttu-id="05972-219">デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-219">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="05972-220">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-220">appStoreBlocked</span></span>|<span data-ttu-id="05972-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-221">Boolean</span></span>|<span data-ttu-id="05972-222">ユーザーによる App Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-222">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="05972-223">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="05972-223">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="05972-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-224">Boolean</span></span>|<span data-ttu-id="05972-225">ユーザーによるアプリの購入を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-225">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="05972-226">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="05972-226">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="05972-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-227">Boolean</span></span>|<span data-ttu-id="05972-228">ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-228">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="05972-229">監視モードのみに適用されます (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-229">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="05972-230">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="05972-230">appStoreRequirePassword</span></span>|<span data-ttu-id="05972-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-231">Boolean</span></span>|<span data-ttu-id="05972-232">App Store 使用時に、パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="05972-232">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="05972-233">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="05972-233">autoFillForceAuthentication</span></span>|<span data-ttu-id="05972-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-234">Boolean</span></span>|<span data-ttu-id="05972-235">Safari や、監視対象デバイスの他のアプリで、パスワードとクレジットカード情報を自動入力する前に、ユーザー認証を強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-235">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="05972-236">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="05972-236">bluetoothBlockModification</span></span>|<span data-ttu-id="05972-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-237">Boolean</span></span>|<span data-ttu-id="05972-238">デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-238">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="05972-239">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-239">cameraBlocked</span></span>|<span data-ttu-id="05972-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-240">Boolean</span></span>|<span data-ttu-id="05972-241">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-241">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="05972-242">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="05972-242">cellularBlockDataRoaming</span></span>|<span data-ttu-id="05972-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-243">Boolean</span></span>|<span data-ttu-id="05972-244">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-244">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="05972-245">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="05972-245">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="05972-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-246">Boolean</span></span>|<span data-ttu-id="05972-247">ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-247">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="05972-248">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="05972-248">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="05972-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-249">Boolean</span></span>|<span data-ttu-id="05972-250">デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-250">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-251">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="05972-251">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="05972-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-252">Boolean</span></span>|<span data-ttu-id="05972-253">個人用ホットスポットをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-253">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="05972-254">Cellularblockplan の変更</span><span class="sxs-lookup"><span data-stu-id="05972-254">cellularBlockPlanModification</span></span>|<span data-ttu-id="05972-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-255">Boolean</span></span>|<span data-ttu-id="05972-256">ユーザーが、監視対象デバイスの携帯電話プランの設定を変更することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-256">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="05972-257">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="05972-257">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="05972-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-258">Boolean</span></span>|<span data-ttu-id="05972-259">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-259">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="05972-260">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="05972-260">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="05972-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-261">Boolean</span></span>|<span data-ttu-id="05972-262">信頼されていない TLS の証明書をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-262">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="05972-263">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="05972-263">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="05972-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-264">Boolean</span></span>|<span data-ttu-id="05972-265">デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-265">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="05972-266">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="05972-266">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="05972-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-267">Boolean</span></span>|<span data-ttu-id="05972-268">デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-268">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-269">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="05972-269">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="05972-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-270">Boolean</span></span>|<span data-ttu-id="05972-271">デバイスが監視モードのときに、学生に確認せずに教師の要求に対して自動的にアクセス許可を付与するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-271">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-272">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="05972-272">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="05972-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-273">Boolean</span></span>|<span data-ttu-id="05972-274">学生にメッセージを表示せずに、アプリまたはデバイスのロックを教師に許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-274">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="05972-275">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="05972-275">Supervised only.</span></span>|
|<span data-ttu-id="05972-276">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="05972-276">compliantAppsList</span></span>|<span data-ttu-id="05972-277">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="05972-277">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="05972-278">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="05972-278">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="05972-279">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="05972-279">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="05972-280">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="05972-280">compliantAppListType</span></span>|[<span data-ttu-id="05972-281">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="05972-281">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="05972-282">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="05972-282">List that is in the AppComplianceList.</span></span> <span data-ttu-id="05972-283">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="05972-283">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="05972-284">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="05972-284">configurationProfileBlockChanges</span></span>|<span data-ttu-id="05972-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-285">Boolean</span></span>|<span data-ttu-id="05972-286">デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-286">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-287">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-287">definitionLookupBlocked</span></span>|<span data-ttu-id="05972-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-288">Boolean</span></span>|<span data-ttu-id="05972-289">デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-289">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="05972-290">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="05972-290">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="05972-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-291">Boolean</span></span>|<span data-ttu-id="05972-292">デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-292">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-293">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="05972-293">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="05972-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-294">Boolean</span></span>|<span data-ttu-id="05972-295">デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-295">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-296">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="05972-296">deviceBlockNameModification</span></span>|<span data-ttu-id="05972-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-297">Boolean</span></span>|<span data-ttu-id="05972-298">デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-298">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="05972-299">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="05972-299">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="05972-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-300">Boolean</span></span>|<span data-ttu-id="05972-301">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-301">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="05972-302">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="05972-302">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="05972-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-303">Boolean</span></span>|<span data-ttu-id="05972-304">デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-304">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="05972-305">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="05972-305">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="05972-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-306">Boolean</span></span>|<span data-ttu-id="05972-307">ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-307">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="05972-308">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="05972-308">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="05972-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-309">Boolean</span></span>|<span data-ttu-id="05972-310">ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-310">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="05972-311">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="05972-311">emailInDomainSuffixes</span></span>|<span data-ttu-id="05972-312">String コレクション</span><span class="sxs-lookup"><span data-stu-id="05972-312">String collection</span></span>|<span data-ttu-id="05972-313">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="05972-313">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="05972-314">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="05972-314">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="05972-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-315">Boolean</span></span>|<span data-ttu-id="05972-316">ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-316">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="05972-317">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="05972-317">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="05972-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-318">Boolean</span></span>|<span data-ttu-id="05972-319">ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-319">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="05972-320">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="05972-320">esimBlockModification</span></span>|<span data-ttu-id="05972-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-321">Boolean</span></span>|<span data-ttu-id="05972-322">監視対象デバイスの eSIM での携帯電話プランの追加または削除を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-322">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="05972-323">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-323">faceTimeBlocked</span></span>|<span data-ttu-id="05972-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-324">Boolean</span></span>|<span data-ttu-id="05972-325">ユーザーによる FaceTime の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-325">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="05972-326">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-326">findMyFriendsBlocked</span></span>|<span data-ttu-id="05972-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-327">Boolean</span></span>|<span data-ttu-id="05972-328">デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-328">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-329">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="05972-329">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="05972-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-330">Boolean</span></span>|<span data-ttu-id="05972-331">ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-331">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="05972-332">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="05972-332">gamingBlockMultiplayer</span></span>|<span data-ttu-id="05972-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-333">Boolean</span></span>|<span data-ttu-id="05972-334">ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-334">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="05972-335">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-335">gameCenterBlocked</span></span>|<span data-ttu-id="05972-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-336">Boolean</span></span>|<span data-ttu-id="05972-337">デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-337">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-338">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-338">hostPairingBlocked</span></span>|<span data-ttu-id="05972-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-339">Boolean</span></span>|<span data-ttu-id="05972-340">iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-340">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-341">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-341">iBooksStoreBlocked</span></span>|<span data-ttu-id="05972-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-342">Boolean</span></span>|<span data-ttu-id="05972-343">デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-343">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-344">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="05972-344">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="05972-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-345">Boolean</span></span>|<span data-ttu-id="05972-346">アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-346">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="05972-347">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="05972-347">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="05972-348">ブール型</span><span class="sxs-lookup"><span data-stu-id="05972-348">Boolean</span></span>|<span data-ttu-id="05972-349">ユーザーが iOS デバイスで開始された作業を別の iOS デバイスまたは macOS デバイスに継続して実行することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-349">Indicates whether or not to block the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="05972-350">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="05972-350">iCloudBlockBackup</span></span>|<span data-ttu-id="05972-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-351">Boolean</span></span>|<span data-ttu-id="05972-352">iCloud バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-352">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="05972-353">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="05972-353">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="05972-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-354">Boolean</span></span>|<span data-ttu-id="05972-355">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-355">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="05972-356">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="05972-356">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="05972-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-357">Boolean</span></span>|<span data-ttu-id="05972-358">管理対象アプリのクラウドの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-358">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="05972-359">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="05972-359">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="05972-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-360">Boolean</span></span>|<span data-ttu-id="05972-361">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-361">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="05972-362">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="05972-362">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="05972-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-363">Boolean</span></span>|<span data-ttu-id="05972-364">iCloud フォトのストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-364">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="05972-365">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="05972-365">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="05972-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-366">Boolean</span></span>|<span data-ttu-id="05972-367">共有フォト ストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-367">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="05972-368">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="05972-368">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="05972-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-369">Boolean</span></span>|<span data-ttu-id="05972-370">iCloud のバックアップを暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-370">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="05972-371">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="05972-371">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="05972-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-372">Boolean</span></span>|<span data-ttu-id="05972-373">ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="05972-373">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="05972-374">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="05972-374">iTunesBlockMusicService</span></span>|<span data-ttu-id="05972-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-375">Boolean</span></span>|<span data-ttu-id="05972-376">デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-376">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="05972-377">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="05972-377">iTunesBlockRadio</span></span>|<span data-ttu-id="05972-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-378">Boolean</span></span>|<span data-ttu-id="05972-379">デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-379">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="05972-380">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="05972-380">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="05972-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-381">Boolean</span></span>|<span data-ttu-id="05972-382">デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-382">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="05972-383">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="05972-383">keyboardBlockDictation</span></span>|<span data-ttu-id="05972-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-384">Boolean</span></span>|<span data-ttu-id="05972-385">デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-385">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-386">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="05972-386">keyboardBlockPredictive</span></span>|<span data-ttu-id="05972-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-387">Boolean</span></span>|<span data-ttu-id="05972-388">デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-388">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="05972-389">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="05972-389">keyboardBlockShortcuts</span></span>|<span data-ttu-id="05972-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-390">Boolean</span></span>|<span data-ttu-id="05972-391">デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-391">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="05972-392">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="05972-392">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="05972-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-393">Boolean</span></span>|<span data-ttu-id="05972-394">デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-394">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="05972-395">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="05972-395">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="05972-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-396">Boolean</span></span>|<span data-ttu-id="05972-397">キオスク モード時の補助音声を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-397">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-398">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="05972-398">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="05972-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-399">Boolean</span></span>|<span data-ttu-id="05972-400">キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-400">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-401">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="05972-401">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="05972-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-402">Boolean</span></span>|<span data-ttu-id="05972-403">キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-403">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="05972-404">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="05972-404">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="05972-405">代わりに KioskModeBlockAutoLock を使用します。</span><span class="sxs-lookup"><span data-stu-id="05972-405">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="05972-406">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="05972-406">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="05972-407">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-407">Boolean</span></span>|<span data-ttu-id="05972-408">キオスクモード時にデバイスの自動ロックをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-408">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-409">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="05972-409">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="05972-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-410">Boolean</span></span>|<span data-ttu-id="05972-411">キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-411">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-412">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="05972-412">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="05972-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-413">Boolean</span></span>|<span data-ttu-id="05972-414">キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-414">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="05972-415">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="05972-415">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="05972-416">代わりに KioskModeBlockRingerSwitch を使用します。</span><span class="sxs-lookup"><span data-stu-id="05972-416">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="05972-417">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="05972-417">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="05972-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-418">Boolean</span></span>|<span data-ttu-id="05972-419">キオスクモード時の着信音スイッチの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-419">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-420">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="05972-420">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="05972-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-421">Boolean</span></span>|<span data-ttu-id="05972-422">キオスク モード時の画面の回転を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-422">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="05972-423">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="05972-423">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="05972-424">代わりに KioskModeBlockScreenRotation を使用します。</span><span class="sxs-lookup"><span data-stu-id="05972-424">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="05972-425">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="05972-425">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="05972-426">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-426">Boolean</span></span>|<span data-ttu-id="05972-427">キオスクモード時の画面の回転を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-427">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-428">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="05972-428">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="05972-429">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-429">Boolean</span></span>|<span data-ttu-id="05972-430">キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-430">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="05972-431">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="05972-431">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="05972-432">代わりに KioskModeBlockSleepButton を使用します。</span><span class="sxs-lookup"><span data-stu-id="05972-432">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="05972-433">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="05972-433">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="05972-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-434">Boolean</span></span>|<span data-ttu-id="05972-435">キオスクモード時のスリープボタンの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-435">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-436">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="05972-436">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="05972-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-437">Boolean</span></span>|<span data-ttu-id="05972-438">キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-438">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="05972-439">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="05972-439">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="05972-440">代わりに KioskModeBlockTouchscreen を使用します。</span><span class="sxs-lookup"><span data-stu-id="05972-440">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="05972-441">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="05972-441">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="05972-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-442">Boolean</span></span>|<span data-ttu-id="05972-443">キオスクモード時のタッチスクリーンの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-443">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-444">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="05972-444">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="05972-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-445">Boolean</span></span>|<span data-ttu-id="05972-446">キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-446">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-447">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="05972-447">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="05972-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-448">Boolean</span></span>|<span data-ttu-id="05972-449">キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-449">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="05972-450">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="05972-450">This property's functionality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="05972-451">代わりに KioskModeBlockVolumeButtons を使用します。</span><span class="sxs-lookup"><span data-stu-id="05972-451">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="05972-452">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="05972-452">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="05972-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-453">Boolean</span></span>|<span data-ttu-id="05972-454">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-454">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="05972-455">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="05972-455">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="05972-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-456">Boolean</span></span>|<span data-ttu-id="05972-457">キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-457">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-458">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="05972-458">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="05972-459">String</span><span class="sxs-lookup"><span data-stu-id="05972-459">String</span></span>|<span data-ttu-id="05972-460">キオスク モード用に使用するアプリへの、App Store 内の URL。</span><span class="sxs-lookup"><span data-stu-id="05972-460">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="05972-461">KioskModeManagedAppId が不明な場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="05972-461">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="05972-462">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="05972-462">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="05972-463">String</span><span class="sxs-lookup"><span data-stu-id="05972-463">String</span></span>|<span data-ttu-id="05972-464">キオスクモード用に使用する組み込みアプリの ID。</span><span class="sxs-lookup"><span data-stu-id="05972-464">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="05972-465">KioskModeManagedAppId および KioskModeAppStoreUrl が設定されていない場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="05972-465">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="05972-466">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="05972-466">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="05972-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-467">Boolean</span></span>|<span data-ttu-id="05972-468">キオスク モード時に Assistive Touch が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-468">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-469">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="05972-469">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="05972-470">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-470">Boolean</span></span>|<span data-ttu-id="05972-471">キオスク モード時に色反転が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-471">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-472">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="05972-472">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="05972-473">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-473">Boolean</span></span>|<span data-ttu-id="05972-474">キオスク モード時にモノラル オーディオが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-474">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-475">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="05972-475">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="05972-476">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-476">Boolean</span></span>|<span data-ttu-id="05972-477">キオスク モード時にボイス オーバーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-477">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-478">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="05972-478">kioskModeRequireZoom</span></span>|<span data-ttu-id="05972-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-479">Boolean</span></span>|<span data-ttu-id="05972-480">キオスク モード時にズームが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-480">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="05972-481">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="05972-481">kioskModeManagedAppId</span></span>|<span data-ttu-id="05972-482">String</span><span class="sxs-lookup"><span data-stu-id="05972-482">String</span></span>|<span data-ttu-id="05972-483">キオスク モード用に使用するアプリの管理対象アプリ ID。</span><span class="sxs-lookup"><span data-stu-id="05972-483">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="05972-484">KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。</span><span class="sxs-lookup"><span data-stu-id="05972-484">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="05972-485">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="05972-485">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="05972-486">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-486">Boolean</span></span>|<span data-ttu-id="05972-487">ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-487">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="05972-488">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="05972-488">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="05972-489">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-489">Boolean</span></span>|<span data-ttu-id="05972-490">ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-490">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="05972-491">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="05972-491">lockScreenBlockPassbook</span></span>|<span data-ttu-id="05972-492">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-492">Boolean</span></span>|<span data-ttu-id="05972-493">デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-493">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="05972-494">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="05972-494">lockScreenBlockTodayView</span></span>|<span data-ttu-id="05972-495">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-495">Boolean</span></span>|<span data-ttu-id="05972-496">ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-496">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="05972-497">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="05972-497">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="05972-498">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="05972-498">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="05972-499">メディア コンテンツの評価の設定 (オーストラリア向け)</span><span class="sxs-lookup"><span data-stu-id="05972-499">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="05972-500">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="05972-500">mediaContentRatingCanada</span></span>|[<span data-ttu-id="05972-501">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="05972-501">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="05972-502">メディア コンテンツの評価の設定 (カナダ向け)</span><span class="sxs-lookup"><span data-stu-id="05972-502">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="05972-503">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="05972-503">mediaContentRatingFrance</span></span>|[<span data-ttu-id="05972-504">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="05972-504">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="05972-505">メディア コンテンツの評価の設定 (フランス向け)</span><span class="sxs-lookup"><span data-stu-id="05972-505">Media content rating settings for France</span></span>|
|<span data-ttu-id="05972-506">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="05972-506">mediaContentRatingGermany</span></span>|[<span data-ttu-id="05972-507">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="05972-507">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="05972-508">メディア コンテンツの評価の設定 (ドイツ向け)</span><span class="sxs-lookup"><span data-stu-id="05972-508">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="05972-509">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="05972-509">mediaContentRatingIreland</span></span>|[<span data-ttu-id="05972-510">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="05972-510">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="05972-511">メディア コンテンツの評価の設定 (アイルランド向け)</span><span class="sxs-lookup"><span data-stu-id="05972-511">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="05972-512">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="05972-512">mediaContentRatingJapan</span></span>|[<span data-ttu-id="05972-513">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="05972-513">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="05972-514">メディア コンテンツの評価の設定 (日本向け)</span><span class="sxs-lookup"><span data-stu-id="05972-514">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="05972-515">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="05972-515">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="05972-516">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="05972-516">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="05972-517">メディア コンテンツの評価の設定 (ニュージーランド向け)</span><span class="sxs-lookup"><span data-stu-id="05972-517">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="05972-518">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="05972-518">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="05972-519">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="05972-519">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="05972-520">メディア コンテンツの評価の設定 (英国向け)</span><span class="sxs-lookup"><span data-stu-id="05972-520">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="05972-521">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="05972-521">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="05972-522">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="05972-522">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="05972-523">メディア コンテンツの評価の設定 (米国向け)</span><span class="sxs-lookup"><span data-stu-id="05972-523">Media content rating settings for United States</span></span>|
|<span data-ttu-id="05972-524">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="05972-524">networkUsageRules</span></span>|<span data-ttu-id="05972-525">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="05972-525">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="05972-526">管理対象アプリと、それらに適用されるネットワーク ルールのリストです。</span><span class="sxs-lookup"><span data-stu-id="05972-526">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="05972-527">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="05972-527">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="05972-528">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="05972-528">mediaContentRatingApps</span></span>|[<span data-ttu-id="05972-529">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="05972-529">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="05972-530">アプリのメディアコンテンツの評価の設定。</span><span class="sxs-lookup"><span data-stu-id="05972-530">Media content rating settings for Apps.</span></span> <span data-ttu-id="05972-531">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="05972-531">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="05972-532">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-532">messagesBlocked</span></span>|<span data-ttu-id="05972-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-533">Boolean</span></span>|<span data-ttu-id="05972-534">ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-534">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="05972-535">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="05972-535">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="05972-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-536">Boolean</span></span>|<span data-ttu-id="05972-537">通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-537">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="05972-538">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="05972-538">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="05972-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-539">Boolean</span></span>|<span data-ttu-id="05972-540">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-540">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="05972-541">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="05972-541">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="05972-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-542">Boolean</span></span>|<span data-ttu-id="05972-543">監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。</span><span class="sxs-lookup"><span data-stu-id="05972-543">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="05972-544">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="05972-544">passcodeBlockModification</span></span>|<span data-ttu-id="05972-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-545">Boolean</span></span>|<span data-ttu-id="05972-546">監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-546">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="05972-547">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="05972-547">passcodeBlockSimple</span></span>|<span data-ttu-id="05972-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-548">Boolean</span></span>|<span data-ttu-id="05972-549">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-549">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="05972-550">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="05972-550">passcodeExpirationDays</span></span>|<span data-ttu-id="05972-551">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-551">Int32</span></span>|<span data-ttu-id="05972-552">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="05972-552">Number of days before the passcode expires.</span></span> <span data-ttu-id="05972-553">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="05972-553">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="05972-554">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="05972-554">passcodeMinimumLength</span></span>|<span data-ttu-id="05972-555">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-555">Int32</span></span>|<span data-ttu-id="05972-556">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="05972-556">Minimum length of passcode.</span></span> <span data-ttu-id="05972-557">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="05972-557">Valid values 4 to 14</span></span>|
|<span data-ttu-id="05972-558">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="05972-558">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="05972-559">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-559">Int32</span></span>|<span data-ttu-id="05972-560">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="05972-560">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="05972-561">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="05972-561">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="05972-562">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-562">Int32</span></span>|<span data-ttu-id="05972-563">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="05972-563">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="05972-564">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="05972-564">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="05972-565">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-565">Int32</span></span>|<span data-ttu-id="05972-566">パスコードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="05972-566">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="05972-567">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="05972-567">Valid values 0 to 4</span></span>|
|<span data-ttu-id="05972-568">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="05972-568">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="05972-569">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-569">Int32</span></span>|<span data-ttu-id="05972-570">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="05972-570">Number of previous passcodes to block.</span></span> <span data-ttu-id="05972-571">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="05972-571">Valid values 1 to 24</span></span>|
|<span data-ttu-id="05972-572">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="05972-572">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="05972-573">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-573">Int32</span></span>|<span data-ttu-id="05972-574">デバイスをワイプするまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="05972-574">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="05972-575">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="05972-575">Valid values 4 to 11</span></span>|
|<span data-ttu-id="05972-576">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="05972-576">passcodeRequiredType</span></span>|[<span data-ttu-id="05972-577">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="05972-577">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="05972-578">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="05972-578">Type of passcode that is required.</span></span> <span data-ttu-id="05972-579">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="05972-579">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="05972-580">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="05972-580">passcodeRequired</span></span>|<span data-ttu-id="05972-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-581">Boolean</span></span>|<span data-ttu-id="05972-582">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="05972-582">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="05972-583">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-583">podcastsBlocked</span></span>|<span data-ttu-id="05972-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-584">Boolean</span></span>|<span data-ttu-id="05972-585">ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-585">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="05972-586">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="05972-586">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="05972-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-587">Boolean</span></span>|<span data-ttu-id="05972-588">監視対象デバイスで近くのデバイスをセットアップするためのプロンプトを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-588">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="05972-589">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="05972-589">safariBlockAutofill</span></span>|<span data-ttu-id="05972-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-590">Boolean</span></span>|<span data-ttu-id="05972-591">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-591">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="05972-592">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="05972-592">safariBlockJavaScript</span></span>|<span data-ttu-id="05972-593">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-593">Boolean</span></span>|<span data-ttu-id="05972-594">Safari 内で JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-594">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="05972-595">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="05972-595">safariBlockPopups</span></span>|<span data-ttu-id="05972-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-596">Boolean</span></span>|<span data-ttu-id="05972-597">Safari 内でポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-597">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="05972-598">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-598">safariBlocked</span></span>|<span data-ttu-id="05972-599">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-599">Boolean</span></span>|<span data-ttu-id="05972-600">ユーザーによる Safari の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-600">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="05972-601">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="05972-601">safariCookieSettings</span></span>|[<span data-ttu-id="05972-602">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="05972-602">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="05972-603">Safari の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="05972-603">Cookie settings for Safari.</span></span> <span data-ttu-id="05972-604">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="05972-604">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="05972-605">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="05972-605">safariManagedDomains</span></span>|<span data-ttu-id="05972-606">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="05972-606">String collection</span></span>|<span data-ttu-id="05972-607">ここに記載されているパターンに一致する URL は管理対象と見なされます。</span><span class="sxs-lookup"><span data-stu-id="05972-607">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="05972-608">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="05972-608">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="05972-609">String コレクション</span><span class="sxs-lookup"><span data-stu-id="05972-609">String collection</span></span>|<span data-ttu-id="05972-610">ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。</span><span class="sxs-lookup"><span data-stu-id="05972-610">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="05972-611">監視モードのデバイスに適用されます (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-611">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="05972-612">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="05972-612">safariRequireFraudWarning</span></span>|<span data-ttu-id="05972-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-613">Boolean</span></span>|<span data-ttu-id="05972-614">Safari での不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-614">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="05972-615">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-615">screenCaptureBlocked</span></span>|<span data-ttu-id="05972-616">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-616">Boolean</span></span>|<span data-ttu-id="05972-617">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-617">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="05972-618">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-618">siriBlocked</span></span>|<span data-ttu-id="05972-619">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-619">Boolean</span></span>|<span data-ttu-id="05972-620">ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-620">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="05972-621">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="05972-621">siriBlockedWhenLocked</span></span>|<span data-ttu-id="05972-622">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-622">Boolean</span></span>|<span data-ttu-id="05972-623">ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-623">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="05972-624">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="05972-624">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="05972-625">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-625">Boolean</span></span>|<span data-ttu-id="05972-626">監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-626">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="05972-627">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="05972-627">siriRequireProfanityFilter</span></span>|<span data-ttu-id="05972-628">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-628">Boolean</span></span>|<span data-ttu-id="05972-629">Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-629">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="05972-630">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="05972-630">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="05972-631">Int32</span><span class="sxs-lookup"><span data-stu-id="05972-631">Int32</span></span>|<span data-ttu-id="05972-632">監視対象デバイスに対してソフトウェア更新プログラムが delyed される日数を設定します。</span><span class="sxs-lookup"><span data-stu-id="05972-632">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="05972-633">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="05972-633">Valid values 0 to 90</span></span>|
|<span data-ttu-id="05972-634">ソフトウェアの更新 Force延期</span><span class="sxs-lookup"><span data-stu-id="05972-634">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="05972-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-635">Boolean</span></span>|<span data-ttu-id="05972-636">デバイスが監視モードのときに、ユーザーのソフトウェア更新プログラムの表示を延期するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-636">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-637">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="05972-637">spotlightBlockInternetResults</span></span>|<span data-ttu-id="05972-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-638">Boolean</span></span>|<span data-ttu-id="05972-639">監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-639">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="05972-640">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-640">voiceDialingBlocked</span></span>|<span data-ttu-id="05972-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-641">Boolean</span></span>|<span data-ttu-id="05972-642">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-642">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="05972-643">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="05972-643">wallpaperBlockModification</span></span>|<span data-ttu-id="05972-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-644">Boolean</span></span>|<span data-ttu-id="05972-645">監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-645">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="05972-646">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="05972-646">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="05972-647">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-647">Boolean</span></span>|<span data-ttu-id="05972-648">デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-648">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="05972-649">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="05972-649">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="05972-650">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-650">Boolean</span></span>|<span data-ttu-id="05972-651">教室経由で管理されていないコースに登録された学生が、コースを離れるときに教師にアクセス許可を要求するかどうかを示します (iOS 11.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-651">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="05972-652">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="05972-652">keychainBlockCloudSync</span></span>|<span data-ttu-id="05972-653">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-653">Boolean</span></span>|<span data-ttu-id="05972-654">ICloud のキーチェーン同期がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-654">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="05972-655">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="05972-655">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="05972-656">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-656">Boolean</span></span>|<span data-ttu-id="05972-657">空軍の PKI 更新がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-657">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="05972-658">この制限を false に設定しても、CRL および OCSP チェック (iOS 7.0 以降) は無効になりません。</span><span class="sxs-lookup"><span data-stu-id="05972-658">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="05972-659">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="05972-659">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="05972-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-660">Boolean</span></span>|<span data-ttu-id="05972-661">Ad の追跡が制限されているかどうかを示します。(iOS 7.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-661">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="05972-662">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="05972-662">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="05972-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-663">Boolean</span></span>|<span data-ttu-id="05972-664">エンタープライズブックのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-664">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="05972-665">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="05972-665">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="05972-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-666">Boolean</span></span>|<span data-ttu-id="05972-667">エンタープライズブックのメモと強調表示の同期がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-667">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="05972-668">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-668">airPrintBlocked</span></span>|<span data-ttu-id="05972-669">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-669">Boolean</span></span>|<span data-ttu-id="05972-670">放映印刷をブロックするかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-670">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="05972-671">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="05972-671">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="05972-672">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-672">Boolean</span></span>|<span data-ttu-id="05972-673">放映された印刷に対して、ユーザー名とパスワードのキーチェーンストレージをブロックするかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-673">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="05972-674">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="05972-674">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="05972-675">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-675">Boolean</span></span>|<span data-ttu-id="05972-676">TLS 印刷通信 (iOS 11.0 以降) に対して信頼できる証明書が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-676">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="05972-677">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="05972-677">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="05972-678">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-678">Boolean</span></span>|<span data-ttu-id="05972-679">放映された印刷プリンターの iBeacon 検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-679">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="05972-680">これにより、ネットワークトラフィック (iOS 11.0 以降) では、フィッシングからの Bluetooth ビーコンを誤って印刷することがなくなります。</span><span class="sxs-lookup"><span data-stu-id="05972-680">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="05972-681">blockSystemAppRemoval 削除</span><span class="sxs-lookup"><span data-stu-id="05972-681">blockSystemAppRemoval</span></span>|<span data-ttu-id="05972-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-682">Boolean</span></span>|<span data-ttu-id="05972-683">デバイスからのシステムアプリの削除が、監視対象デバイスでブロックされているかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-683">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="05972-684">vpnBlockCreation 作成</span><span class="sxs-lookup"><span data-stu-id="05972-684">vpnBlockCreation</span></span>|<span data-ttu-id="05972-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-685">Boolean</span></span>|<span data-ttu-id="05972-686">VPN 構成の作成がブロックされるかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-686">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="05972-687">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-687">appRemovalBlocked</span></span>|<span data-ttu-id="05972-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-688">Boolean</span></span>|<span data-ttu-id="05972-689">アプリの削除が許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-689">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="05972-690">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="05972-690">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="05972-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-691">Boolean</span></span>|<span data-ttu-id="05972-692">デバイスがロックされているときに USB アクセサリへの接続が許可されるかどうかを示します (iOS 11.4.1 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-692">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="05972-693">passwordBlockAutoFill フィル</span><span class="sxs-lookup"><span data-stu-id="05972-693">passwordBlockAutoFill</span></span>|<span data-ttu-id="05972-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-694">Boolean</span></span>|<span data-ttu-id="05972-695">パスワードのオートフィル機能が許可されているかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-695">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="05972-696">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="05972-696">passwordBlockProximityRequests</span></span>|<span data-ttu-id="05972-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-697">Boolean</span></span>|<span data-ttu-id="05972-698">近くのデバイスからのパスワードの要求をブロックするかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-698">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="05972-699">Passwordblockエア Drop共有</span><span class="sxs-lookup"><span data-stu-id="05972-699">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="05972-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-700">Boolean</span></span>|<span data-ttu-id="05972-701">通話ドロップパスワード機能 iOS 12.0 以降) でのパスワードの共有を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="05972-701">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="05972-702">dateAndTimeForceSetAutomatically に</span><span class="sxs-lookup"><span data-stu-id="05972-702">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="05972-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-703">Boolean</span></span>|<span data-ttu-id="05972-704">ユーザーが日付と時刻を自動的に設定する機能が有効であるかどうか、およびユーザーが無効にすることができないかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-704">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="05972-705">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="05972-705">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="05972-706">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-706">Boolean</span></span>|<span data-ttu-id="05972-707">管理対象アプリが、管理されていない連絡先アカウントに連絡先を書き込むことができるかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-707">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="05972-708">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="05972-708">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="05972-709">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-709">Boolean</span></span>|<span data-ttu-id="05972-710">管理対象外アプリが管理された連絡先から読み取ることができるかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-710">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="05972-711">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="05972-711">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="05972-712">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-712">Boolean</span></span>|<span data-ttu-id="05972-713">ユーザーが個人用ホットスポットの設定を変更することを禁止するかどうかを示します (iOS 12.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-713">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="05972-714">siriDisableServerLogging</span><span class="sxs-lookup"><span data-stu-id="05972-714">siriDisableServerLogging</span></span>|<span data-ttu-id="05972-715">Boolean</span><span class="sxs-lookup"><span data-stu-id="05972-715">Boolean</span></span>|<span data-ttu-id="05972-716">サーバー側の Siri ログが無効かどうかを示します (iOS 12.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="05972-716">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="05972-717">応答</span><span class="sxs-lookup"><span data-stu-id="05972-717">Response</span></span>
<span data-ttu-id="05972-718">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="05972-718">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05972-719">例</span><span class="sxs-lookup"><span data-stu-id="05972-719">Example</span></span>

### <a name="request"></a><span data-ttu-id="05972-720">要求</span><span class="sxs-lookup"><span data-stu-id="05972-720">Request</span></span>
<span data-ttu-id="05972-721">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05972-721">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 10159

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
  "siriDisableServerLogging": true
}
```

### <a name="response"></a><span data-ttu-id="05972-722">応答</span><span class="sxs-lookup"><span data-stu-id="05972-722">Response</span></span>
<span data-ttu-id="05972-p142">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="05972-p142">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 10331

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
  "siriDisableServerLogging": true
}
```





