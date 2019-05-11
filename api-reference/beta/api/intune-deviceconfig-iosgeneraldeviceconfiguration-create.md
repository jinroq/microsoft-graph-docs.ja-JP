---
title: Create iosGeneralDeviceConfiguration
description: 新しい iosGeneralDeviceConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4ea0f0e23f63f839e3dfa79e3888aa356eee1376
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33923476"
---
# <a name="create-iosgeneraldeviceconfiguration"></a><span data-ttu-id="6b204-103">Create iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b204-103">Create iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="6b204-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b204-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b204-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b204-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b204-106">新しい [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6b204-106">Create a new [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b204-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6b204-107">Prerequisites</span></span>
<span data-ttu-id="6b204-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b204-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b204-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b204-110">Permission type</span></span>|<span data-ttu-id="6b204-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b204-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b204-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b204-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6b204-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b204-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b204-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b204-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b204-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b204-115">Not supported.</span></span>|
|<span data-ttu-id="6b204-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b204-116">Application</span></span>|<span data-ttu-id="6b204-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b204-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b204-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b204-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="6b204-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b204-119">Request headers</span></span>
|<span data-ttu-id="6b204-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b204-120">Header</span></span>|<span data-ttu-id="6b204-121">値</span><span class="sxs-lookup"><span data-stu-id="6b204-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b204-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b204-122">Authorization</span></span>|<span data-ttu-id="6b204-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6b204-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b204-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6b204-124">Accept</span></span>|<span data-ttu-id="6b204-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6b204-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b204-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b204-126">Request body</span></span>
<span data-ttu-id="6b204-127">要求本文で、iosGeneralDeviceConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b204-127">In the request body, supply a JSON representation for the iosGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="6b204-128">次の表に、iosGeneralDeviceConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-128">The following table shows the properties that are required when you create the iosGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="6b204-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6b204-129">Property</span></span>|<span data-ttu-id="6b204-130">型</span><span class="sxs-lookup"><span data-stu-id="6b204-130">Type</span></span>|<span data-ttu-id="6b204-131">説明</span><span class="sxs-lookup"><span data-stu-id="6b204-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b204-132">id</span><span class="sxs-lookup"><span data-stu-id="6b204-132">id</span></span>|<span data-ttu-id="6b204-133">文字列</span><span class="sxs-lookup"><span data-stu-id="6b204-133">String</span></span>|<span data-ttu-id="6b204-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6b204-134">Key of the entity.</span></span> <span data-ttu-id="6b204-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b204-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b204-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b204-136">lastModifiedDateTime</span></span>|<span data-ttu-id="6b204-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b204-137">DateTimeOffset</span></span>|<span data-ttu-id="6b204-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="6b204-138">DateTime the object was last modified.</span></span> <span data-ttu-id="6b204-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b204-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b204-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="6b204-140">roleScopeTagIds</span></span>|<span data-ttu-id="6b204-141">String collection</span><span class="sxs-lookup"><span data-stu-id="6b204-141">String collection</span></span>|<span data-ttu-id="6b204-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="6b204-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="6b204-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b204-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b204-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="6b204-144">supportsScopeTags</span></span>|<span data-ttu-id="6b204-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-145">Boolean</span></span>|<span data-ttu-id="6b204-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="6b204-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="6b204-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="6b204-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="6b204-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="6b204-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-149">This property is read-only.</span></span> <span data-ttu-id="6b204-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b204-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b204-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b204-151">createdDateTime</span></span>|<span data-ttu-id="6b204-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b204-152">DateTimeOffset</span></span>|<span data-ttu-id="6b204-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="6b204-153">DateTime the object was created.</span></span> <span data-ttu-id="6b204-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b204-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b204-155">description</span><span class="sxs-lookup"><span data-stu-id="6b204-155">description</span></span>|<span data-ttu-id="6b204-156">String</span><span class="sxs-lookup"><span data-stu-id="6b204-156">String</span></span>|<span data-ttu-id="6b204-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="6b204-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b204-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b204-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b204-159">displayName</span><span class="sxs-lookup"><span data-stu-id="6b204-159">displayName</span></span>|<span data-ttu-id="6b204-160">String</span><span class="sxs-lookup"><span data-stu-id="6b204-160">String</span></span>|<span data-ttu-id="6b204-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="6b204-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b204-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b204-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b204-163">version</span><span class="sxs-lookup"><span data-stu-id="6b204-163">version</span></span>|<span data-ttu-id="6b204-164">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-164">Int32</span></span>|<span data-ttu-id="6b204-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="6b204-165">Version of the device configuration.</span></span> <span data-ttu-id="6b204-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6b204-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b204-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="6b204-167">accountBlockModification</span></span>|<span data-ttu-id="6b204-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-168">Boolean</span></span>|<span data-ttu-id="6b204-169">デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="6b204-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="6b204-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-171">Boolean</span></span>|<span data-ttu-id="6b204-172">デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="6b204-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-173">airDropBlocked</span></span>|<span data-ttu-id="6b204-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-174">Boolean</span></span>|<span data-ttu-id="6b204-175">デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="6b204-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="6b204-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-177">Boolean</span></span>|<span data-ttu-id="6b204-178">AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6b204-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="6b204-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="6b204-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-180">Boolean</span></span>|<span data-ttu-id="6b204-181">ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="6b204-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="6b204-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="6b204-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-183">Boolean</span></span>|<span data-ttu-id="6b204-184">デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6b204-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="6b204-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="6b204-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-186">Boolean</span></span>|<span data-ttu-id="6b204-187">ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="6b204-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-188">appleNewsBlocked</span></span>|<span data-ttu-id="6b204-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-189">Boolean</span></span>|<span data-ttu-id="6b204-190">デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6b204-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="6b204-191">appsSingleAppModeList</span></span>|<span data-ttu-id="6b204-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b204-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6b204-193">単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="6b204-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="6b204-194">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="6b204-194">Supervised only.</span></span> <span data-ttu-id="6b204-195">iOS 7.0 以降。</span><span class="sxs-lookup"><span data-stu-id="6b204-195">iOS 7.0 and later.</span></span> <span data-ttu-id="6b204-196">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6b204-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="6b204-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="6b204-197">appsVisibilityList</span></span>|<span data-ttu-id="6b204-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b204-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6b204-199">可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。</span><span class="sxs-lookup"><span data-stu-id="6b204-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="6b204-200">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6b204-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6b204-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="6b204-201">appsVisibilityListType</span></span>|[<span data-ttu-id="6b204-202">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="6b204-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="6b204-203">AppsVisibilityList 内にあるリストの種類です。</span><span class="sxs-lookup"><span data-stu-id="6b204-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="6b204-204">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="6b204-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6b204-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="6b204-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="6b204-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-206">Boolean</span></span>|<span data-ttu-id="6b204-207">デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6b204-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-208">appStoreBlocked</span></span>|<span data-ttu-id="6b204-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-209">Boolean</span></span>|<span data-ttu-id="6b204-210">ユーザーによる App Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="6b204-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="6b204-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="6b204-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-212">Boolean</span></span>|<span data-ttu-id="6b204-213">ユーザーによるアプリの購入を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="6b204-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="6b204-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="6b204-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-215">Boolean</span></span>|<span data-ttu-id="6b204-216">ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="6b204-217">監視モードのみに適用されます (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6b204-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="6b204-218">appStoreRequirePassword</span></span>|<span data-ttu-id="6b204-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-219">Boolean</span></span>|<span data-ttu-id="6b204-220">App Store 使用時に、パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b204-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="6b204-221">autoFillForceAuthentication</span><span class="sxs-lookup"><span data-stu-id="6b204-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="6b204-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-222">Boolean</span></span>|<span data-ttu-id="6b204-223">Safari や、監視対象デバイスの他のアプリで、パスワードとクレジットカード情報を自動入力する前に、ユーザー認証を強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="6b204-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="6b204-224">bluetoothBlockModification</span></span>|<span data-ttu-id="6b204-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-225">Boolean</span></span>|<span data-ttu-id="6b204-226">デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="6b204-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-227">cameraBlocked</span></span>|<span data-ttu-id="6b204-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-228">Boolean</span></span>|<span data-ttu-id="6b204-229">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="6b204-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="6b204-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="6b204-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-231">Boolean</span></span>|<span data-ttu-id="6b204-232">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="6b204-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="6b204-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="6b204-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-234">Boolean</span></span>|<span data-ttu-id="6b204-235">ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="6b204-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="6b204-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="6b204-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-237">Boolean</span></span>|<span data-ttu-id="6b204-238">デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="6b204-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="6b204-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-240">Boolean</span></span>|<span data-ttu-id="6b204-241">個人用ホットスポットをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="6b204-242">Cellularblockplan の変更</span><span class="sxs-lookup"><span data-stu-id="6b204-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="6b204-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-243">Boolean</span></span>|<span data-ttu-id="6b204-244">ユーザーが、監視対象デバイスの携帯電話プランの設定を変更することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="6b204-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="6b204-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="6b204-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-246">Boolean</span></span>|<span data-ttu-id="6b204-247">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="6b204-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="6b204-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="6b204-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-249">Boolean</span></span>|<span data-ttu-id="6b204-250">信頼されていない TLS の証明書をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="6b204-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6b204-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="6b204-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-252">Boolean</span></span>|<span data-ttu-id="6b204-253">デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6b204-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="6b204-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="6b204-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-255">Boolean</span></span>|<span data-ttu-id="6b204-256">デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-257">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="6b204-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="6b204-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-258">Boolean</span></span>|<span data-ttu-id="6b204-259">デバイスが監視モードのときに、学生に確認せずに教師の要求に対して自動的にアクセス許可を付与するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-260">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="6b204-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="6b204-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-261">Boolean</span></span>|<span data-ttu-id="6b204-262">学生にメッセージを表示せずに、アプリまたはデバイスのロックを教師に許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="6b204-263">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="6b204-263">Supervised only.</span></span>|
|<span data-ttu-id="6b204-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="6b204-264">compliantAppsList</span></span>|<span data-ttu-id="6b204-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b204-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="6b204-266">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="6b204-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="6b204-267">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6b204-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="6b204-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="6b204-268">compliantAppListType</span></span>|[<span data-ttu-id="6b204-269">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="6b204-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="6b204-270">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="6b204-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="6b204-271">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="6b204-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="6b204-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="6b204-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="6b204-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-273">Boolean</span></span>|<span data-ttu-id="6b204-274">デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-275">definitionLookupBlocked</span></span>|<span data-ttu-id="6b204-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-276">Boolean</span></span>|<span data-ttu-id="6b204-277">デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="6b204-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="6b204-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="6b204-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-279">Boolean</span></span>|<span data-ttu-id="6b204-280">デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="6b204-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="6b204-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-282">Boolean</span></span>|<span data-ttu-id="6b204-283">デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="6b204-284">deviceBlockNameModification</span></span>|<span data-ttu-id="6b204-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-285">Boolean</span></span>|<span data-ttu-id="6b204-286">デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6b204-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="6b204-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="6b204-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-288">Boolean</span></span>|<span data-ttu-id="6b204-289">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="6b204-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="6b204-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="6b204-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-291">Boolean</span></span>|<span data-ttu-id="6b204-292">デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="6b204-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="6b204-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="6b204-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-294">Boolean</span></span>|<span data-ttu-id="6b204-295">ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="6b204-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="6b204-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="6b204-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-297">Boolean</span></span>|<span data-ttu-id="6b204-298">ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="6b204-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="6b204-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="6b204-300">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6b204-300">String collection</span></span>|<span data-ttu-id="6b204-301">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="6b204-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="6b204-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="6b204-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="6b204-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-303">Boolean</span></span>|<span data-ttu-id="6b204-304">ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="6b204-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="6b204-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="6b204-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-306">Boolean</span></span>|<span data-ttu-id="6b204-307">ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="6b204-308">esimBlockModification</span><span class="sxs-lookup"><span data-stu-id="6b204-308">esimBlockModification</span></span>|<span data-ttu-id="6b204-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-309">Boolean</span></span>|<span data-ttu-id="6b204-310">監視対象デバイスの eSIM での携帯電話プランの追加または削除を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="6b204-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-311">faceTimeBlocked</span></span>|<span data-ttu-id="6b204-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-312">Boolean</span></span>|<span data-ttu-id="6b204-313">ユーザーによる FaceTime の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="6b204-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="6b204-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-315">Boolean</span></span>|<span data-ttu-id="6b204-316">デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="6b204-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="6b204-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-318">Boolean</span></span>|<span data-ttu-id="6b204-319">ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="6b204-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="6b204-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="6b204-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-321">Boolean</span></span>|<span data-ttu-id="6b204-322">ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="6b204-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-323">gameCenterBlocked</span></span>|<span data-ttu-id="6b204-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-324">Boolean</span></span>|<span data-ttu-id="6b204-325">デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-326">hostPairingBlocked</span></span>|<span data-ttu-id="6b204-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-327">Boolean</span></span>|<span data-ttu-id="6b204-328">iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="6b204-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-330">Boolean</span></span>|<span data-ttu-id="6b204-331">デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="6b204-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="6b204-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-333">Boolean</span></span>|<span data-ttu-id="6b204-334">アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="6b204-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="6b204-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="6b204-336">ブール型</span><span class="sxs-lookup"><span data-stu-id="6b204-336">Boolean</span></span>|<span data-ttu-id="6b204-337">ユーザーが iOS デバイスで開始された作業を別の iOS デバイスまたは macOS デバイスに継続して実行することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="6b204-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="6b204-338">iCloudBlockBackup</span></span>|<span data-ttu-id="6b204-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-339">Boolean</span></span>|<span data-ttu-id="6b204-340">iCloud バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="6b204-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="6b204-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="6b204-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-342">Boolean</span></span>|<span data-ttu-id="6b204-343">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="6b204-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="6b204-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="6b204-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-345">Boolean</span></span>|<span data-ttu-id="6b204-346">管理対象アプリのクラウドの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="6b204-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="6b204-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="6b204-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-348">Boolean</span></span>|<span data-ttu-id="6b204-349">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="6b204-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="6b204-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="6b204-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-351">Boolean</span></span>|<span data-ttu-id="6b204-352">iCloud フォトのストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="6b204-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="6b204-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="6b204-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-354">Boolean</span></span>|<span data-ttu-id="6b204-355">共有フォト ストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="6b204-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="6b204-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="6b204-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-357">Boolean</span></span>|<span data-ttu-id="6b204-358">iCloud のバックアップを暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="6b204-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="6b204-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="6b204-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-360">Boolean</span></span>|<span data-ttu-id="6b204-361">ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b204-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="6b204-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="6b204-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="6b204-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-363">Boolean</span></span>|<span data-ttu-id="6b204-364">デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="6b204-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="6b204-365">iTunesBlockRadio</span></span>|<span data-ttu-id="6b204-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-366">Boolean</span></span>|<span data-ttu-id="6b204-367">デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6b204-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="6b204-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="6b204-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-369">Boolean</span></span>|<span data-ttu-id="6b204-370">デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6b204-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="6b204-371">keyboardBlockDictation</span></span>|<span data-ttu-id="6b204-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-372">Boolean</span></span>|<span data-ttu-id="6b204-373">デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="6b204-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="6b204-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-375">Boolean</span></span>|<span data-ttu-id="6b204-376">デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6b204-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="6b204-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="6b204-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-378">Boolean</span></span>|<span data-ttu-id="6b204-379">デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6b204-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="6b204-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="6b204-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-381">Boolean</span></span>|<span data-ttu-id="6b204-382">デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="6b204-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="6b204-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="6b204-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-384">Boolean</span></span>|<span data-ttu-id="6b204-385">キオスク モード時の補助音声を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="6b204-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="6b204-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-387">Boolean</span></span>|<span data-ttu-id="6b204-388">キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="6b204-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="6b204-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-390">Boolean</span></span>|<span data-ttu-id="6b204-391">キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span> <span data-ttu-id="6b204-392">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="6b204-392">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="6b204-393">代わりに KioskModeBlockAutoLock を使用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-393">Use KioskModeBlockAutoLock instead.</span></span>|
|<span data-ttu-id="6b204-394">kioskModeBlockAutoLock</span><span class="sxs-lookup"><span data-stu-id="6b204-394">kioskModeBlockAutoLock</span></span>|<span data-ttu-id="6b204-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-395">Boolean</span></span>|<span data-ttu-id="6b204-396">キオスクモード時にデバイスの自動ロックをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-396">Indicates whether or not to block device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-397">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="6b204-397">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="6b204-398">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-398">Boolean</span></span>|<span data-ttu-id="6b204-399">キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-399">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-400">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="6b204-400">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="6b204-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-401">Boolean</span></span>|<span data-ttu-id="6b204-402">キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-402">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span> <span data-ttu-id="6b204-403">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="6b204-403">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="6b204-404">代わりに KioskModeBlockRingerSwitch を使用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-404">Use KioskModeBlockRingerSwitch instead.</span></span>|
|<span data-ttu-id="6b204-405">kioskModeBlockRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="6b204-405">kioskModeBlockRingerSwitch</span></span>|<span data-ttu-id="6b204-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-406">Boolean</span></span>|<span data-ttu-id="6b204-407">キオスクモード時の着信音スイッチの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-407">Indicates whether or not to block use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-408">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="6b204-408">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="6b204-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-409">Boolean</span></span>|<span data-ttu-id="6b204-410">キオスク モード時の画面の回転を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-410">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span> <span data-ttu-id="6b204-411">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="6b204-411">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="6b204-412">代わりに KioskModeBlockScreenRotation を使用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-412">Use KioskModeBlockScreenRotation instead.</span></span>|
|<span data-ttu-id="6b204-413">kioskModeBlockScreenRotation</span><span class="sxs-lookup"><span data-stu-id="6b204-413">kioskModeBlockScreenRotation</span></span>|<span data-ttu-id="6b204-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-414">Boolean</span></span>|<span data-ttu-id="6b204-415">キオスクモード時の画面の回転を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-415">Indicates whether or not to block screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-416">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="6b204-416">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="6b204-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-417">Boolean</span></span>|<span data-ttu-id="6b204-418">キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-418">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span> <span data-ttu-id="6b204-419">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="6b204-419">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="6b204-420">代わりに KioskModeBlockSleepButton を使用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-420">Use KioskModeBlockSleepButton instead.</span></span>|
|<span data-ttu-id="6b204-421">kioskModeBlockSleepButton</span><span class="sxs-lookup"><span data-stu-id="6b204-421">kioskModeBlockSleepButton</span></span>|<span data-ttu-id="6b204-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-422">Boolean</span></span>|<span data-ttu-id="6b204-423">キオスクモード時のスリープボタンの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-423">Indicates whether or not to block use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-424">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="6b204-424">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="6b204-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-425">Boolean</span></span>|<span data-ttu-id="6b204-426">キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-426">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span> <span data-ttu-id="6b204-427">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="6b204-427">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="6b204-428">代わりに KioskModeBlockTouchscreen を使用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-428">Use KioskModeBlockTouchscreen instead.</span></span>|
|<span data-ttu-id="6b204-429">kioskModeBlockTouchscreen</span><span class="sxs-lookup"><span data-stu-id="6b204-429">kioskModeBlockTouchscreen</span></span>|<span data-ttu-id="6b204-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-430">Boolean</span></span>|<span data-ttu-id="6b204-431">キオスクモード時のタッチスクリーンの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-431">Indicates whether or not to block use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-432">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="6b204-432">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="6b204-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-433">Boolean</span></span>|<span data-ttu-id="6b204-434">キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-434">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-435">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="6b204-435">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="6b204-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-436">Boolean</span></span>|<span data-ttu-id="6b204-437">キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-437">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span> <span data-ttu-id="6b204-438">このプロパティの機能は、OS の既定値と重複しています。非推奨です。</span><span class="sxs-lookup"><span data-stu-id="6b204-438">This property's funcitonality is redundant with the OS default and is deprecated.</span></span> <span data-ttu-id="6b204-439">代わりに KioskModeBlockVolumeButtons を使用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-439">Use KioskModeBlockVolumeButtons instead.</span></span>|
|<span data-ttu-id="6b204-440">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="6b204-440">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="6b204-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-441">Boolean</span></span>|<span data-ttu-id="6b204-442">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-442">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="6b204-443">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="6b204-443">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="6b204-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-444">Boolean</span></span>|<span data-ttu-id="6b204-445">キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-445">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-446">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="6b204-446">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="6b204-447">String</span><span class="sxs-lookup"><span data-stu-id="6b204-447">String</span></span>|<span data-ttu-id="6b204-448">キオスク モード用に使用するアプリへの、App Store 内の URL。</span><span class="sxs-lookup"><span data-stu-id="6b204-448">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="6b204-449">KioskModeManagedAppId が不明な場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-449">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="6b204-450">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="6b204-450">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="6b204-451">String</span><span class="sxs-lookup"><span data-stu-id="6b204-451">String</span></span>|<span data-ttu-id="6b204-452">キオスクモード用に使用する組み込みアプリの ID。</span><span class="sxs-lookup"><span data-stu-id="6b204-452">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="6b204-453">KioskModeManagedAppId および KioskModeAppStoreUrl が設定されていない場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="6b204-453">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="6b204-454">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="6b204-454">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="6b204-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-455">Boolean</span></span>|<span data-ttu-id="6b204-456">キオスク モード時に Assistive Touch が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-456">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-457">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="6b204-457">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="6b204-458">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-458">Boolean</span></span>|<span data-ttu-id="6b204-459">キオスク モード時に色反転が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-459">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-460">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="6b204-460">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="6b204-461">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-461">Boolean</span></span>|<span data-ttu-id="6b204-462">キオスク モード時にモノラル オーディオが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-462">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-463">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="6b204-463">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="6b204-464">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-464">Boolean</span></span>|<span data-ttu-id="6b204-465">キオスク モード時にボイス オーバーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-465">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-466">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="6b204-466">kioskModeRequireZoom</span></span>|<span data-ttu-id="6b204-467">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-467">Boolean</span></span>|<span data-ttu-id="6b204-468">キオスク モード時にズームが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-468">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="6b204-469">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="6b204-469">kioskModeManagedAppId</span></span>|<span data-ttu-id="6b204-470">String</span><span class="sxs-lookup"><span data-stu-id="6b204-470">String</span></span>|<span data-ttu-id="6b204-471">キオスク モード用に使用するアプリの管理対象アプリ ID。</span><span class="sxs-lookup"><span data-stu-id="6b204-471">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="6b204-472">KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。</span><span class="sxs-lookup"><span data-stu-id="6b204-472">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="6b204-473">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="6b204-473">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="6b204-474">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-474">Boolean</span></span>|<span data-ttu-id="6b204-475">ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-475">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="6b204-476">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="6b204-476">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="6b204-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-477">Boolean</span></span>|<span data-ttu-id="6b204-478">ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-478">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="6b204-479">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="6b204-479">lockScreenBlockPassbook</span></span>|<span data-ttu-id="6b204-480">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-480">Boolean</span></span>|<span data-ttu-id="6b204-481">デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-481">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="6b204-482">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="6b204-482">lockScreenBlockTodayView</span></span>|<span data-ttu-id="6b204-483">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-483">Boolean</span></span>|<span data-ttu-id="6b204-484">ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-484">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="6b204-485">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6b204-485">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="6b204-486">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="6b204-486">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="6b204-487">メディア コンテンツの評価の設定 (オーストラリア向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-487">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="6b204-488">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6b204-488">mediaContentRatingCanada</span></span>|[<span data-ttu-id="6b204-489">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="6b204-489">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="6b204-490">メディア コンテンツの評価の設定 (カナダ向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-490">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="6b204-491">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="6b204-491">mediaContentRatingFrance</span></span>|[<span data-ttu-id="6b204-492">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="6b204-492">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="6b204-493">メディア コンテンツの評価の設定 (フランス向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-493">Media content rating settings for France</span></span>|
|<span data-ttu-id="6b204-494">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6b204-494">mediaContentRatingGermany</span></span>|[<span data-ttu-id="6b204-495">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="6b204-495">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="6b204-496">メディア コンテンツの評価の設定 (ドイツ向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-496">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="6b204-497">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="6b204-497">mediaContentRatingIreland</span></span>|[<span data-ttu-id="6b204-498">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="6b204-498">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="6b204-499">メディア コンテンツの評価の設定 (アイルランド向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-499">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="6b204-500">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6b204-500">mediaContentRatingJapan</span></span>|[<span data-ttu-id="6b204-501">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="6b204-501">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="6b204-502">メディア コンテンツの評価の設定 (日本向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-502">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="6b204-503">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6b204-503">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="6b204-504">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="6b204-504">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="6b204-505">メディア コンテンツの評価の設定 (ニュージーランド向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-505">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="6b204-506">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6b204-506">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="6b204-507">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="6b204-507">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="6b204-508">メディア コンテンツの評価の設定 (英国向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-508">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="6b204-509">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6b204-509">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="6b204-510">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="6b204-510">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="6b204-511">メディア コンテンツの評価の設定 (米国向け)</span><span class="sxs-lookup"><span data-stu-id="6b204-511">Media content rating settings for United States</span></span>|
|<span data-ttu-id="6b204-512">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="6b204-512">networkUsageRules</span></span>|<span data-ttu-id="6b204-513">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6b204-513">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="6b204-514">管理対象アプリと、それらに適用されるネットワーク ルールのリストです。</span><span class="sxs-lookup"><span data-stu-id="6b204-514">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="6b204-515">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="6b204-515">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="6b204-516">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="6b204-516">mediaContentRatingApps</span></span>|[<span data-ttu-id="6b204-517">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="6b204-517">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="6b204-518">アプリのメディアコンテンツの評価の設定。</span><span class="sxs-lookup"><span data-stu-id="6b204-518">Media content rating settings for Apps.</span></span> <span data-ttu-id="6b204-519">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="6b204-519">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="6b204-520">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-520">messagesBlocked</span></span>|<span data-ttu-id="6b204-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-521">Boolean</span></span>|<span data-ttu-id="6b204-522">ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-522">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="6b204-523">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="6b204-523">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="6b204-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-524">Boolean</span></span>|<span data-ttu-id="6b204-525">通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-525">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6b204-526">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="6b204-526">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="6b204-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-527">Boolean</span></span>|<span data-ttu-id="6b204-528">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-528">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="6b204-529">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="6b204-529">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="6b204-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-530">Boolean</span></span>|<span data-ttu-id="6b204-531">監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。</span><span class="sxs-lookup"><span data-stu-id="6b204-531">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="6b204-532">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="6b204-532">passcodeBlockModification</span></span>|<span data-ttu-id="6b204-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-533">Boolean</span></span>|<span data-ttu-id="6b204-534">監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-534">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="6b204-535">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="6b204-535">passcodeBlockSimple</span></span>|<span data-ttu-id="6b204-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-536">Boolean</span></span>|<span data-ttu-id="6b204-537">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-537">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="6b204-538">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="6b204-538">passcodeExpirationDays</span></span>|<span data-ttu-id="6b204-539">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-539">Int32</span></span>|<span data-ttu-id="6b204-540">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="6b204-540">Number of days before the passcode expires.</span></span> <span data-ttu-id="6b204-541">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="6b204-541">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="6b204-542">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="6b204-542">passcodeMinimumLength</span></span>|<span data-ttu-id="6b204-543">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-543">Int32</span></span>|<span data-ttu-id="6b204-544">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="6b204-544">Minimum length of passcode.</span></span> <span data-ttu-id="6b204-545">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="6b204-545">Valid values 4 to 14</span></span>|
|<span data-ttu-id="6b204-546">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="6b204-546">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="6b204-547">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-547">Int32</span></span>|<span data-ttu-id="6b204-548">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="6b204-548">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="6b204-549">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="6b204-549">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="6b204-550">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-550">Int32</span></span>|<span data-ttu-id="6b204-551">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="6b204-551">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="6b204-552">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="6b204-552">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="6b204-553">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-553">Int32</span></span>|<span data-ttu-id="6b204-554">パスコードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="6b204-554">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="6b204-555">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="6b204-555">Valid values 0 to 4</span></span>|
|<span data-ttu-id="6b204-556">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="6b204-556">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="6b204-557">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-557">Int32</span></span>|<span data-ttu-id="6b204-558">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="6b204-558">Number of previous passcodes to block.</span></span> <span data-ttu-id="6b204-559">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="6b204-559">Valid values 1 to 24</span></span>|
|<span data-ttu-id="6b204-560">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="6b204-560">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="6b204-561">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-561">Int32</span></span>|<span data-ttu-id="6b204-562">デバイスをワイプするまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="6b204-562">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="6b204-563">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="6b204-563">Valid values 4 to 11</span></span>|
|<span data-ttu-id="6b204-564">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="6b204-564">passcodeRequiredType</span></span>|[<span data-ttu-id="6b204-565">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="6b204-565">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="6b204-566">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="6b204-566">Type of passcode that is required.</span></span> <span data-ttu-id="6b204-567">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="6b204-567">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="6b204-568">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="6b204-568">passcodeRequired</span></span>|<span data-ttu-id="6b204-569">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-569">Boolean</span></span>|<span data-ttu-id="6b204-570">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b204-570">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="6b204-571">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-571">podcastsBlocked</span></span>|<span data-ttu-id="6b204-572">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-572">Boolean</span></span>|<span data-ttu-id="6b204-573">ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-573">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="6b204-574">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="6b204-574">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="6b204-575">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-575">Boolean</span></span>|<span data-ttu-id="6b204-576">監視対象デバイスで近くのデバイスをセットアップするためのプロンプトを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-576">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="6b204-577">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="6b204-577">safariBlockAutofill</span></span>|<span data-ttu-id="6b204-578">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-578">Boolean</span></span>|<span data-ttu-id="6b204-579">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-579">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="6b204-580">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="6b204-580">safariBlockJavaScript</span></span>|<span data-ttu-id="6b204-581">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-581">Boolean</span></span>|<span data-ttu-id="6b204-582">Safari 内で JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-582">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="6b204-583">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="6b204-583">safariBlockPopups</span></span>|<span data-ttu-id="6b204-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-584">Boolean</span></span>|<span data-ttu-id="6b204-585">Safari 内でポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-585">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="6b204-586">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-586">safariBlocked</span></span>|<span data-ttu-id="6b204-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-587">Boolean</span></span>|<span data-ttu-id="6b204-588">ユーザーによる Safari の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-588">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="6b204-589">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="6b204-589">safariCookieSettings</span></span>|[<span data-ttu-id="6b204-590">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="6b204-590">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="6b204-591">Safari の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="6b204-591">Cookie settings for Safari.</span></span> <span data-ttu-id="6b204-592">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="6b204-592">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="6b204-593">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="6b204-593">safariManagedDomains</span></span>|<span data-ttu-id="6b204-594">String collection</span><span class="sxs-lookup"><span data-stu-id="6b204-594">String collection</span></span>|<span data-ttu-id="6b204-595">ここに記載されているパターンに一致する URL は管理対象と見なされます。</span><span class="sxs-lookup"><span data-stu-id="6b204-595">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="6b204-596">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="6b204-596">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="6b204-597">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6b204-597">String collection</span></span>|<span data-ttu-id="6b204-598">ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。</span><span class="sxs-lookup"><span data-stu-id="6b204-598">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="6b204-599">監視モードのデバイスに適用されます (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-599">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="6b204-600">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="6b204-600">safariRequireFraudWarning</span></span>|<span data-ttu-id="6b204-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-601">Boolean</span></span>|<span data-ttu-id="6b204-602">Safari での不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-602">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="6b204-603">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-603">screenCaptureBlocked</span></span>|<span data-ttu-id="6b204-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-604">Boolean</span></span>|<span data-ttu-id="6b204-605">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-605">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="6b204-606">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-606">siriBlocked</span></span>|<span data-ttu-id="6b204-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-607">Boolean</span></span>|<span data-ttu-id="6b204-608">ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-608">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="6b204-609">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="6b204-609">siriBlockedWhenLocked</span></span>|<span data-ttu-id="6b204-610">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-610">Boolean</span></span>|<span data-ttu-id="6b204-611">ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-611">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="6b204-612">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="6b204-612">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="6b204-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-613">Boolean</span></span>|<span data-ttu-id="6b204-614">監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-614">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="6b204-615">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="6b204-615">siriRequireProfanityFilter</span></span>|<span data-ttu-id="6b204-616">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-616">Boolean</span></span>|<span data-ttu-id="6b204-617">Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-617">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="6b204-618">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="6b204-618">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="6b204-619">Int32</span><span class="sxs-lookup"><span data-stu-id="6b204-619">Int32</span></span>|<span data-ttu-id="6b204-620">監視対象デバイスに対してソフトウェア更新プログラムが delyed される日数を設定します。</span><span class="sxs-lookup"><span data-stu-id="6b204-620">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="6b204-621">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="6b204-621">Valid values 0 to 90</span></span>|
|<span data-ttu-id="6b204-622">ソフトウェアの更新 Force延期</span><span class="sxs-lookup"><span data-stu-id="6b204-622">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="6b204-623">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-623">Boolean</span></span>|<span data-ttu-id="6b204-624">デバイスが監視モードのときに、ユーザーのソフトウェア更新プログラムの表示を延期するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-624">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-625">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="6b204-625">spotlightBlockInternetResults</span></span>|<span data-ttu-id="6b204-626">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-626">Boolean</span></span>|<span data-ttu-id="6b204-627">監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-627">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="6b204-628">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-628">voiceDialingBlocked</span></span>|<span data-ttu-id="6b204-629">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-629">Boolean</span></span>|<span data-ttu-id="6b204-630">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-630">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="6b204-631">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="6b204-631">wallpaperBlockModification</span></span>|<span data-ttu-id="6b204-632">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-632">Boolean</span></span>|<span data-ttu-id="6b204-633">監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-633">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="6b204-634">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="6b204-634">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="6b204-635">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-635">Boolean</span></span>|<span data-ttu-id="6b204-636">デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-636">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="6b204-637">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="6b204-637">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="6b204-638">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-638">Boolean</span></span>|<span data-ttu-id="6b204-639">教室経由で管理されていないコースに登録された学生が、コースを離れるときに教師にアクセス許可を要求するかどうかを示します (iOS 11.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-639">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="6b204-640">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="6b204-640">keychainBlockCloudSync</span></span>|<span data-ttu-id="6b204-641">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-641">Boolean</span></span>|<span data-ttu-id="6b204-642">ICloud のキーチェーン同期がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-642">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="6b204-643">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="6b204-643">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="6b204-644">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-644">Boolean</span></span>|<span data-ttu-id="6b204-645">空軍の PKI 更新がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-645">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="6b204-646">この制限を false に設定しても、CRL および OCSP チェック (iOS 7.0 以降) は無効になりません。</span><span class="sxs-lookup"><span data-stu-id="6b204-646">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="6b204-647">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="6b204-647">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="6b204-648">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-648">Boolean</span></span>|<span data-ttu-id="6b204-649">Ad の追跡が制限されているかどうかを示します。(iOS 7.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-649">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="6b204-650">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="6b204-650">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="6b204-651">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-651">Boolean</span></span>|<span data-ttu-id="6b204-652">エンタープライズブックのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-652">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="6b204-653">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="6b204-653">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="6b204-654">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-654">Boolean</span></span>|<span data-ttu-id="6b204-655">エンタープライズブックのメモと強調表示の同期がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-655">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="6b204-656">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-656">airPrintBlocked</span></span>|<span data-ttu-id="6b204-657">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-657">Boolean</span></span>|<span data-ttu-id="6b204-658">放映印刷をブロックするかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-658">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="6b204-659">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="6b204-659">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="6b204-660">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-660">Boolean</span></span>|<span data-ttu-id="6b204-661">放映された印刷に対して、ユーザー名とパスワードのキーチェーンストレージをブロックするかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-661">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="6b204-662">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="6b204-662">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="6b204-663">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-663">Boolean</span></span>|<span data-ttu-id="6b204-664">TLS 印刷通信 (iOS 11.0 以降) に対して信頼できる証明書が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-664">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="6b204-665">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="6b204-665">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="6b204-666">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-666">Boolean</span></span>|<span data-ttu-id="6b204-667">放映された印刷プリンターの iBeacon 検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-667">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="6b204-668">これにより、ネットワークトラフィック (iOS 11.0 以降) では、フィッシングからの Bluetooth ビーコンを誤って印刷することがなくなります。</span><span class="sxs-lookup"><span data-stu-id="6b204-668">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="6b204-669">blockSystemAppRemoval 削除</span><span class="sxs-lookup"><span data-stu-id="6b204-669">blockSystemAppRemoval</span></span>|<span data-ttu-id="6b204-670">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-670">Boolean</span></span>|<span data-ttu-id="6b204-671">デバイスからのシステムアプリの削除が、監視対象デバイスでブロックされているかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-671">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="6b204-672">vpnBlockCreation 作成</span><span class="sxs-lookup"><span data-stu-id="6b204-672">vpnBlockCreation</span></span>|<span data-ttu-id="6b204-673">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-673">Boolean</span></span>|<span data-ttu-id="6b204-674">VPN 構成の作成がブロックされるかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-674">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="6b204-675">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-675">appRemovalBlocked</span></span>|<span data-ttu-id="6b204-676">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-676">Boolean</span></span>|<span data-ttu-id="6b204-677">アプリの削除が許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-677">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="6b204-678">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="6b204-678">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="6b204-679">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-679">Boolean</span></span>|<span data-ttu-id="6b204-680">デバイスがロックされているときに USB アクセサリへの接続が許可されるかどうかを示します (iOS 11.4.1 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-680">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="6b204-681">passwordBlockAutoFill フィル</span><span class="sxs-lookup"><span data-stu-id="6b204-681">passwordBlockAutoFill</span></span>|<span data-ttu-id="6b204-682">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-682">Boolean</span></span>|<span data-ttu-id="6b204-683">パスワードのオートフィル機能が許可されているかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-683">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="6b204-684">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="6b204-684">passwordBlockProximityRequests</span></span>|<span data-ttu-id="6b204-685">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-685">Boolean</span></span>|<span data-ttu-id="6b204-686">近くのデバイスからのパスワードの要求をブロックするかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-686">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="6b204-687">Passwordblockエア Drop共有</span><span class="sxs-lookup"><span data-stu-id="6b204-687">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="6b204-688">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-688">Boolean</span></span>|<span data-ttu-id="6b204-689">通話ドロップパスワード機能 iOS 12.0 以降) でのパスワードの共有を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b204-689">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="6b204-690">dateAndTimeForceSetAutomatically に</span><span class="sxs-lookup"><span data-stu-id="6b204-690">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="6b204-691">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-691">Boolean</span></span>|<span data-ttu-id="6b204-692">ユーザーが日付と時刻を自動的に設定する機能が有効であるかどうか、およびユーザーが無効にすることができないかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-692">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="6b204-693">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="6b204-693">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="6b204-694">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-694">Boolean</span></span>|<span data-ttu-id="6b204-695">管理対象アプリが、管理されていない連絡先アカウントに連絡先を書き込むことができるかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-695">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="6b204-696">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="6b204-696">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="6b204-697">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-697">Boolean</span></span>|<span data-ttu-id="6b204-698">管理対象外アプリが管理された連絡先から読み取ることができるかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-698">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|
|<span data-ttu-id="6b204-699">cellularBlockPersonalHotspotModification</span><span class="sxs-lookup"><span data-stu-id="6b204-699">cellularBlockPersonalHotspotModification</span></span>|<span data-ttu-id="6b204-700">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-700">Boolean</span></span>|<span data-ttu-id="6b204-701">ユーザーが個人用ホットスポットの設定を変更することを禁止するかどうかを示します (iOS 12.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-701">Indicates whether or not to block the user from modifying the personal hotspot setting (iOS 12.2 or later).</span></span>|
|<span data-ttu-id="6b204-702">siriDisableServerLogging</span><span class="sxs-lookup"><span data-stu-id="6b204-702">siriDisableServerLogging</span></span>|<span data-ttu-id="6b204-703">Boolean</span><span class="sxs-lookup"><span data-stu-id="6b204-703">Boolean</span></span>|<span data-ttu-id="6b204-704">サーバー側の Siri ログが無効かどうかを示します (iOS 12.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="6b204-704">Indicates whether or not server-side Siri logging is disabled (iOS 12.2 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="6b204-705">応答</span><span class="sxs-lookup"><span data-stu-id="6b204-705">Response</span></span>
<span data-ttu-id="6b204-706">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6b204-706">If successful, this method returns a `201 Created` response code and a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b204-707">例</span><span class="sxs-lookup"><span data-stu-id="6b204-707">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b204-708">要求</span><span class="sxs-lookup"><span data-stu-id="6b204-708">Request</span></span>
<span data-ttu-id="6b204-709">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b204-709">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 9386

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="6b204-710">応答</span><span class="sxs-lookup"><span data-stu-id="6b204-710">Response</span></span>
<span data-ttu-id="6b204-p139">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6b204-p139">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 9558

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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




