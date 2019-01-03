---
title: Update iosGeneralDeviceConfiguration
description: iosGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 3919b743cae86d40a30c03e39b7bdc89312c1cca
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334340"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="dc63d-103">Update iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="dc63d-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="dc63d-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc63d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc63d-105">[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-105">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc63d-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="dc63d-106">Prerequisites</span></span>
<span data-ttu-id="dc63d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc63d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc63d-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc63d-109">Permission type</span></span>|<span data-ttu-id="dc63d-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc63d-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc63d-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc63d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dc63d-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc63d-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dc63d-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc63d-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc63d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc63d-114">Not supported.</span></span>|
|<span data-ttu-id="dc63d-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc63d-115">Application</span></span>|<span data-ttu-id="dc63d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc63d-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc63d-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc63d-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dc63d-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc63d-118">Request headers</span></span>
|<span data-ttu-id="dc63d-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc63d-119">Header</span></span>|<span data-ttu-id="dc63d-120">値</span><span class="sxs-lookup"><span data-stu-id="dc63d-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc63d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc63d-121">Authorization</span></span>|<span data-ttu-id="dc63d-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dc63d-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc63d-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dc63d-123">Accept</span></span>|<span data-ttu-id="dc63d-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dc63d-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc63d-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc63d-125">Request body</span></span>
<span data-ttu-id="dc63d-126">要求本文で、[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-126">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="dc63d-127">次の表に、[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-127">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="dc63d-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc63d-128">Property</span></span>|<span data-ttu-id="dc63d-129">種類</span><span class="sxs-lookup"><span data-stu-id="dc63d-129">Type</span></span>|<span data-ttu-id="dc63d-130">説明</span><span class="sxs-lookup"><span data-stu-id="dc63d-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc63d-131">ID</span><span class="sxs-lookup"><span data-stu-id="dc63d-131">id</span></span>|<span data-ttu-id="dc63d-132">String</span><span class="sxs-lookup"><span data-stu-id="dc63d-132">String</span></span>|<span data-ttu-id="dc63d-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dc63d-133">Key of the entity.</span></span> <span data-ttu-id="dc63d-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dc63d-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc63d-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dc63d-135">lastModifiedDateTime</span></span>|<span data-ttu-id="dc63d-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc63d-136">DateTimeOffset</span></span>|<span data-ttu-id="dc63d-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="dc63d-137">DateTime the object was last modified.</span></span> <span data-ttu-id="dc63d-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dc63d-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc63d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dc63d-139">createdDateTime</span></span>|<span data-ttu-id="dc63d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dc63d-140">DateTimeOffset</span></span>|<span data-ttu-id="dc63d-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="dc63d-141">DateTime the object was created.</span></span> <span data-ttu-id="dc63d-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dc63d-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc63d-143">説明</span><span class="sxs-lookup"><span data-stu-id="dc63d-143">description</span></span>|<span data-ttu-id="dc63d-144">String</span><span class="sxs-lookup"><span data-stu-id="dc63d-144">String</span></span>|<span data-ttu-id="dc63d-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="dc63d-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dc63d-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dc63d-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc63d-147">displayName</span><span class="sxs-lookup"><span data-stu-id="dc63d-147">displayName</span></span>|<span data-ttu-id="dc63d-148">String</span><span class="sxs-lookup"><span data-stu-id="dc63d-148">String</span></span>|<span data-ttu-id="dc63d-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="dc63d-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dc63d-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dc63d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc63d-151">version</span><span class="sxs-lookup"><span data-stu-id="dc63d-151">version</span></span>|<span data-ttu-id="dc63d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="dc63d-152">Int32</span></span>|<span data-ttu-id="dc63d-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="dc63d-153">Version of the device configuration.</span></span> <span data-ttu-id="dc63d-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="dc63d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dc63d-155">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-155">accountBlockModification</span></span>|<span data-ttu-id="dc63d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-156">Boolean</span></span>|<span data-ttu-id="dc63d-157">デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-157">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-158">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="dc63d-158">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="dc63d-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-159">Boolean</span></span>|<span data-ttu-id="dc63d-160">デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-160">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="dc63d-161">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-161">airDropBlocked</span></span>|<span data-ttu-id="dc63d-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-162">Boolean</span></span>|<span data-ttu-id="dc63d-163">デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-163">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-164">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="dc63d-164">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="dc63d-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-165">Boolean</span></span>|<span data-ttu-id="dc63d-166">AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-166">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dc63d-167">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="dc63d-167">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="dc63d-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-168">Boolean</span></span>|<span data-ttu-id="dc63d-169">ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-169">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="dc63d-170">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="dc63d-170">appleWatchBlockPairing</span></span>|<span data-ttu-id="dc63d-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-171">Boolean</span></span>|<span data-ttu-id="dc63d-172">デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-172">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dc63d-173">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="dc63d-173">appleWatchForceWristDetection</span></span>|<span data-ttu-id="dc63d-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-174">Boolean</span></span>|<span data-ttu-id="dc63d-175">ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-175">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="dc63d-176">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-176">appleNewsBlocked</span></span>|<span data-ttu-id="dc63d-177">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-177">Boolean</span></span>|<span data-ttu-id="dc63d-178">デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-178">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dc63d-179">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="dc63d-179">appsSingleAppModeList</span></span>|<span data-ttu-id="dc63d-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc63d-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="dc63d-181">単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-181">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="dc63d-182">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="dc63d-182">Supervised only.</span></span> <span data-ttu-id="dc63d-183">iOS 7.0 以降。</span><span class="sxs-lookup"><span data-stu-id="dc63d-183">iOS 7.0 and later.</span></span> <span data-ttu-id="dc63d-184">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-184">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="dc63d-185">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="dc63d-185">appsVisibilityList</span></span>|<span data-ttu-id="dc63d-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc63d-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="dc63d-187">可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-187">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="dc63d-188">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="dc63d-189">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="dc63d-189">appsVisibilityListType</span></span>|[<span data-ttu-id="dc63d-190">appListType</span><span class="sxs-lookup"><span data-stu-id="dc63d-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="dc63d-191">AppsVisibilityList 内にあるリストの種類です。</span><span class="sxs-lookup"><span data-stu-id="dc63d-191">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="dc63d-192">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="dc63d-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="dc63d-193">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="dc63d-193">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="dc63d-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-194">Boolean</span></span>|<span data-ttu-id="dc63d-195">デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-195">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dc63d-196">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-196">appStoreBlocked</span></span>|<span data-ttu-id="dc63d-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-197">Boolean</span></span>|<span data-ttu-id="dc63d-198">ユーザーによる App Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-198">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="dc63d-199">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="dc63d-199">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="dc63d-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-200">Boolean</span></span>|<span data-ttu-id="dc63d-201">ユーザーによるアプリの購入を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-201">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="dc63d-202">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="dc63d-202">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="dc63d-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-203">Boolean</span></span>|<span data-ttu-id="dc63d-204">ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-204">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="dc63d-205">監視モードのみに適用されます (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-205">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dc63d-206">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="dc63d-206">appStoreRequirePassword</span></span>|<span data-ttu-id="dc63d-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-207">Boolean</span></span>|<span data-ttu-id="dc63d-208">App Store 使用時に、パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-208">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="dc63d-209">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-209">bluetoothBlockModification</span></span>|<span data-ttu-id="dc63d-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-210">Boolean</span></span>|<span data-ttu-id="dc63d-211">デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-211">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="dc63d-212">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-212">cameraBlocked</span></span>|<span data-ttu-id="dc63d-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-213">Boolean</span></span>|<span data-ttu-id="dc63d-214">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-214">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="dc63d-215">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="dc63d-215">cellularBlockDataRoaming</span></span>|<span data-ttu-id="dc63d-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-216">Boolean</span></span>|<span data-ttu-id="dc63d-217">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-217">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="dc63d-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="dc63d-218">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="dc63d-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-219">Boolean</span></span>|<span data-ttu-id="dc63d-220">ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-220">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="dc63d-221">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-221">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="dc63d-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-222">Boolean</span></span>|<span data-ttu-id="dc63d-223">デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-223">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-224">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="dc63d-224">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="dc63d-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-225">Boolean</span></span>|<span data-ttu-id="dc63d-226">個人用ホットスポットをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-226">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="dc63d-227">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="dc63d-227">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="dc63d-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-228">Boolean</span></span>|<span data-ttu-id="dc63d-229">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-229">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="dc63d-230">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="dc63d-230">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="dc63d-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-231">Boolean</span></span>|<span data-ttu-id="dc63d-232">信頼されていない TLS の証明書をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-232">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="dc63d-233">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="dc63d-233">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="dc63d-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-234">Boolean</span></span>|<span data-ttu-id="dc63d-235">デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-235">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="dc63d-236">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="dc63d-236">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="dc63d-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-237">Boolean</span></span>|<span data-ttu-id="dc63d-238">デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-238">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-239">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="dc63d-239">compliantAppsList</span></span>|<span data-ttu-id="dc63d-240">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc63d-240">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="dc63d-241">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-241">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="dc63d-242">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-242">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="dc63d-243">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="dc63d-243">compliantAppListType</span></span>|[<span data-ttu-id="dc63d-244">appListType</span><span class="sxs-lookup"><span data-stu-id="dc63d-244">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="dc63d-245">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="dc63d-245">List that is in the AppComplianceList.</span></span> <span data-ttu-id="dc63d-246">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="dc63d-246">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="dc63d-247">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="dc63d-247">configurationProfileBlockChanges</span></span>|<span data-ttu-id="dc63d-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-248">Boolean</span></span>|<span data-ttu-id="dc63d-249">デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-249">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-250">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-250">definitionLookupBlocked</span></span>|<span data-ttu-id="dc63d-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-251">Boolean</span></span>|<span data-ttu-id="dc63d-252">デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-252">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="dc63d-253">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="dc63d-253">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="dc63d-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-254">Boolean</span></span>|<span data-ttu-id="dc63d-255">デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-255">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-256">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="dc63d-256">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="dc63d-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-257">Boolean</span></span>|<span data-ttu-id="dc63d-258">デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-258">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-259">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-259">deviceBlockNameModification</span></span>|<span data-ttu-id="dc63d-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-260">Boolean</span></span>|<span data-ttu-id="dc63d-261">デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-261">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dc63d-262">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="dc63d-262">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="dc63d-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-263">Boolean</span></span>|<span data-ttu-id="dc63d-264">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-264">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="dc63d-265">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-265">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="dc63d-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-266">Boolean</span></span>|<span data-ttu-id="dc63d-267">デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-267">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="dc63d-268">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="dc63d-268">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="dc63d-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-269">Boolean</span></span>|<span data-ttu-id="dc63d-270">ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-270">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="dc63d-271">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="dc63d-271">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="dc63d-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-272">Boolean</span></span>|<span data-ttu-id="dc63d-273">ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-273">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="dc63d-274">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="dc63d-274">emailInDomainSuffixes</span></span>|<span data-ttu-id="dc63d-275">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dc63d-275">String collection</span></span>|<span data-ttu-id="dc63d-276">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-276">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="dc63d-277">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="dc63d-277">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="dc63d-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-278">Boolean</span></span>|<span data-ttu-id="dc63d-279">ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-279">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="dc63d-280">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-280">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="dc63d-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-281">Boolean</span></span>|<span data-ttu-id="dc63d-282">ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-282">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="dc63d-283">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-283">faceTimeBlocked</span></span>|<span data-ttu-id="dc63d-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-284">Boolean</span></span>|<span data-ttu-id="dc63d-285">ユーザーによる FaceTime の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-285">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="dc63d-286">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-286">findMyFriendsBlocked</span></span>|<span data-ttu-id="dc63d-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-287">Boolean</span></span>|<span data-ttu-id="dc63d-288">デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-288">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-289">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="dc63d-289">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="dc63d-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-290">Boolean</span></span>|<span data-ttu-id="dc63d-291">ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-291">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="dc63d-292">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="dc63d-292">gamingBlockMultiplayer</span></span>|<span data-ttu-id="dc63d-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-293">Boolean</span></span>|<span data-ttu-id="dc63d-294">ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-294">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="dc63d-295">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-295">gameCenterBlocked</span></span>|<span data-ttu-id="dc63d-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-296">Boolean</span></span>|<span data-ttu-id="dc63d-297">デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-297">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-298">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-298">hostPairingBlocked</span></span>|<span data-ttu-id="dc63d-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-299">Boolean</span></span>|<span data-ttu-id="dc63d-300">iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-300">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-301">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-301">iBooksStoreBlocked</span></span>|<span data-ttu-id="dc63d-302">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-302">Boolean</span></span>|<span data-ttu-id="dc63d-303">デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-303">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-304">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="dc63d-304">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="dc63d-305">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-305">Boolean</span></span>|<span data-ttu-id="dc63d-306">アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-306">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="dc63d-307">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="dc63d-307">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="dc63d-308">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-308">Boolean</span></span>|<span data-ttu-id="dc63d-309">iOS デバイスで起動した作業の、別の iOS デバイスまたは macOS デバイスでの継続実施をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-309">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="dc63d-310">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="dc63d-310">iCloudBlockBackup</span></span>|<span data-ttu-id="dc63d-311">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-311">Boolean</span></span>|<span data-ttu-id="dc63d-312">iCloud バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-312">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="dc63d-313">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="dc63d-313">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="dc63d-314">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-314">Boolean</span></span>|<span data-ttu-id="dc63d-315">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-315">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="dc63d-316">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="dc63d-316">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="dc63d-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-317">Boolean</span></span>|<span data-ttu-id="dc63d-318">管理対象アプリのクラウドの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-318">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="dc63d-319">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="dc63d-319">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="dc63d-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-320">Boolean</span></span>|<span data-ttu-id="dc63d-321">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-321">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="dc63d-322">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="dc63d-322">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="dc63d-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-323">Boolean</span></span>|<span data-ttu-id="dc63d-324">iCloud フォトのストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-324">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="dc63d-325">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="dc63d-325">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="dc63d-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-326">Boolean</span></span>|<span data-ttu-id="dc63d-327">共有フォト ストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-327">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="dc63d-328">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="dc63d-328">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="dc63d-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-329">Boolean</span></span>|<span data-ttu-id="dc63d-330">iCloud のバックアップを暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-330">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="dc63d-331">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="dc63d-331">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="dc63d-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-332">Boolean</span></span>|<span data-ttu-id="dc63d-333">ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-333">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="dc63d-334">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="dc63d-334">iTunesBlockMusicService</span></span>|<span data-ttu-id="dc63d-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-335">Boolean</span></span>|<span data-ttu-id="dc63d-336">デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-336">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="dc63d-337">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="dc63d-337">iTunesBlockRadio</span></span>|<span data-ttu-id="dc63d-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-338">Boolean</span></span>|<span data-ttu-id="dc63d-339">デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-339">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="dc63d-340">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="dc63d-340">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="dc63d-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-341">Boolean</span></span>|<span data-ttu-id="dc63d-342">デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-342">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="dc63d-343">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="dc63d-343">keyboardBlockDictation</span></span>|<span data-ttu-id="dc63d-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-344">Boolean</span></span>|<span data-ttu-id="dc63d-345">デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-345">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-346">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="dc63d-346">keyboardBlockPredictive</span></span>|<span data-ttu-id="dc63d-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-347">Boolean</span></span>|<span data-ttu-id="dc63d-348">デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-348">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="dc63d-349">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="dc63d-349">keyboardBlockShortcuts</span></span>|<span data-ttu-id="dc63d-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-350">Boolean</span></span>|<span data-ttu-id="dc63d-351">デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-351">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dc63d-352">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="dc63d-352">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="dc63d-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-353">Boolean</span></span>|<span data-ttu-id="dc63d-354">デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-354">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="dc63d-355">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="dc63d-355">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="dc63d-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-356">Boolean</span></span>|<span data-ttu-id="dc63d-357">キオスク モード時の補助音声を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-357">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-358">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="dc63d-358">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="dc63d-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-359">Boolean</span></span>|<span data-ttu-id="dc63d-360">キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-360">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-361">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="dc63d-361">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="dc63d-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-362">Boolean</span></span>|<span data-ttu-id="dc63d-363">キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-363">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-364">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="dc63d-364">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="dc63d-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-365">Boolean</span></span>|<span data-ttu-id="dc63d-366">キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-366">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-367">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="dc63d-367">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="dc63d-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-368">Boolean</span></span>|<span data-ttu-id="dc63d-369">キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-369">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-370">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="dc63d-370">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="dc63d-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-371">Boolean</span></span>|<span data-ttu-id="dc63d-372">キオスク モード時の画面の回転を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-372">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-373">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="dc63d-373">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="dc63d-374">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-374">Boolean</span></span>|<span data-ttu-id="dc63d-375">キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-375">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-376">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="dc63d-376">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="dc63d-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-377">Boolean</span></span>|<span data-ttu-id="dc63d-378">キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-378">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-379">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="dc63d-379">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="dc63d-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-380">Boolean</span></span>|<span data-ttu-id="dc63d-381">キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-381">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-382">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="dc63d-382">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="dc63d-383">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-383">Boolean</span></span>|<span data-ttu-id="dc63d-384">キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-384">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-385">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="dc63d-385">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="dc63d-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-386">Boolean</span></span>|<span data-ttu-id="dc63d-387">キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-387">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-388">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="dc63d-388">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="dc63d-389">String</span><span class="sxs-lookup"><span data-stu-id="dc63d-389">String</span></span>|<span data-ttu-id="dc63d-390">キオスク モード用に使用するアプリへの、App Store 内の URL。</span><span class="sxs-lookup"><span data-stu-id="dc63d-390">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="dc63d-391">KioskModeManagedAppId が不明な場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-391">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="dc63d-392">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="dc63d-392">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="dc63d-393">String</span><span class="sxs-lookup"><span data-stu-id="dc63d-393">String</span></span>|<span data-ttu-id="dc63d-394">キオスク モードを使用する組み込みアプリケーションの ID です。</span><span class="sxs-lookup"><span data-stu-id="dc63d-394">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="dc63d-395">KioskModeManagedAppId と KioskModeAppStoreUrl が設定されていない場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-395">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="dc63d-396">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="dc63d-396">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="dc63d-397">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-397">Boolean</span></span>|<span data-ttu-id="dc63d-398">キオスク モード時に Assistive Touch が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-398">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-399">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="dc63d-399">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="dc63d-400">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-400">Boolean</span></span>|<span data-ttu-id="dc63d-401">キオスク モード時に色反転が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-401">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-402">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="dc63d-402">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="dc63d-403">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-403">Boolean</span></span>|<span data-ttu-id="dc63d-404">キオスク モード時にモノラル オーディオが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-404">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-405">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="dc63d-405">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="dc63d-406">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-406">Boolean</span></span>|<span data-ttu-id="dc63d-407">キオスク モード時にボイス オーバーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-407">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-408">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="dc63d-408">kioskModeRequireZoom</span></span>|<span data-ttu-id="dc63d-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-409">Boolean</span></span>|<span data-ttu-id="dc63d-410">キオスク モード時にズームが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-410">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="dc63d-411">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="dc63d-411">kioskModeManagedAppId</span></span>|<span data-ttu-id="dc63d-412">String</span><span class="sxs-lookup"><span data-stu-id="dc63d-412">String</span></span>|<span data-ttu-id="dc63d-413">キオスク モード用に使用するアプリの管理対象アプリ ID。</span><span class="sxs-lookup"><span data-stu-id="dc63d-413">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="dc63d-414">KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-414">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="dc63d-415">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="dc63d-415">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="dc63d-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-416">Boolean</span></span>|<span data-ttu-id="dc63d-417">ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-417">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="dc63d-418">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="dc63d-418">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="dc63d-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-419">Boolean</span></span>|<span data-ttu-id="dc63d-420">ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-420">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="dc63d-421">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="dc63d-421">lockScreenBlockPassbook</span></span>|<span data-ttu-id="dc63d-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-422">Boolean</span></span>|<span data-ttu-id="dc63d-423">デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-423">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="dc63d-424">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="dc63d-424">lockScreenBlockTodayView</span></span>|<span data-ttu-id="dc63d-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-425">Boolean</span></span>|<span data-ttu-id="dc63d-426">ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-426">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="dc63d-427">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="dc63d-427">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="dc63d-428">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="dc63d-428">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="dc63d-429">メディア コンテンツの評価の設定 (オーストラリア向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-429">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="dc63d-430">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="dc63d-430">mediaContentRatingCanada</span></span>|[<span data-ttu-id="dc63d-431">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="dc63d-431">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="dc63d-432">メディア コンテンツの評価の設定 (カナダ向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-432">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="dc63d-433">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="dc63d-433">mediaContentRatingFrance</span></span>|[<span data-ttu-id="dc63d-434">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="dc63d-434">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="dc63d-435">メディア コンテンツの評価の設定 (フランス向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-435">Media content rating settings for France</span></span>|
|<span data-ttu-id="dc63d-436">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="dc63d-436">mediaContentRatingGermany</span></span>|[<span data-ttu-id="dc63d-437">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="dc63d-437">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="dc63d-438">メディア コンテンツの評価の設定 (ドイツ向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-438">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="dc63d-439">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="dc63d-439">mediaContentRatingIreland</span></span>|[<span data-ttu-id="dc63d-440">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="dc63d-440">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="dc63d-441">メディア コンテンツの評価の設定 (アイルランド向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-441">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="dc63d-442">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="dc63d-442">mediaContentRatingJapan</span></span>|[<span data-ttu-id="dc63d-443">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="dc63d-443">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="dc63d-444">メディア コンテンツの評価の設定 (日本向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-444">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="dc63d-445">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="dc63d-445">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="dc63d-446">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="dc63d-446">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="dc63d-447">メディア コンテンツの評価の設定 (ニュージーランド向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-447">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="dc63d-448">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="dc63d-448">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="dc63d-449">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="dc63d-449">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="dc63d-450">メディア コンテンツの評価の設定 (英国向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-450">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="dc63d-451">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="dc63d-451">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="dc63d-452">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="dc63d-452">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="dc63d-453">メディア コンテンツの評価の設定 (米国向け)</span><span class="sxs-lookup"><span data-stu-id="dc63d-453">Media content rating settings for United States</span></span>|
|<span data-ttu-id="dc63d-454">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="dc63d-454">networkUsageRules</span></span>|<span data-ttu-id="dc63d-455">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="dc63d-455">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="dc63d-456">管理対象アプリと、それらに適用されるネットワーク ルールのリストです。</span><span class="sxs-lookup"><span data-stu-id="dc63d-456">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="dc63d-457">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-457">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="dc63d-458">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="dc63d-458">mediaContentRatingApps</span></span>|[<span data-ttu-id="dc63d-459">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="dc63d-459">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="dc63d-460">メディア コンテンツのアプリケーションの設定を評価します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-460">Media content rating settings for Apps.</span></span> <span data-ttu-id="dc63d-461">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="dc63d-461">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="dc63d-462">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-462">messagesBlocked</span></span>|<span data-ttu-id="dc63d-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-463">Boolean</span></span>|<span data-ttu-id="dc63d-464">ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-464">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="dc63d-465">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-465">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="dc63d-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-466">Boolean</span></span>|<span data-ttu-id="dc63d-467">通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-467">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="dc63d-468">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="dc63d-468">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="dc63d-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-469">Boolean</span></span>|<span data-ttu-id="dc63d-470">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-470">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="dc63d-471">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-471">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="dc63d-472">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-472">Boolean</span></span>|<span data-ttu-id="dc63d-473">監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-473">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="dc63d-474">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-474">passcodeBlockModification</span></span>|<span data-ttu-id="dc63d-475">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-475">Boolean</span></span>|<span data-ttu-id="dc63d-476">監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-476">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="dc63d-477">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="dc63d-477">passcodeBlockSimple</span></span>|<span data-ttu-id="dc63d-478">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-478">Boolean</span></span>|<span data-ttu-id="dc63d-479">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-479">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="dc63d-480">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="dc63d-480">passcodeExpirationDays</span></span>|<span data-ttu-id="dc63d-481">Int32</span><span class="sxs-lookup"><span data-stu-id="dc63d-481">Int32</span></span>|<span data-ttu-id="dc63d-482">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="dc63d-482">Number of days before the passcode expires.</span></span> <span data-ttu-id="dc63d-483">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="dc63d-483">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="dc63d-484">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="dc63d-484">passcodeMinimumLength</span></span>|<span data-ttu-id="dc63d-485">Int32</span><span class="sxs-lookup"><span data-stu-id="dc63d-485">Int32</span></span>|<span data-ttu-id="dc63d-486">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="dc63d-486">Minimum length of passcode.</span></span> <span data-ttu-id="dc63d-487">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="dc63d-487">Valid values 4 to 14</span></span>|
|<span data-ttu-id="dc63d-488">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="dc63d-488">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="dc63d-489">Int32</span><span class="sxs-lookup"><span data-stu-id="dc63d-489">Int32</span></span>|<span data-ttu-id="dc63d-490">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-490">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="dc63d-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="dc63d-491">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="dc63d-492">Int32</span><span class="sxs-lookup"><span data-stu-id="dc63d-492">Int32</span></span>|<span data-ttu-id="dc63d-493">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-493">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="dc63d-494">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="dc63d-494">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="dc63d-495">Int32</span><span class="sxs-lookup"><span data-stu-id="dc63d-495">Int32</span></span>|<span data-ttu-id="dc63d-496">パスコードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="dc63d-496">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="dc63d-497">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="dc63d-497">Valid values 0 to 4</span></span>|
|<span data-ttu-id="dc63d-498">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="dc63d-498">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="dc63d-499">Int32</span><span class="sxs-lookup"><span data-stu-id="dc63d-499">Int32</span></span>|<span data-ttu-id="dc63d-500">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="dc63d-500">Number of previous passcodes to block.</span></span> <span data-ttu-id="dc63d-501">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="dc63d-501">Valid values 1 to 24</span></span>|
|<span data-ttu-id="dc63d-502">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="dc63d-502">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="dc63d-503">Int32</span><span class="sxs-lookup"><span data-stu-id="dc63d-503">Int32</span></span>|<span data-ttu-id="dc63d-504">デバイスをワイプするまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="dc63d-504">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="dc63d-505">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="dc63d-505">Valid values 4 to 11</span></span>|
|<span data-ttu-id="dc63d-506">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="dc63d-506">passcodeRequiredType</span></span>|[<span data-ttu-id="dc63d-507">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="dc63d-507">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="dc63d-508">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="dc63d-508">Type of passcode that is required.</span></span> <span data-ttu-id="dc63d-509">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="dc63d-509">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="dc63d-510">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="dc63d-510">passcodeRequired</span></span>|<span data-ttu-id="dc63d-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-511">Boolean</span></span>|<span data-ttu-id="dc63d-512">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-512">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="dc63d-513">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-513">podcastsBlocked</span></span>|<span data-ttu-id="dc63d-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-514">Boolean</span></span>|<span data-ttu-id="dc63d-515">ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-515">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="dc63d-516">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="dc63d-516">safariBlockAutofill</span></span>|<span data-ttu-id="dc63d-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-517">Boolean</span></span>|<span data-ttu-id="dc63d-518">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-518">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="dc63d-519">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="dc63d-519">safariBlockJavaScript</span></span>|<span data-ttu-id="dc63d-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-520">Boolean</span></span>|<span data-ttu-id="dc63d-521">Safari 内で JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-521">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="dc63d-522">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="dc63d-522">safariBlockPopups</span></span>|<span data-ttu-id="dc63d-523">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-523">Boolean</span></span>|<span data-ttu-id="dc63d-524">Safari 内でポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-524">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="dc63d-525">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-525">safariBlocked</span></span>|<span data-ttu-id="dc63d-526">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-526">Boolean</span></span>|<span data-ttu-id="dc63d-527">ユーザーによる Safari の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-527">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="dc63d-528">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="dc63d-528">safariCookieSettings</span></span>|[<span data-ttu-id="dc63d-529">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="dc63d-529">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="dc63d-530">Safari の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="dc63d-530">Cookie settings for Safari.</span></span> <span data-ttu-id="dc63d-531">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="dc63d-531">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="dc63d-532">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="dc63d-532">safariManagedDomains</span></span>|<span data-ttu-id="dc63d-533">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dc63d-533">String collection</span></span>|<span data-ttu-id="dc63d-534">ここに記載されているパターンに一致する URL は管理対象と見なされます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-534">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="dc63d-535">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="dc63d-535">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="dc63d-536">String コレクション</span><span class="sxs-lookup"><span data-stu-id="dc63d-536">String collection</span></span>|<span data-ttu-id="dc63d-537">ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-537">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="dc63d-538">監視モードのデバイスに適用されます (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-538">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="dc63d-539">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="dc63d-539">safariRequireFraudWarning</span></span>|<span data-ttu-id="dc63d-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-540">Boolean</span></span>|<span data-ttu-id="dc63d-541">Safari での不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-541">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="dc63d-542">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-542">screenCaptureBlocked</span></span>|<span data-ttu-id="dc63d-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-543">Boolean</span></span>|<span data-ttu-id="dc63d-544">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-544">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="dc63d-545">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-545">siriBlocked</span></span>|<span data-ttu-id="dc63d-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-546">Boolean</span></span>|<span data-ttu-id="dc63d-547">ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-547">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="dc63d-548">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-548">siriBlockedWhenLocked</span></span>|<span data-ttu-id="dc63d-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-549">Boolean</span></span>|<span data-ttu-id="dc63d-550">ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-550">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="dc63d-551">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="dc63d-551">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="dc63d-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-552">Boolean</span></span>|<span data-ttu-id="dc63d-553">監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-553">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="dc63d-554">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="dc63d-554">siriRequireProfanityFilter</span></span>|<span data-ttu-id="dc63d-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-555">Boolean</span></span>|<span data-ttu-id="dc63d-556">Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-556">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="dc63d-557">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="dc63d-557">spotlightBlockInternetResults</span></span>|<span data-ttu-id="dc63d-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-558">Boolean</span></span>|<span data-ttu-id="dc63d-559">監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-559">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="dc63d-560">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="dc63d-560">voiceDialingBlocked</span></span>|<span data-ttu-id="dc63d-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-561">Boolean</span></span>|<span data-ttu-id="dc63d-562">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-562">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="dc63d-563">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="dc63d-563">wallpaperBlockModification</span></span>|<span data-ttu-id="dc63d-564">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-564">Boolean</span></span>|<span data-ttu-id="dc63d-565">監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="dc63d-565">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="dc63d-566">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="dc63d-566">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="dc63d-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="dc63d-567">Boolean</span></span>|<span data-ttu-id="dc63d-568">デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-568">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|



## <a name="response"></a><span data-ttu-id="dc63d-569">応答</span><span class="sxs-lookup"><span data-stu-id="dc63d-569">Response</span></span>
<span data-ttu-id="dc63d-570">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dc63d-570">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc63d-571">例</span><span class="sxs-lookup"><span data-stu-id="dc63d-571">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc63d-572">要求</span><span class="sxs-lookup"><span data-stu-id="dc63d-572">Request</span></span>
<span data-ttu-id="dc63d-573">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc63d-573">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 7841

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```

### <a name="response"></a><span data-ttu-id="dc63d-574">応答</span><span class="sxs-lookup"><span data-stu-id="dc63d-574">Response</span></span>
<span data-ttu-id="dc63d-p127">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc63d-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8013

{
  "@odata.type": "#microsoft.graph.iosGeneralDeviceConfiguration",
  "id": "ebba5202-5202-ebba-0252-baeb0252baeb",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "bluetoothBlockModification": true,
  "cameraBlocked": true,
  "cellularBlockDataRoaming": true,
  "cellularBlockGlobalBackgroundFetchWhileRoaming": true,
  "cellularBlockPerAppDataModification": true,
  "cellularBlockPersonalHotspot": true,
  "cellularBlockVoiceRoaming": true,
  "certificatesBlockUntrustedTlsCertificates": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
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
  "spotlightBlockInternetResults": true,
  "voiceDialingBlocked": true,
  "wallpaperBlockModification": true,
  "wiFiConnectOnlyToConfiguredNetworks": true
}
```


