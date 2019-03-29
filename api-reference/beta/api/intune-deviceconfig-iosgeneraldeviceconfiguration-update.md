---
title: Update iosGeneralDeviceConfiguration
description: iosGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f72ae25934e08c228375dbfefc6a243e87792b82
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30974364"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="689c5-103">Update iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="689c5-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="689c5-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="689c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="689c5-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="689c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="689c5-106">[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="689c5-106">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="689c5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="689c5-107">Prerequisites</span></span>
<span data-ttu-id="689c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="689c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="689c5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="689c5-110">Permission type</span></span>|<span data-ttu-id="689c5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="689c5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="689c5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="689c5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="689c5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="689c5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="689c5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="689c5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="689c5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="689c5-115">Not supported.</span></span>|
|<span data-ttu-id="689c5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="689c5-116">Application</span></span>|<span data-ttu-id="689c5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="689c5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="689c5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="689c5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="689c5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="689c5-119">Request headers</span></span>
|<span data-ttu-id="689c5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="689c5-120">Header</span></span>|<span data-ttu-id="689c5-121">値</span><span class="sxs-lookup"><span data-stu-id="689c5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="689c5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="689c5-122">Authorization</span></span>|<span data-ttu-id="689c5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="689c5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="689c5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="689c5-124">Accept</span></span>|<span data-ttu-id="689c5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="689c5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="689c5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="689c5-126">Request body</span></span>
<span data-ttu-id="689c5-127">要求本文で、[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="689c5-127">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="689c5-128">次の表に、[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-128">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="689c5-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="689c5-129">Property</span></span>|<span data-ttu-id="689c5-130">型</span><span class="sxs-lookup"><span data-stu-id="689c5-130">Type</span></span>|<span data-ttu-id="689c5-131">説明</span><span class="sxs-lookup"><span data-stu-id="689c5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="689c5-132">id</span><span class="sxs-lookup"><span data-stu-id="689c5-132">id</span></span>|<span data-ttu-id="689c5-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="689c5-133">String</span></span>|<span data-ttu-id="689c5-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="689c5-134">Key of the entity.</span></span> <span data-ttu-id="689c5-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="689c5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="689c5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="689c5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="689c5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="689c5-137">DateTimeOffset</span></span>|<span data-ttu-id="689c5-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="689c5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="689c5-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="689c5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="689c5-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="689c5-140">roleScopeTagIds</span></span>|<span data-ttu-id="689c5-141">String collection</span><span class="sxs-lookup"><span data-stu-id="689c5-141">String collection</span></span>|<span data-ttu-id="689c5-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="689c5-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="689c5-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="689c5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="689c5-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="689c5-144">supportsScopeTags</span></span>|<span data-ttu-id="689c5-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-145">Boolean</span></span>|<span data-ttu-id="689c5-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="689c5-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="689c5-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="689c5-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="689c5-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="689c5-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="689c5-149">This property is read-only.</span></span> <span data-ttu-id="689c5-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="689c5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="689c5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="689c5-151">createdDateTime</span></span>|<span data-ttu-id="689c5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="689c5-152">DateTimeOffset</span></span>|<span data-ttu-id="689c5-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="689c5-153">DateTime the object was created.</span></span> <span data-ttu-id="689c5-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="689c5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="689c5-155">description</span><span class="sxs-lookup"><span data-stu-id="689c5-155">description</span></span>|<span data-ttu-id="689c5-156">String</span><span class="sxs-lookup"><span data-stu-id="689c5-156">String</span></span>|<span data-ttu-id="689c5-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="689c5-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="689c5-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="689c5-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="689c5-159">displayName</span><span class="sxs-lookup"><span data-stu-id="689c5-159">displayName</span></span>|<span data-ttu-id="689c5-160">String</span><span class="sxs-lookup"><span data-stu-id="689c5-160">String</span></span>|<span data-ttu-id="689c5-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="689c5-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="689c5-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="689c5-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="689c5-163">version</span><span class="sxs-lookup"><span data-stu-id="689c5-163">version</span></span>|<span data-ttu-id="689c5-164">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-164">Int32</span></span>|<span data-ttu-id="689c5-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="689c5-165">Version of the device configuration.</span></span> <span data-ttu-id="689c5-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="689c5-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="689c5-167">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="689c5-167">accountBlockModification</span></span>|<span data-ttu-id="689c5-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-168">Boolean</span></span>|<span data-ttu-id="689c5-169">デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-169">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-170">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="689c5-170">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="689c5-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-171">Boolean</span></span>|<span data-ttu-id="689c5-172">デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-172">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="689c5-173">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-173">airDropBlocked</span></span>|<span data-ttu-id="689c5-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-174">Boolean</span></span>|<span data-ttu-id="689c5-175">デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-175">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-176">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="689c5-176">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="689c5-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-177">Boolean</span></span>|<span data-ttu-id="689c5-178">AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-178">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="689c5-179">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="689c5-179">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="689c5-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-180">Boolean</span></span>|<span data-ttu-id="689c5-181">ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-181">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="689c5-182">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="689c5-182">appleWatchBlockPairing</span></span>|<span data-ttu-id="689c5-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-183">Boolean</span></span>|<span data-ttu-id="689c5-184">デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-184">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="689c5-185">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="689c5-185">appleWatchForceWristDetection</span></span>|<span data-ttu-id="689c5-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-186">Boolean</span></span>|<span data-ttu-id="689c5-187">ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-187">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="689c5-188">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-188">appleNewsBlocked</span></span>|<span data-ttu-id="689c5-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-189">Boolean</span></span>|<span data-ttu-id="689c5-190">デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-190">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="689c5-191">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="689c5-191">appsSingleAppModeList</span></span>|<span data-ttu-id="689c5-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="689c5-192">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="689c5-193">単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="689c5-193">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="689c5-194">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="689c5-194">Supervised only.</span></span> <span data-ttu-id="689c5-195">iOS 7.0 以降。</span><span class="sxs-lookup"><span data-stu-id="689c5-195">iOS 7.0 and later.</span></span> <span data-ttu-id="689c5-196">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="689c5-196">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="689c5-197">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="689c5-197">appsVisibilityList</span></span>|<span data-ttu-id="689c5-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="689c5-198">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="689c5-199">可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。</span><span class="sxs-lookup"><span data-stu-id="689c5-199">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="689c5-200">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="689c5-200">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="689c5-201">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="689c5-201">appsVisibilityListType</span></span>|[<span data-ttu-id="689c5-202">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="689c5-202">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="689c5-203">AppsVisibilityList 内にあるリストの種類です。</span><span class="sxs-lookup"><span data-stu-id="689c5-203">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="689c5-204">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="689c5-204">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="689c5-205">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="689c5-205">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="689c5-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-206">Boolean</span></span>|<span data-ttu-id="689c5-207">デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-207">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="689c5-208">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-208">appStoreBlocked</span></span>|<span data-ttu-id="689c5-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-209">Boolean</span></span>|<span data-ttu-id="689c5-210">ユーザーによる App Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-210">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="689c5-211">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="689c5-211">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="689c5-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-212">Boolean</span></span>|<span data-ttu-id="689c5-213">ユーザーによるアプリの購入を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-213">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="689c5-214">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="689c5-214">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="689c5-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-215">Boolean</span></span>|<span data-ttu-id="689c5-216">ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-216">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="689c5-217">監視モードのみに適用されます (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-217">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="689c5-218">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="689c5-218">appStoreRequirePassword</span></span>|<span data-ttu-id="689c5-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-219">Boolean</span></span>|<span data-ttu-id="689c5-220">App Store 使用時に、パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="689c5-220">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="689c5-221">autofillforceauthentication</span><span class="sxs-lookup"><span data-stu-id="689c5-221">autoFillForceAuthentication</span></span>|<span data-ttu-id="689c5-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-222">Boolean</span></span>|<span data-ttu-id="689c5-223">Safari や、監視対象デバイスの他のアプリで、パスワードとクレジットカード情報を自動入力する前に、ユーザー認証を強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-223">Indicates whether or not to force user authentication before autofilling passwords and credit card information in Safari and other apps on supervised devices.</span></span>|
|<span data-ttu-id="689c5-224">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="689c5-224">bluetoothBlockModification</span></span>|<span data-ttu-id="689c5-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-225">Boolean</span></span>|<span data-ttu-id="689c5-226">デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-226">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="689c5-227">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-227">cameraBlocked</span></span>|<span data-ttu-id="689c5-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-228">Boolean</span></span>|<span data-ttu-id="689c5-229">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-229">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="689c5-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="689c5-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="689c5-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-231">Boolean</span></span>|<span data-ttu-id="689c5-232">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="689c5-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="689c5-233">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="689c5-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-234">Boolean</span></span>|<span data-ttu-id="689c5-235">ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-235">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="689c5-236">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="689c5-236">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="689c5-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-237">Boolean</span></span>|<span data-ttu-id="689c5-238">デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-238">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-239">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="689c5-239">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="689c5-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-240">Boolean</span></span>|<span data-ttu-id="689c5-241">個人用ホットスポットをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-241">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="689c5-242">cellularblockplan の変更</span><span class="sxs-lookup"><span data-stu-id="689c5-242">cellularBlockPlanModification</span></span>|<span data-ttu-id="689c5-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-243">Boolean</span></span>|<span data-ttu-id="689c5-244">ユーザーが、監視対象デバイスの携帯電話プランの設定を変更することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-244">Indicates whether or not to allow users to change the settings of the cellular plan on a supervised device.</span></span>|
|<span data-ttu-id="689c5-245">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="689c5-245">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="689c5-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-246">Boolean</span></span>|<span data-ttu-id="689c5-247">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-247">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="689c5-248">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="689c5-248">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="689c5-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-249">Boolean</span></span>|<span data-ttu-id="689c5-250">信頼されていない TLS の証明書をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-250">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="689c5-251">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="689c5-251">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="689c5-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-252">Boolean</span></span>|<span data-ttu-id="689c5-253">デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-253">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="689c5-254">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="689c5-254">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="689c5-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-255">Boolean</span></span>|<span data-ttu-id="689c5-256">デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-256">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-257">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="689c5-257">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="689c5-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-258">Boolean</span></span>|<span data-ttu-id="689c5-259">デバイスが監視モードのときに、学生に確認せずに教師の要求に対して自動的にアクセス許可を付与するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-259">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student, when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-260">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="689c5-260">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="689c5-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-261">Boolean</span></span>|<span data-ttu-id="689c5-262">学生にメッセージを表示せずに、アプリまたはデバイスのロックを教師に許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-262">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="689c5-263">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="689c5-263">Supervised only.</span></span>|
|<span data-ttu-id="689c5-264">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="689c5-264">compliantAppsList</span></span>|<span data-ttu-id="689c5-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="689c5-265">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="689c5-266">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="689c5-266">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="689c5-267">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="689c5-267">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="689c5-268">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="689c5-268">compliantAppListType</span></span>|[<span data-ttu-id="689c5-269">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="689c5-269">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="689c5-270">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="689c5-270">List that is in the AppComplianceList.</span></span> <span data-ttu-id="689c5-271">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="689c5-271">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="689c5-272">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="689c5-272">configurationProfileBlockChanges</span></span>|<span data-ttu-id="689c5-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-273">Boolean</span></span>|<span data-ttu-id="689c5-274">デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-274">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-275">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-275">definitionLookupBlocked</span></span>|<span data-ttu-id="689c5-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-276">Boolean</span></span>|<span data-ttu-id="689c5-277">デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-277">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="689c5-278">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="689c5-278">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="689c5-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-279">Boolean</span></span>|<span data-ttu-id="689c5-280">デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-280">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-281">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="689c5-281">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="689c5-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-282">Boolean</span></span>|<span data-ttu-id="689c5-283">デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-283">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-284">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="689c5-284">deviceBlockNameModification</span></span>|<span data-ttu-id="689c5-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-285">Boolean</span></span>|<span data-ttu-id="689c5-286">デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-286">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="689c5-287">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="689c5-287">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="689c5-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-288">Boolean</span></span>|<span data-ttu-id="689c5-289">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-289">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="689c5-290">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="689c5-290">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="689c5-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-291">Boolean</span></span>|<span data-ttu-id="689c5-292">デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-292">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="689c5-293">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="689c5-293">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="689c5-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-294">Boolean</span></span>|<span data-ttu-id="689c5-295">ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-295">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="689c5-296">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="689c5-296">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="689c5-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-297">Boolean</span></span>|<span data-ttu-id="689c5-298">ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-298">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="689c5-299">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="689c5-299">emailInDomainSuffixes</span></span>|<span data-ttu-id="689c5-300">String コレクション</span><span class="sxs-lookup"><span data-stu-id="689c5-300">String collection</span></span>|<span data-ttu-id="689c5-301">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="689c5-301">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="689c5-302">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="689c5-302">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="689c5-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-303">Boolean</span></span>|<span data-ttu-id="689c5-304">ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-304">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="689c5-305">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="689c5-305">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="689c5-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-306">Boolean</span></span>|<span data-ttu-id="689c5-307">ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-307">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="689c5-308">esimblockmodification</span><span class="sxs-lookup"><span data-stu-id="689c5-308">esimBlockModification</span></span>|<span data-ttu-id="689c5-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-309">Boolean</span></span>|<span data-ttu-id="689c5-310">監視対象デバイスの eSIM での携帯電話プランの追加または削除を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-310">Indicates whether or not to allow the addition or removal of cellular plans on the eSIM of a supervised device.</span></span>|
|<span data-ttu-id="689c5-311">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-311">faceTimeBlocked</span></span>|<span data-ttu-id="689c5-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-312">Boolean</span></span>|<span data-ttu-id="689c5-313">ユーザーによる FaceTime の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-313">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="689c5-314">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-314">findMyFriendsBlocked</span></span>|<span data-ttu-id="689c5-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-315">Boolean</span></span>|<span data-ttu-id="689c5-316">デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-316">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-317">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="689c5-317">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="689c5-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-318">Boolean</span></span>|<span data-ttu-id="689c5-319">ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-319">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="689c5-320">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="689c5-320">gamingBlockMultiplayer</span></span>|<span data-ttu-id="689c5-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-321">Boolean</span></span>|<span data-ttu-id="689c5-322">ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-322">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="689c5-323">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-323">gameCenterBlocked</span></span>|<span data-ttu-id="689c5-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-324">Boolean</span></span>|<span data-ttu-id="689c5-325">デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-325">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-326">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-326">hostPairingBlocked</span></span>|<span data-ttu-id="689c5-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-327">Boolean</span></span>|<span data-ttu-id="689c5-328">iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-328">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-329">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-329">iBooksStoreBlocked</span></span>|<span data-ttu-id="689c5-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-330">Boolean</span></span>|<span data-ttu-id="689c5-331">デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-331">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-332">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="689c5-332">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="689c5-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-333">Boolean</span></span>|<span data-ttu-id="689c5-334">アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-334">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="689c5-335">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="689c5-335">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="689c5-336">ブール型</span><span class="sxs-lookup"><span data-stu-id="689c5-336">Boolean</span></span>|<span data-ttu-id="689c5-337">ユーザーが ios デバイスで開始された作業を別の ios デバイスまたは macOS デバイスに継続して実行することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-337">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="689c5-338">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="689c5-338">iCloudBlockBackup</span></span>|<span data-ttu-id="689c5-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-339">Boolean</span></span>|<span data-ttu-id="689c5-340">iCloud バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-340">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="689c5-341">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="689c5-341">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="689c5-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-342">Boolean</span></span>|<span data-ttu-id="689c5-343">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-343">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="689c5-344">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="689c5-344">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="689c5-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-345">Boolean</span></span>|<span data-ttu-id="689c5-346">管理対象アプリのクラウドの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-346">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="689c5-347">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="689c5-347">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="689c5-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-348">Boolean</span></span>|<span data-ttu-id="689c5-349">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-349">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="689c5-350">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="689c5-350">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="689c5-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-351">Boolean</span></span>|<span data-ttu-id="689c5-352">iCloud フォトのストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-352">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="689c5-353">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="689c5-353">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="689c5-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-354">Boolean</span></span>|<span data-ttu-id="689c5-355">共有フォト ストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-355">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="689c5-356">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="689c5-356">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="689c5-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-357">Boolean</span></span>|<span data-ttu-id="689c5-358">iCloud のバックアップを暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-358">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="689c5-359">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="689c5-359">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="689c5-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-360">Boolean</span></span>|<span data-ttu-id="689c5-361">ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="689c5-361">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="689c5-362">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="689c5-362">iTunesBlockMusicService</span></span>|<span data-ttu-id="689c5-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-363">Boolean</span></span>|<span data-ttu-id="689c5-364">デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-364">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="689c5-365">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="689c5-365">iTunesBlockRadio</span></span>|<span data-ttu-id="689c5-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-366">Boolean</span></span>|<span data-ttu-id="689c5-367">デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-367">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="689c5-368">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="689c5-368">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="689c5-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-369">Boolean</span></span>|<span data-ttu-id="689c5-370">デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-370">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="689c5-371">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="689c5-371">keyboardBlockDictation</span></span>|<span data-ttu-id="689c5-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-372">Boolean</span></span>|<span data-ttu-id="689c5-373">デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-373">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-374">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="689c5-374">keyboardBlockPredictive</span></span>|<span data-ttu-id="689c5-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-375">Boolean</span></span>|<span data-ttu-id="689c5-376">デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-376">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="689c5-377">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="689c5-377">keyboardBlockShortcuts</span></span>|<span data-ttu-id="689c5-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-378">Boolean</span></span>|<span data-ttu-id="689c5-379">デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-379">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="689c5-380">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="689c5-380">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="689c5-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-381">Boolean</span></span>|<span data-ttu-id="689c5-382">デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-382">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="689c5-383">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="689c5-383">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="689c5-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-384">Boolean</span></span>|<span data-ttu-id="689c5-385">キオスク モード時の補助音声を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-385">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-386">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="689c5-386">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="689c5-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-387">Boolean</span></span>|<span data-ttu-id="689c5-388">キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-388">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-389">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="689c5-389">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="689c5-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-390">Boolean</span></span>|<span data-ttu-id="689c5-391">キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-391">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-392">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="689c5-392">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="689c5-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-393">Boolean</span></span>|<span data-ttu-id="689c5-394">キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-394">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-395">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="689c5-395">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="689c5-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-396">Boolean</span></span>|<span data-ttu-id="689c5-397">キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-397">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-398">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="689c5-398">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="689c5-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-399">Boolean</span></span>|<span data-ttu-id="689c5-400">キオスク モード時の画面の回転を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-400">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-401">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="689c5-401">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="689c5-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-402">Boolean</span></span>|<span data-ttu-id="689c5-403">キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-403">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-404">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="689c5-404">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="689c5-405">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-405">Boolean</span></span>|<span data-ttu-id="689c5-406">キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-406">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-407">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="689c5-407">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="689c5-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-408">Boolean</span></span>|<span data-ttu-id="689c5-409">キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-409">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-410">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="689c5-410">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="689c5-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-411">Boolean</span></span>|<span data-ttu-id="689c5-412">キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-412">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-413">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="689c5-413">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="689c5-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-414">Boolean</span></span>|<span data-ttu-id="689c5-415">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-415">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="689c5-416">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="689c5-416">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="689c5-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-417">Boolean</span></span>|<span data-ttu-id="689c5-418">キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-418">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-419">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="689c5-419">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="689c5-420">String</span><span class="sxs-lookup"><span data-stu-id="689c5-420">String</span></span>|<span data-ttu-id="689c5-421">キオスク モード用に使用するアプリへの、App Store 内の URL。</span><span class="sxs-lookup"><span data-stu-id="689c5-421">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="689c5-422">KioskModeManagedAppId が不明な場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="689c5-422">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="689c5-423">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="689c5-423">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="689c5-424">String</span><span class="sxs-lookup"><span data-stu-id="689c5-424">String</span></span>|<span data-ttu-id="689c5-425">キオスクモード用に使用する組み込みアプリの ID。</span><span class="sxs-lookup"><span data-stu-id="689c5-425">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="689c5-426">KioskModeManagedAppId および KioskModeAppStoreUrl が設定されていない場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="689c5-426">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="689c5-427">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="689c5-427">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="689c5-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-428">Boolean</span></span>|<span data-ttu-id="689c5-429">キオスク モード時に Assistive Touch が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-429">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-430">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="689c5-430">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="689c5-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-431">Boolean</span></span>|<span data-ttu-id="689c5-432">キオスク モード時に色反転が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-432">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-433">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="689c5-433">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="689c5-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-434">Boolean</span></span>|<span data-ttu-id="689c5-435">キオスク モード時にモノラル オーディオが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-435">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-436">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="689c5-436">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="689c5-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-437">Boolean</span></span>|<span data-ttu-id="689c5-438">キオスク モード時にボイス オーバーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-438">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-439">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="689c5-439">kioskModeRequireZoom</span></span>|<span data-ttu-id="689c5-440">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-440">Boolean</span></span>|<span data-ttu-id="689c5-441">キオスク モード時にズームが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-441">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="689c5-442">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="689c5-442">kioskModeManagedAppId</span></span>|<span data-ttu-id="689c5-443">String</span><span class="sxs-lookup"><span data-stu-id="689c5-443">String</span></span>|<span data-ttu-id="689c5-444">キオスク モード用に使用するアプリの管理対象アプリ ID。</span><span class="sxs-lookup"><span data-stu-id="689c5-444">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="689c5-445">KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。</span><span class="sxs-lookup"><span data-stu-id="689c5-445">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="689c5-446">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="689c5-446">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="689c5-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-447">Boolean</span></span>|<span data-ttu-id="689c5-448">ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-448">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="689c5-449">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="689c5-449">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="689c5-450">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-450">Boolean</span></span>|<span data-ttu-id="689c5-451">ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-451">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="689c5-452">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="689c5-452">lockScreenBlockPassbook</span></span>|<span data-ttu-id="689c5-453">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-453">Boolean</span></span>|<span data-ttu-id="689c5-454">デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-454">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="689c5-455">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="689c5-455">lockScreenBlockTodayView</span></span>|<span data-ttu-id="689c5-456">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-456">Boolean</span></span>|<span data-ttu-id="689c5-457">ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-457">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="689c5-458">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="689c5-458">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="689c5-459">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="689c5-459">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="689c5-460">メディア コンテンツの評価の設定 (オーストラリア向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-460">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="689c5-461">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="689c5-461">mediaContentRatingCanada</span></span>|[<span data-ttu-id="689c5-462">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="689c5-462">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="689c5-463">メディア コンテンツの評価の設定 (カナダ向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-463">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="689c5-464">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="689c5-464">mediaContentRatingFrance</span></span>|[<span data-ttu-id="689c5-465">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="689c5-465">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="689c5-466">メディア コンテンツの評価の設定 (フランス向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-466">Media content rating settings for France</span></span>|
|<span data-ttu-id="689c5-467">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="689c5-467">mediaContentRatingGermany</span></span>|[<span data-ttu-id="689c5-468">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="689c5-468">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="689c5-469">メディア コンテンツの評価の設定 (ドイツ向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-469">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="689c5-470">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="689c5-470">mediaContentRatingIreland</span></span>|[<span data-ttu-id="689c5-471">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="689c5-471">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="689c5-472">メディア コンテンツの評価の設定 (アイルランド向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-472">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="689c5-473">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="689c5-473">mediaContentRatingJapan</span></span>|[<span data-ttu-id="689c5-474">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="689c5-474">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="689c5-475">メディア コンテンツの評価の設定 (日本向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-475">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="689c5-476">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="689c5-476">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="689c5-477">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="689c5-477">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="689c5-478">メディア コンテンツの評価の設定 (ニュージーランド向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-478">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="689c5-479">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="689c5-479">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="689c5-480">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="689c5-480">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="689c5-481">メディア コンテンツの評価の設定 (英国向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-481">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="689c5-482">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="689c5-482">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="689c5-483">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="689c5-483">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="689c5-484">メディア コンテンツの評価の設定 (米国向け)</span><span class="sxs-lookup"><span data-stu-id="689c5-484">Media content rating settings for United States</span></span>|
|<span data-ttu-id="689c5-485">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="689c5-485">networkUsageRules</span></span>|<span data-ttu-id="689c5-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="689c5-486">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="689c5-487">管理対象アプリと、それらに適用されるネットワーク ルールのリストです。</span><span class="sxs-lookup"><span data-stu-id="689c5-487">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="689c5-488">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="689c5-488">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="689c5-489">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="689c5-489">mediaContentRatingApps</span></span>|[<span data-ttu-id="689c5-490">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="689c5-490">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="689c5-491">アプリのメディアコンテンツの評価の設定。</span><span class="sxs-lookup"><span data-stu-id="689c5-491">Media content rating settings for Apps.</span></span> <span data-ttu-id="689c5-492">可能な値は `allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17` です。</span><span class="sxs-lookup"><span data-stu-id="689c5-492">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="689c5-493">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-493">messagesBlocked</span></span>|<span data-ttu-id="689c5-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-494">Boolean</span></span>|<span data-ttu-id="689c5-495">ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-495">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="689c5-496">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="689c5-496">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="689c5-497">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-497">Boolean</span></span>|<span data-ttu-id="689c5-498">通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-498">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="689c5-499">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="689c5-499">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="689c5-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-500">Boolean</span></span>|<span data-ttu-id="689c5-501">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-501">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="689c5-502">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="689c5-502">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="689c5-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-503">Boolean</span></span>|<span data-ttu-id="689c5-504">監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。</span><span class="sxs-lookup"><span data-stu-id="689c5-504">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="689c5-505">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="689c5-505">passcodeBlockModification</span></span>|<span data-ttu-id="689c5-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-506">Boolean</span></span>|<span data-ttu-id="689c5-507">監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-507">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="689c5-508">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="689c5-508">passcodeBlockSimple</span></span>|<span data-ttu-id="689c5-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-509">Boolean</span></span>|<span data-ttu-id="689c5-510">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-510">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="689c5-511">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="689c5-511">passcodeExpirationDays</span></span>|<span data-ttu-id="689c5-512">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-512">Int32</span></span>|<span data-ttu-id="689c5-513">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="689c5-513">Number of days before the passcode expires.</span></span> <span data-ttu-id="689c5-514">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="689c5-514">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="689c5-515">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="689c5-515">passcodeMinimumLength</span></span>|<span data-ttu-id="689c5-516">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-516">Int32</span></span>|<span data-ttu-id="689c5-517">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="689c5-517">Minimum length of passcode.</span></span> <span data-ttu-id="689c5-518">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="689c5-518">Valid values 4 to 14</span></span>|
|<span data-ttu-id="689c5-519">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="689c5-519">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="689c5-520">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-520">Int32</span></span>|<span data-ttu-id="689c5-521">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="689c5-521">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="689c5-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="689c5-522">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="689c5-523">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-523">Int32</span></span>|<span data-ttu-id="689c5-524">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="689c5-524">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="689c5-525">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="689c5-525">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="689c5-526">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-526">Int32</span></span>|<span data-ttu-id="689c5-527">パスコードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="689c5-527">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="689c5-528">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="689c5-528">Valid values 0 to 4</span></span>|
|<span data-ttu-id="689c5-529">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="689c5-529">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="689c5-530">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-530">Int32</span></span>|<span data-ttu-id="689c5-531">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="689c5-531">Number of previous passcodes to block.</span></span> <span data-ttu-id="689c5-532">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="689c5-532">Valid values 1 to 24</span></span>|
|<span data-ttu-id="689c5-533">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="689c5-533">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="689c5-534">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-534">Int32</span></span>|<span data-ttu-id="689c5-535">デバイスをワイプするまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="689c5-535">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="689c5-536">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="689c5-536">Valid values 4 to 11</span></span>|
|<span data-ttu-id="689c5-537">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="689c5-537">passcodeRequiredType</span></span>|[<span data-ttu-id="689c5-538">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="689c5-538">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="689c5-539">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="689c5-539">Type of passcode that is required.</span></span> <span data-ttu-id="689c5-540">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="689c5-540">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="689c5-541">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="689c5-541">passcodeRequired</span></span>|<span data-ttu-id="689c5-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-542">Boolean</span></span>|<span data-ttu-id="689c5-543">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="689c5-543">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="689c5-544">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-544">podcastsBlocked</span></span>|<span data-ttu-id="689c5-545">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-545">Boolean</span></span>|<span data-ttu-id="689c5-546">ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-546">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="689c5-547">proximityBlockSetupToNewDevice</span><span class="sxs-lookup"><span data-stu-id="689c5-547">proximityBlockSetupToNewDevice</span></span>|<span data-ttu-id="689c5-548">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-548">Boolean</span></span>|<span data-ttu-id="689c5-549">監視対象デバイスで近くのデバイスをセットアップするためのプロンプトを有効にするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-549">Indicates whether or not to enable the prompt to setup nearby devices with a supervised device.</span></span>|
|<span data-ttu-id="689c5-550">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="689c5-550">safariBlockAutofill</span></span>|<span data-ttu-id="689c5-551">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-551">Boolean</span></span>|<span data-ttu-id="689c5-552">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-552">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="689c5-553">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="689c5-553">safariBlockJavaScript</span></span>|<span data-ttu-id="689c5-554">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-554">Boolean</span></span>|<span data-ttu-id="689c5-555">Safari 内で JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-555">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="689c5-556">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="689c5-556">safariBlockPopups</span></span>|<span data-ttu-id="689c5-557">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-557">Boolean</span></span>|<span data-ttu-id="689c5-558">Safari 内でポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-558">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="689c5-559">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-559">safariBlocked</span></span>|<span data-ttu-id="689c5-560">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-560">Boolean</span></span>|<span data-ttu-id="689c5-561">ユーザーによる Safari の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-561">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="689c5-562">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="689c5-562">safariCookieSettings</span></span>|[<span data-ttu-id="689c5-563">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="689c5-563">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="689c5-564">Safari の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="689c5-564">Cookie settings for Safari.</span></span> <span data-ttu-id="689c5-565">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="689c5-565">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="689c5-566">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="689c5-566">safariManagedDomains</span></span>|<span data-ttu-id="689c5-567">String collection</span><span class="sxs-lookup"><span data-stu-id="689c5-567">String collection</span></span>|<span data-ttu-id="689c5-568">ここに記載されているパターンに一致する URL は管理対象と見なされます。</span><span class="sxs-lookup"><span data-stu-id="689c5-568">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="689c5-569">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="689c5-569">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="689c5-570">String コレクション</span><span class="sxs-lookup"><span data-stu-id="689c5-570">String collection</span></span>|<span data-ttu-id="689c5-571">ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。</span><span class="sxs-lookup"><span data-stu-id="689c5-571">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="689c5-572">監視モードのデバイスに適用されます (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-572">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="689c5-573">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="689c5-573">safariRequireFraudWarning</span></span>|<span data-ttu-id="689c5-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-574">Boolean</span></span>|<span data-ttu-id="689c5-575">Safari での不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-575">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="689c5-576">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-576">screenCaptureBlocked</span></span>|<span data-ttu-id="689c5-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-577">Boolean</span></span>|<span data-ttu-id="689c5-578">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-578">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="689c5-579">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-579">siriBlocked</span></span>|<span data-ttu-id="689c5-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-580">Boolean</span></span>|<span data-ttu-id="689c5-581">ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-581">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="689c5-582">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="689c5-582">siriBlockedWhenLocked</span></span>|<span data-ttu-id="689c5-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-583">Boolean</span></span>|<span data-ttu-id="689c5-584">ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-584">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="689c5-585">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="689c5-585">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="689c5-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-586">Boolean</span></span>|<span data-ttu-id="689c5-587">監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-587">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="689c5-588">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="689c5-588">siriRequireProfanityFilter</span></span>|<span data-ttu-id="689c5-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-589">Boolean</span></span>|<span data-ttu-id="689c5-590">Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-590">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="689c5-591">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="689c5-591">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="689c5-592">Int32</span><span class="sxs-lookup"><span data-stu-id="689c5-592">Int32</span></span>|<span data-ttu-id="689c5-593">監視対象デバイスに対してソフトウェア更新プログラムが delyed される日数を設定します。</span><span class="sxs-lookup"><span data-stu-id="689c5-593">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="689c5-594">有効な値は 0 から 90 までです</span><span class="sxs-lookup"><span data-stu-id="689c5-594">Valid values 0 to 90</span></span>|
|<span data-ttu-id="689c5-595">ソフトウェアの更新 force延期</span><span class="sxs-lookup"><span data-stu-id="689c5-595">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="689c5-596">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-596">Boolean</span></span>|<span data-ttu-id="689c5-597">デバイスが監視モードのときに、ユーザーのソフトウェア更新プログラムの表示を延期するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-597">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-598">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="689c5-598">spotlightBlockInternetResults</span></span>|<span data-ttu-id="689c5-599">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-599">Boolean</span></span>|<span data-ttu-id="689c5-600">監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-600">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="689c5-601">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-601">voiceDialingBlocked</span></span>|<span data-ttu-id="689c5-602">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-602">Boolean</span></span>|<span data-ttu-id="689c5-603">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-603">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="689c5-604">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="689c5-604">wallpaperBlockModification</span></span>|<span data-ttu-id="689c5-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-605">Boolean</span></span>|<span data-ttu-id="689c5-606">監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-606">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="689c5-607">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="689c5-607">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="689c5-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-608">Boolean</span></span>|<span data-ttu-id="689c5-609">デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-609">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="689c5-610">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="689c5-610">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="689c5-611">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-611">Boolean</span></span>|<span data-ttu-id="689c5-612">教室経由で管理されていないコースに登録された学生が、コースを離れるときに教師にアクセス許可を要求するかどうかを示します (iOS 11.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-612">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="689c5-613">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="689c5-613">keychainBlockCloudSync</span></span>|<span data-ttu-id="689c5-614">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-614">Boolean</span></span>|<span data-ttu-id="689c5-615">iCloud のキーチェーン同期がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-615">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="689c5-616">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="689c5-616">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="689c5-617">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-617">Boolean</span></span>|<span data-ttu-id="689c5-618">空軍の PKI 更新がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-618">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="689c5-619">この制限を false に設定しても、CRL および OCSP チェック (iOS 7.0 以降) は無効になりません。</span><span class="sxs-lookup"><span data-stu-id="689c5-619">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="689c5-620">privacyforcelimitadtracking</span><span class="sxs-lookup"><span data-stu-id="689c5-620">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="689c5-621">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-621">Boolean</span></span>|<span data-ttu-id="689c5-622">ad の追跡が制限されているかどうかを示します。(iOS 7.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-622">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="689c5-623">enterprisebookblockbackup</span><span class="sxs-lookup"><span data-stu-id="689c5-623">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="689c5-624">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-624">Boolean</span></span>|<span data-ttu-id="689c5-625">エンタープライズブックのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-625">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="689c5-626">enterprisebookblockmetadatasync</span><span class="sxs-lookup"><span data-stu-id="689c5-626">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="689c5-627">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-627">Boolean</span></span>|<span data-ttu-id="689c5-628">エンタープライズブックのメモと強調表示の同期がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-628">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="689c5-629">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-629">airPrintBlocked</span></span>|<span data-ttu-id="689c5-630">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-630">Boolean</span></span>|<span data-ttu-id="689c5-631">放映印刷をブロックするかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-631">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="689c5-632">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="689c5-632">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="689c5-633">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-633">Boolean</span></span>|<span data-ttu-id="689c5-634">放映された印刷に対して、ユーザー名とパスワードのキーチェーンストレージをブロックするかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-634">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="689c5-635">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="689c5-635">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="689c5-636">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-636">Boolean</span></span>|<span data-ttu-id="689c5-637">TLS 印刷通信 (iOS 11.0 以降) に対して信頼できる証明書が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-637">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="689c5-638">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="689c5-638">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="689c5-639">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-639">Boolean</span></span>|<span data-ttu-id="689c5-640">放映された印刷プリンターの ibeacon 検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-640">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="689c5-641">これにより、ネットワークトラフィック (iOS 11.0 以降) では、フィッシングからの Bluetooth ビーコンを誤って印刷することがなくなります。</span><span class="sxs-lookup"><span data-stu-id="689c5-641">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="689c5-642">blocksystemappremoval 削除</span><span class="sxs-lookup"><span data-stu-id="689c5-642">blockSystemAppRemoval</span></span>|<span data-ttu-id="689c5-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-643">Boolean</span></span>|<span data-ttu-id="689c5-644">デバイスからのシステムアプリの削除が、監視対象デバイスでブロックされているかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-644">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="689c5-645">vpnblockcreation 作成</span><span class="sxs-lookup"><span data-stu-id="689c5-645">vpnBlockCreation</span></span>|<span data-ttu-id="689c5-646">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-646">Boolean</span></span>|<span data-ttu-id="689c5-647">VPN 構成の作成がブロックされるかどうかを示します (iOS 11.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-647">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="689c5-648">appRemovalBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-648">appRemovalBlocked</span></span>|<span data-ttu-id="689c5-649">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-649">Boolean</span></span>|<span data-ttu-id="689c5-650">アプリの削除が許可されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-650">Indicates if the removal of apps is allowed.</span></span>|
|<span data-ttu-id="689c5-651">usbRestrictedModeBlocked</span><span class="sxs-lookup"><span data-stu-id="689c5-651">usbRestrictedModeBlocked</span></span>|<span data-ttu-id="689c5-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-652">Boolean</span></span>|<span data-ttu-id="689c5-653">デバイスがロックされているときに USB アクセサリへの接続が許可されるかどうかを示します (iOS 11.4.1 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-653">Indicates if connecting to USB accessories while the device is locked is allowed (iOS 11.4.1 and later).</span></span>|
|<span data-ttu-id="689c5-654">passwordblockautofill フィル</span><span class="sxs-lookup"><span data-stu-id="689c5-654">passwordBlockAutoFill</span></span>|<span data-ttu-id="689c5-655">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-655">Boolean</span></span>|<span data-ttu-id="689c5-656">パスワードのオートフィル機能が許可されているかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-656">Indicates if the AutoFill passwords feature is allowed (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="689c5-657">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="689c5-657">passwordBlockProximityRequests</span></span>|<span data-ttu-id="689c5-658">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-658">Boolean</span></span>|<span data-ttu-id="689c5-659">近くのデバイスからのパスワードの要求をブロックするかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-659">Indicates whether or not to block requesting passwords from nearby devices (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="689c5-660">passwordblockエア drop共有</span><span class="sxs-lookup"><span data-stu-id="689c5-660">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="689c5-661">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-661">Boolean</span></span>|<span data-ttu-id="689c5-662">通話ドロップパスワード機能 iOS 12.0 以降) でのパスワードの共有を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="689c5-662">Indicates whether or not to block sharing passwords with the AirDrop passwords feature iOS 12.0 and later).</span></span>|
|<span data-ttu-id="689c5-663">dateandtimeforcesetautomatically に</span><span class="sxs-lookup"><span data-stu-id="689c5-663">dateAndTimeForceSetAutomatically</span></span>|<span data-ttu-id="689c5-664">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-664">Boolean</span></span>|<span data-ttu-id="689c5-665">ユーザーが日付と時刻を自動的に設定する機能が有効であるかどうか、およびユーザーが無効にすることができないかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-665">Indicates whether or not the Date and Time "Set Automatically" feature is enabled and cannot be turned off by the user (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="689c5-666">contactsAllowManagedToUnmanagedWrite</span><span class="sxs-lookup"><span data-stu-id="689c5-666">contactsAllowManagedToUnmanagedWrite</span></span>|<span data-ttu-id="689c5-667">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-667">Boolean</span></span>|<span data-ttu-id="689c5-668">管理対象アプリが、管理されていない連絡先アカウントに連絡先を書き込むことができるかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-668">Indicates whether or not managed apps can write contacts to unmanaged contacts accounts (iOS 12.0 and later).</span></span>|
|<span data-ttu-id="689c5-669">contactsAllowUnmanagedToManagedRead</span><span class="sxs-lookup"><span data-stu-id="689c5-669">contactsAllowUnmanagedToManagedRead</span></span>|<span data-ttu-id="689c5-670">Boolean</span><span class="sxs-lookup"><span data-stu-id="689c5-670">Boolean</span></span>|<span data-ttu-id="689c5-671">管理対象外アプリが管理された連絡先から読み取ることができるかどうかを示します (iOS 12.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="689c5-671">Indicates whether or not unmanaged apps can read from managed contacts accounts (iOS 12.0 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="689c5-672">応答</span><span class="sxs-lookup"><span data-stu-id="689c5-672">Response</span></span>
<span data-ttu-id="689c5-673">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="689c5-673">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="689c5-674">例</span><span class="sxs-lookup"><span data-stu-id="689c5-674">Example</span></span>

### <a name="request"></a><span data-ttu-id="689c5-675">要求</span><span class="sxs-lookup"><span data-stu-id="689c5-675">Request</span></span>
<span data-ttu-id="689c5-676">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="689c5-676">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 9105

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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
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
  "contactsAllowUnmanagedToManagedRead": true
}
```

### <a name="response"></a><span data-ttu-id="689c5-677">応答</span><span class="sxs-lookup"><span data-stu-id="689c5-677">Response</span></span>
<span data-ttu-id="689c5-p133">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="689c5-p133">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 9277

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
  "kioskModeAllowColorInversionSettings": true,
  "kioskModeAllowRingerSwitch": true,
  "kioskModeAllowScreenRotation": true,
  "kioskModeAllowSleepButton": true,
  "kioskModeAllowTouchscreen": true,
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
  "contactsAllowUnmanagedToManagedRead": true
}
```




