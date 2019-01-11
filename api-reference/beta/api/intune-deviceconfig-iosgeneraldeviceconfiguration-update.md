---
title: Update iosGeneralDeviceConfiguration
description: iosGeneralDeviceConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8c4aa2af2946c7e99d8a17b3bc98a688b10efd04
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27854020"
---
# <a name="update-iosgeneraldeviceconfiguration"></a><span data-ttu-id="f45fd-103">Update iosGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f45fd-103">Update iosGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f45fd-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f45fd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f45fd-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f45fd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f45fd-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f45fd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f45fd-107">[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-107">Update the properties of a [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f45fd-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f45fd-108">Prerequisites</span></span>
<span data-ttu-id="f45fd-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f45fd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f45fd-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f45fd-111">Permission type</span></span>|<span data-ttu-id="f45fd-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f45fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f45fd-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f45fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f45fd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f45fd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f45fd-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f45fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f45fd-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f45fd-116">Not supported.</span></span>|
|<span data-ttu-id="f45fd-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f45fd-117">Application</span></span>|<span data-ttu-id="f45fd-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f45fd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f45fd-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f45fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f45fd-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f45fd-120">Request headers</span></span>
|<span data-ttu-id="f45fd-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f45fd-121">Header</span></span>|<span data-ttu-id="f45fd-122">値</span><span class="sxs-lookup"><span data-stu-id="f45fd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f45fd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f45fd-123">Authorization</span></span>|<span data-ttu-id="f45fd-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f45fd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f45fd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f45fd-125">Accept</span></span>|<span data-ttu-id="f45fd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f45fd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f45fd-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f45fd-127">Request body</span></span>
<span data-ttu-id="f45fd-128">要求本文で、[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-128">In the request body, supply a JSON representation for the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="f45fd-129">次の表に、[iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-129">The following table shows the properties that are required when you create the [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="f45fd-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f45fd-130">Property</span></span>|<span data-ttu-id="f45fd-131">種類</span><span class="sxs-lookup"><span data-stu-id="f45fd-131">Type</span></span>|<span data-ttu-id="f45fd-132">説明</span><span class="sxs-lookup"><span data-stu-id="f45fd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f45fd-133">ID</span><span class="sxs-lookup"><span data-stu-id="f45fd-133">id</span></span>|<span data-ttu-id="f45fd-134">String</span><span class="sxs-lookup"><span data-stu-id="f45fd-134">String</span></span>|<span data-ttu-id="f45fd-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f45fd-135">Key of the entity.</span></span> <span data-ttu-id="f45fd-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45fd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f45fd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f45fd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f45fd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45fd-138">DateTimeOffset</span></span>|<span data-ttu-id="f45fd-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f45fd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f45fd-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45fd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f45fd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f45fd-141">roleScopeTagIds</span></span>|<span data-ttu-id="f45fd-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f45fd-142">String collection</span></span>|<span data-ttu-id="f45fd-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="f45fd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f45fd-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45fd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f45fd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f45fd-145">supportsScopeTags</span></span>|<span data-ttu-id="f45fd-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-146">Boolean</span></span>|<span data-ttu-id="f45fd-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f45fd-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="f45fd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f45fd-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f45fd-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="f45fd-150">This property is read-only.</span></span> <span data-ttu-id="f45fd-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45fd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f45fd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f45fd-152">createdDateTime</span></span>|<span data-ttu-id="f45fd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f45fd-153">DateTimeOffset</span></span>|<span data-ttu-id="f45fd-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f45fd-154">DateTime the object was created.</span></span> <span data-ttu-id="f45fd-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45fd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f45fd-156">説明</span><span class="sxs-lookup"><span data-stu-id="f45fd-156">description</span></span>|<span data-ttu-id="f45fd-157">String</span><span class="sxs-lookup"><span data-stu-id="f45fd-157">String</span></span>|<span data-ttu-id="f45fd-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="f45fd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f45fd-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45fd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f45fd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f45fd-160">displayName</span></span>|<span data-ttu-id="f45fd-161">String</span><span class="sxs-lookup"><span data-stu-id="f45fd-161">String</span></span>|<span data-ttu-id="f45fd-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="f45fd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f45fd-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45fd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f45fd-164">version</span><span class="sxs-lookup"><span data-stu-id="f45fd-164">version</span></span>|<span data-ttu-id="f45fd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f45fd-165">Int32</span></span>|<span data-ttu-id="f45fd-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f45fd-166">Version of the device configuration.</span></span> <span data-ttu-id="f45fd-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f45fd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f45fd-168">accountBlockModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-168">accountBlockModification</span></span>|<span data-ttu-id="f45fd-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-169">Boolean</span></span>|<span data-ttu-id="f45fd-170">デバイスが監視モードのときに、アカウントの変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-170">Indicates whether or not to allow account modification when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-171">activationLockAllowWhenSupervised</span><span class="sxs-lookup"><span data-stu-id="f45fd-171">activationLockAllowWhenSupervised</span></span>|<span data-ttu-id="f45fd-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-172">Boolean</span></span>|<span data-ttu-id="f45fd-173">デバイスが監視モードのときに、アクティベーション ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-173">Indicates whether or not to allow activation lock when the device is in the supervised mode.</span></span>|
|<span data-ttu-id="f45fd-174">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-174">airDropBlocked</span></span>|<span data-ttu-id="f45fd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-175">Boolean</span></span>|<span data-ttu-id="f45fd-176">デバイスが監視モードのときに、AirDrop を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-176">Indicates whether or not to allow AirDrop when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-177">airDropForceUnmanagedDropTarget</span><span class="sxs-lookup"><span data-stu-id="f45fd-177">airDropForceUnmanagedDropTarget</span></span>|<span data-ttu-id="f45fd-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-178">Boolean</span></span>|<span data-ttu-id="f45fd-179">AirDrop を管理対象外のドロップ ターゲットと見なすかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-179">Indicates whether or not to cause AirDrop to be considered an unmanaged drop target (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f45fd-180">airPlayForcePairingPasswordForOutgoingRequests</span><span class="sxs-lookup"><span data-stu-id="f45fd-180">airPlayForcePairingPasswordForOutgoingRequests</span></span>|<span data-ttu-id="f45fd-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-181">Boolean</span></span>|<span data-ttu-id="f45fd-182">ペアリング パスワードを使用するために、このデバイスからの AirPlay 要求を受信するすべてのデバイスを適用するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-182">Indicates whether or not to enforce all devices receiving AirPlay requests from this device to use a pairing password.</span></span>|
|<span data-ttu-id="f45fd-183">appleWatchBlockPairing</span><span class="sxs-lookup"><span data-stu-id="f45fd-183">appleWatchBlockPairing</span></span>|<span data-ttu-id="f45fd-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-184">Boolean</span></span>|<span data-ttu-id="f45fd-185">デバイスが監視モードのときに、Apple Watch のペアリングを許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-185">Indicates whether or not to allow Apple Watch pairing when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f45fd-186">appleWatchForceWristDetection</span><span class="sxs-lookup"><span data-stu-id="f45fd-186">appleWatchForceWristDetection</span></span>|<span data-ttu-id="f45fd-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-187">Boolean</span></span>|<span data-ttu-id="f45fd-188">ペアリングされている Apple Watch に手首検出機能を強制的に使用させるかどうかを示します (iOS 8.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-188">Indicates whether or not to force a paired Apple Watch to use Wrist Detection (iOS 8.2 and later).</span></span>|
|<span data-ttu-id="f45fd-189">appleNewsBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-189">appleNewsBlocked</span></span>|<span data-ttu-id="f45fd-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-190">Boolean</span></span>|<span data-ttu-id="f45fd-191">デバイスが監視モードのときに、ユーザーによる News の使用を禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-191">Indicates whether or not to block the user from using News when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f45fd-192">appsSingleAppModeList</span><span class="sxs-lookup"><span data-stu-id="f45fd-192">appsSingleAppModeList</span></span>|<span data-ttu-id="f45fd-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f45fd-193">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f45fd-194">単一アプリ モードに自律的に入ることが許可されている iOS アプリのリストを取得または設定します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-194">Gets or sets the list of iOS apps allowed to autonomously enter Single App Mode.</span></span> <span data-ttu-id="f45fd-195">監視モードのみ。</span><span class="sxs-lookup"><span data-stu-id="f45fd-195">Supervised only.</span></span> <span data-ttu-id="f45fd-196">iOS 7.0 以降。</span><span class="sxs-lookup"><span data-stu-id="f45fd-196">iOS 7.0 and later.</span></span> <span data-ttu-id="f45fd-197">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-197">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="f45fd-198">appsVisibilityList</span><span class="sxs-lookup"><span data-stu-id="f45fd-198">appsVisibilityList</span></span>|<span data-ttu-id="f45fd-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f45fd-199">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f45fd-200">可視性リストにあるアプリのリスト (iOS 9.3 以降で、AppVisibilityListType によって制御される、表示可能/起動可能なアプリのリスト、または非表示/起動できないアプリのリスト)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-200">List of apps in the visibility list (either visible/launchable apps list or hidden/unlaunchable apps list, controlled by AppsVisibilityListType) (iOS 9.3 and later).</span></span> <span data-ttu-id="f45fd-201">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-201">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f45fd-202">appsVisibilityListType</span><span class="sxs-lookup"><span data-stu-id="f45fd-202">appsVisibilityListType</span></span>|[<span data-ttu-id="f45fd-203">appListType</span><span class="sxs-lookup"><span data-stu-id="f45fd-203">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f45fd-204">AppsVisibilityList 内にあるリストの種類です。</span><span class="sxs-lookup"><span data-stu-id="f45fd-204">Type of list that is in the AppsVisibilityList.</span></span> <span data-ttu-id="f45fd-205">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="f45fd-205">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f45fd-206">appStoreBlockAutomaticDownloads</span><span class="sxs-lookup"><span data-stu-id="f45fd-206">appStoreBlockAutomaticDownloads</span></span>|<span data-ttu-id="f45fd-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-207">Boolean</span></span>|<span data-ttu-id="f45fd-208">デバイスが監視モードのときに、他のデバイスで購入したアプリの自動ダウンロードをブロックするかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-208">Indicates whether or not to block the automatic downloading of apps purchased on other devices when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f45fd-209">appStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-209">appStoreBlocked</span></span>|<span data-ttu-id="f45fd-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-210">Boolean</span></span>|<span data-ttu-id="f45fd-211">ユーザーによる App Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-211">Indicates whether or not to block the user from using the App Store.</span></span>|
|<span data-ttu-id="f45fd-212">appStoreBlockInAppPurchases</span><span class="sxs-lookup"><span data-stu-id="f45fd-212">appStoreBlockInAppPurchases</span></span>|<span data-ttu-id="f45fd-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-213">Boolean</span></span>|<span data-ttu-id="f45fd-214">ユーザーによるアプリの購入を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-214">Indicates whether or not to block the user from making in app purchases.</span></span>|
|<span data-ttu-id="f45fd-215">appStoreBlockUIAppInstallation</span><span class="sxs-lookup"><span data-stu-id="f45fd-215">appStoreBlockUIAppInstallation</span></span>|<span data-ttu-id="f45fd-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-216">Boolean</span></span>|<span data-ttu-id="f45fd-217">ホスト アプリによるインストールを制限せずに、App Store アプリをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-217">Indicates whether or not to block the App Store app, not restricting installation through Host apps.</span></span> <span data-ttu-id="f45fd-218">監視モードのみに適用されます (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-218">Applies to supervised mode only (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f45fd-219">appStoreRequirePassword</span><span class="sxs-lookup"><span data-stu-id="f45fd-219">appStoreRequirePassword</span></span>|<span data-ttu-id="f45fd-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-220">Boolean</span></span>|<span data-ttu-id="f45fd-221">App Store 使用時に、パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-221">Indicates whether or not to require a password when using the app store.</span></span>|
|<span data-ttu-id="f45fd-222">bluetoothBlockModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-222">bluetoothBlockModification</span></span>|<span data-ttu-id="f45fd-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-223">Boolean</span></span>|<span data-ttu-id="f45fd-224">デバイスが監視モードのときに、Bluetooth の設定の変更を許可するかどうかを示します (iOS 10.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-224">Indicates whether or not to allow modification of Bluetooth settings when the device is in supervised mode (iOS 10.0 and later).</span></span>|
|<span data-ttu-id="f45fd-225">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-225">cameraBlocked</span></span>|<span data-ttu-id="f45fd-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-226">Boolean</span></span>|<span data-ttu-id="f45fd-227">ユーザーによるデバイスのカメラへのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-227">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="f45fd-228">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="f45fd-228">cellularBlockDataRoaming</span></span>|<span data-ttu-id="f45fd-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-229">Boolean</span></span>|<span data-ttu-id="f45fd-230">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-230">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="f45fd-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span><span class="sxs-lookup"><span data-stu-id="f45fd-231">cellularBlockGlobalBackgroundFetchWhileRoaming</span></span>|<span data-ttu-id="f45fd-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-232">Boolean</span></span>|<span data-ttu-id="f45fd-233">ローミング中に、グローバルなバックグラウンド フェッチをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-233">Indicates whether or not to block global background fetch while roaming.</span></span>|
|<span data-ttu-id="f45fd-234">cellularBlockPerAppDataModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-234">cellularBlockPerAppDataModification</span></span>|<span data-ttu-id="f45fd-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-235">Boolean</span></span>|<span data-ttu-id="f45fd-236">デバイスが監視モードのときに、携帯ネットワーク アプリのデータの使用設定の変更を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-236">Indicates whether or not to allow changes to cellular app data usage settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-237">cellularBlockPersonalHotspot</span><span class="sxs-lookup"><span data-stu-id="f45fd-237">cellularBlockPersonalHotspot</span></span>|<span data-ttu-id="f45fd-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-238">Boolean</span></span>|<span data-ttu-id="f45fd-239">個人用ホットスポットをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-239">Indicates whether or not to block Personal Hotspot.</span></span>|
|<span data-ttu-id="f45fd-240">cellularBlockVoiceRoaming</span><span class="sxs-lookup"><span data-stu-id="f45fd-240">cellularBlockVoiceRoaming</span></span>|<span data-ttu-id="f45fd-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-241">Boolean</span></span>|<span data-ttu-id="f45fd-242">音声通話ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-242">Indicates whether or not to block voice roaming.</span></span>|
|<span data-ttu-id="f45fd-243">certificatesBlockUntrustedTlsCertificates</span><span class="sxs-lookup"><span data-stu-id="f45fd-243">certificatesBlockUntrustedTlsCertificates</span></span>|<span data-ttu-id="f45fd-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-244">Boolean</span></span>|<span data-ttu-id="f45fd-245">信頼されていない TLS の証明書をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-245">Indicates whether or not to block untrusted TLS certificates.</span></span>|
|<span data-ttu-id="f45fd-246">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="f45fd-246">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="f45fd-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-247">Boolean</span></span>|<span data-ttu-id="f45fd-248">デバイスが監視モードのときに、Classroom アプリによるリモート画面の監視を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-248">Indicates whether or not to allow remote screen observation by Classroom app when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f45fd-249">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="f45fd-249">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="f45fd-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-250">Boolean</span></span>|<span data-ttu-id="f45fd-251">デバイスが監視モードになっているときに、Classroom アプリでの管理対象コースの教師に、メッセージを表示せずに学生の画面を表示する許可を自動的に与えるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-251">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-252">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="f45fd-252">compliantAppsList</span></span>|<span data-ttu-id="f45fd-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f45fd-253">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="f45fd-254">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-254">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="f45fd-255">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-255">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="f45fd-256">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="f45fd-256">compliantAppListType</span></span>|[<span data-ttu-id="f45fd-257">appListType</span><span class="sxs-lookup"><span data-stu-id="f45fd-257">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="f45fd-258">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="f45fd-258">List that is in the AppComplianceList.</span></span> <span data-ttu-id="f45fd-259">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="f45fd-259">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="f45fd-260">configurationProfileBlockChanges</span><span class="sxs-lookup"><span data-stu-id="f45fd-260">configurationProfileBlockChanges</span></span>|<span data-ttu-id="f45fd-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-261">Boolean</span></span>|<span data-ttu-id="f45fd-262">デバイスが監視モードのときに、ユーザーが構成プロファイルと証明書を対話形式でインストールするのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-262">Indicates whether or not to block the user from installing configuration profiles and certificates interactively when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-263">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-263">definitionLookupBlocked</span></span>|<span data-ttu-id="f45fd-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-264">Boolean</span></span>|<span data-ttu-id="f45fd-265">デバイスが監視モードのときに、定義の検索を禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-265">Indicates whether or not to block definition lookup when the device is in supervised mode (iOS 8.1.3 and later ).</span></span>|
|<span data-ttu-id="f45fd-266">deviceBlockEnableRestrictions</span><span class="sxs-lookup"><span data-stu-id="f45fd-266">deviceBlockEnableRestrictions</span></span>|<span data-ttu-id="f45fd-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-267">Boolean</span></span>|<span data-ttu-id="f45fd-268">デバイスが監視モードのときに、ユーザーがデバイス設定の制限を有効にできるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-268">Indicates whether or not to allow the user to enables restrictions in the device settings when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-269">deviceBlockEraseContentAndSettings</span><span class="sxs-lookup"><span data-stu-id="f45fd-269">deviceBlockEraseContentAndSettings</span></span>|<span data-ttu-id="f45fd-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-270">Boolean</span></span>|<span data-ttu-id="f45fd-271">デバイスが監視モードのときに、デバイスの [すべてのコンテンツと設定を消去] オプションの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-271">Indicates whether or not to allow the use of the 'Erase all content and settings' option on the device when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-272">deviceBlockNameModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-272">deviceBlockNameModification</span></span>|<span data-ttu-id="f45fd-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-273">Boolean</span></span>|<span data-ttu-id="f45fd-274">デバイスが監視モードのときに、デバイス名の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-274">Indicates whether or not to allow device name modification when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f45fd-275">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="f45fd-275">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="f45fd-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-276">Boolean</span></span>|<span data-ttu-id="f45fd-277">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-277">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="f45fd-278">diagnosticDataBlockSubmissionModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-278">diagnosticDataBlockSubmissionModification</span></span>|<span data-ttu-id="f45fd-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-279">Boolean</span></span>|<span data-ttu-id="f45fd-280">デバイスが監視モードのときに、診断の送信の設定変更を許可するかどうかを示します (iOS 9.3.2 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-280">Indicates whether or not to allow diagnostics submission settings modification when the device is in supervised mode (iOS 9.3.2 and later).</span></span>|
|<span data-ttu-id="f45fd-281">documentsBlockManagedDocumentsInUnmanagedApps</span><span class="sxs-lookup"><span data-stu-id="f45fd-281">documentsBlockManagedDocumentsInUnmanagedApps</span></span>|<span data-ttu-id="f45fd-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-282">Boolean</span></span>|<span data-ttu-id="f45fd-283">ユーザーによる非管理対象アプリでの管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-283">Indicates whether or not to block the user from viewing managed documents in unmanaged apps.</span></span>|
|<span data-ttu-id="f45fd-284">documentsBlockUnmanagedDocumentsInManagedApps</span><span class="sxs-lookup"><span data-stu-id="f45fd-284">documentsBlockUnmanagedDocumentsInManagedApps</span></span>|<span data-ttu-id="f45fd-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-285">Boolean</span></span>|<span data-ttu-id="f45fd-286">ユーザーによる管理対象アプリでの非管理対象ドキュメントの表示を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-286">Indicates whether or not to block the user from viewing unmanaged documents in managed apps.</span></span>|
|<span data-ttu-id="f45fd-287">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="f45fd-287">emailInDomainSuffixes</span></span>|<span data-ttu-id="f45fd-288">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f45fd-288">String collection</span></span>|<span data-ttu-id="f45fd-289">これらの文字列のいずれかに一致するサフィックスがないメール アドレスは、ドメイン外と見なされます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-289">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="f45fd-290">enterpriseAppBlockTrust</span><span class="sxs-lookup"><span data-stu-id="f45fd-290">enterpriseAppBlockTrust</span></span>|<span data-ttu-id="f45fd-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-291">Boolean</span></span>|<span data-ttu-id="f45fd-292">ユーザーによるエンタープライズ アプリの信頼を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-292">Indicates whether or not to block the user from trusting an enterprise app.</span></span>|
|<span data-ttu-id="f45fd-293">enterpriseAppBlockTrustModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-293">enterpriseAppBlockTrustModification</span></span>|<span data-ttu-id="f45fd-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-294">Boolean</span></span>|<span data-ttu-id="f45fd-295">ユーザーによるエンタープライズ アプリの信頼の設定の変更を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-295">Indicates whether or not to block the user from modifying the enterprise app trust settings.</span></span>|
|<span data-ttu-id="f45fd-296">faceTimeBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-296">faceTimeBlocked</span></span>|<span data-ttu-id="f45fd-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-297">Boolean</span></span>|<span data-ttu-id="f45fd-298">ユーザーによる FaceTime の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-298">Indicates whether or not to block the user from using FaceTime.</span></span>|
|<span data-ttu-id="f45fd-299">findMyFriendsBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-299">findMyFriendsBlocked</span></span>|<span data-ttu-id="f45fd-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-300">Boolean</span></span>|<span data-ttu-id="f45fd-301">デバイスが監視モードのときに、"友達を探す" をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-301">Indicates whether or not to block Find My Friends when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-302">gamingBlockGameCenterFriends</span><span class="sxs-lookup"><span data-stu-id="f45fd-302">gamingBlockGameCenterFriends</span></span>|<span data-ttu-id="f45fd-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-303">Boolean</span></span>|<span data-ttu-id="f45fd-304">ユーザーによる Game Center での友達の追加を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-304">Indicates whether or not to block the user from having friends in Game Center.</span></span>|
|<span data-ttu-id="f45fd-305">gamingBlockMultiplayer</span><span class="sxs-lookup"><span data-stu-id="f45fd-305">gamingBlockMultiplayer</span></span>|<span data-ttu-id="f45fd-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-306">Boolean</span></span>|<span data-ttu-id="f45fd-307">ユーザーによるマルチプレイヤー ゲームの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-307">Indicates whether or not to block the user from using multiplayer gaming.</span></span>|
|<span data-ttu-id="f45fd-308">gameCenterBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-308">gameCenterBlocked</span></span>|<span data-ttu-id="f45fd-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-309">Boolean</span></span>|<span data-ttu-id="f45fd-310">デバイスが監視モードのときに、ユーザーによる Game Center の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-310">Indicates whether or not to block the user from using Game Center when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-311">hostPairingBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-311">hostPairingBlocked</span></span>|<span data-ttu-id="f45fd-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-312">Boolean</span></span>|<span data-ttu-id="f45fd-313">iOS デバイスが監視モードのときに、iOS デバイスがペアリングできるデバイスをホスト ペアリングで制御できるようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-313">indicates whether or not to allow host pairing to control the devices an iOS device can pair with when the iOS device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-314">iBooksStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-314">iBooksStoreBlocked</span></span>|<span data-ttu-id="f45fd-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-315">Boolean</span></span>|<span data-ttu-id="f45fd-316">デバイスが監視モードのときに、ユーザーによる iBooks Store の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-316">Indicates whether or not to block the user from using the iBooks Store when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-317">iBooksStoreBlockErotica</span><span class="sxs-lookup"><span data-stu-id="f45fd-317">iBooksStoreBlockErotica</span></span>|<span data-ttu-id="f45fd-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-318">Boolean</span></span>|<span data-ttu-id="f45fd-319">アダルトのフラグが付いている iBookstore からのメディアのダウンロードをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-319">Indicates whether or not to block the user from downloading media from the iBookstore that has been tagged as erotica.</span></span>|
|<span data-ttu-id="f45fd-320">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="f45fd-320">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="f45fd-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-321">Boolean</span></span>|<span data-ttu-id="f45fd-322">iOS デバイスで起動した作業の、別の iOS デバイスまたは macOS デバイスでの継続実施をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-322">Indicates whether or not to block  the the user from continuing work they started on iOS device to another iOS or macOS device.</span></span>|
|<span data-ttu-id="f45fd-323">iCloudBlockBackup</span><span class="sxs-lookup"><span data-stu-id="f45fd-323">iCloudBlockBackup</span></span>|<span data-ttu-id="f45fd-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-324">Boolean</span></span>|<span data-ttu-id="f45fd-325">iCloud バックアップを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-325">Indicates whether or not to block iCloud backup.</span></span>|
|<span data-ttu-id="f45fd-326">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="f45fd-326">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="f45fd-327">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-327">Boolean</span></span>|<span data-ttu-id="f45fd-328">iCloud のドキュメントの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-328">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="f45fd-329">iCloudBlockManagedAppsSync</span><span class="sxs-lookup"><span data-stu-id="f45fd-329">iCloudBlockManagedAppsSync</span></span>|<span data-ttu-id="f45fd-330">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-330">Boolean</span></span>|<span data-ttu-id="f45fd-331">管理対象アプリのクラウドの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-331">Indicates whether or not to block Managed Apps Cloud Sync.</span></span>|
|<span data-ttu-id="f45fd-332">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="f45fd-332">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="f45fd-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-333">Boolean</span></span>|<span data-ttu-id="f45fd-334">iCloud フォト ライブラリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-334">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="f45fd-335">iCloudBlockPhotoStreamSync</span><span class="sxs-lookup"><span data-stu-id="f45fd-335">iCloudBlockPhotoStreamSync</span></span>|<span data-ttu-id="f45fd-336">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-336">Boolean</span></span>|<span data-ttu-id="f45fd-337">iCloud フォトのストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-337">Indicates whether or not to block iCloud Photo Stream Sync.</span></span>|
|<span data-ttu-id="f45fd-338">iCloudBlockSharedPhotoStream</span><span class="sxs-lookup"><span data-stu-id="f45fd-338">iCloudBlockSharedPhotoStream</span></span>|<span data-ttu-id="f45fd-339">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-339">Boolean</span></span>|<span data-ttu-id="f45fd-340">共有フォト ストリームの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-340">Indicates whether or not to block Shared Photo Stream.</span></span>|
|<span data-ttu-id="f45fd-341">iCloudRequireEncryptedBackup</span><span class="sxs-lookup"><span data-stu-id="f45fd-341">iCloudRequireEncryptedBackup</span></span>|<span data-ttu-id="f45fd-342">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-342">Boolean</span></span>|<span data-ttu-id="f45fd-343">iCloud のバックアップを暗号化する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-343">Indicates whether or not to require backups to iCloud be encrypted.</span></span>|
|<span data-ttu-id="f45fd-344">iTunesBlockExplicitContent</span><span class="sxs-lookup"><span data-stu-id="f45fd-344">iTunesBlockExplicitContent</span></span>|<span data-ttu-id="f45fd-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-345">Boolean</span></span>|<span data-ttu-id="f45fd-346">ユーザーによる iTunes および App Store の過激な描写のコンテンツへのアクセスをブロックするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-346">Indicates whether or not to block the user from accessing explicit content in iTunes and the App Store.</span></span>|
|<span data-ttu-id="f45fd-347">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="f45fd-347">iTunesBlockMusicService</span></span>|<span data-ttu-id="f45fd-348">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-348">Boolean</span></span>|<span data-ttu-id="f45fd-349">デバイスが監視モードのときに、Music サービスをブロックして Music アプリをクラシック モードに戻すかどうかを示します (iOS 9.3 以降および macOS 10.12 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-349">Indicates whether or not to block Music service and revert Music app to classic mode when the device is in supervised mode (iOS 9.3 and later and macOS 10.12 and later).</span></span>|
|<span data-ttu-id="f45fd-350">iTunesBlockRadio</span><span class="sxs-lookup"><span data-stu-id="f45fd-350">iTunesBlockRadio</span></span>|<span data-ttu-id="f45fd-351">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-351">Boolean</span></span>|<span data-ttu-id="f45fd-352">デバイスが監視モードのときに、ユーザーによる iTunes Radio の使用を禁止するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-352">Indicates whether or not to block the user from using iTunes Radio when the device is in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f45fd-353">keyboardBlockAutoCorrect</span><span class="sxs-lookup"><span data-stu-id="f45fd-353">keyboardBlockAutoCorrect</span></span>|<span data-ttu-id="f45fd-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-354">Boolean</span></span>|<span data-ttu-id="f45fd-355">デバイスが監視モードのときに、キーボードの自動修正を禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-355">Indicates whether or not to block keyboard auto-correction when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f45fd-356">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="f45fd-356">keyboardBlockDictation</span></span>|<span data-ttu-id="f45fd-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-357">Boolean</span></span>|<span data-ttu-id="f45fd-358">デバイスが監視モードのときに、ユーザーによるディクテーション入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-358">Indicates whether or not to block the user from using dictation input when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-359">keyboardBlockPredictive</span><span class="sxs-lookup"><span data-stu-id="f45fd-359">keyboardBlockPredictive</span></span>|<span data-ttu-id="f45fd-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-360">Boolean</span></span>|<span data-ttu-id="f45fd-361">デバイスが監視モードのときに、予測キーボードを禁止するかどうかを示します (iOS 8.1.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-361">Indicates whether or not to block predictive keyboards when device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f45fd-362">keyboardBlockShortcuts</span><span class="sxs-lookup"><span data-stu-id="f45fd-362">keyboardBlockShortcuts</span></span>|<span data-ttu-id="f45fd-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-363">Boolean</span></span>|<span data-ttu-id="f45fd-364">デバイスが監視モードのときに、キーボード ショートカットを禁止するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-364">Indicates whether or not to block keyboard shortcuts when the device is in supervised mode (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f45fd-365">keyboardBlockSpellCheck</span><span class="sxs-lookup"><span data-stu-id="f45fd-365">keyboardBlockSpellCheck</span></span>|<span data-ttu-id="f45fd-366">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-366">Boolean</span></span>|<span data-ttu-id="f45fd-367">デバイスが監視モードのときに、キーボードのスペル チェックを禁止するかどうかを示します (iOS 8.13 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-367">Indicates whether or not to block keyboard spell-checking when the device is in supervised mode (iOS 8.1.3 and later).</span></span>|
|<span data-ttu-id="f45fd-368">kioskModeAllowAssistiveSpeak</span><span class="sxs-lookup"><span data-stu-id="f45fd-368">kioskModeAllowAssistiveSpeak</span></span>|<span data-ttu-id="f45fd-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-369">Boolean</span></span>|<span data-ttu-id="f45fd-370">キオスク モード時の補助音声を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-370">Indicates whether or not to allow assistive speak while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-371">kioskModeAllowAssistiveTouchSettings</span><span class="sxs-lookup"><span data-stu-id="f45fd-371">kioskModeAllowAssistiveTouchSettings</span></span>|<span data-ttu-id="f45fd-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-372">Boolean</span></span>|<span data-ttu-id="f45fd-373">キオスク モード時の Assistive Touch の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-373">Indicates whether or not to allow access to the Assistive Touch Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-374">kioskModeAllowAutoLock</span><span class="sxs-lookup"><span data-stu-id="f45fd-374">kioskModeAllowAutoLock</span></span>|<span data-ttu-id="f45fd-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-375">Boolean</span></span>|<span data-ttu-id="f45fd-376">キオスク モード時のデバイスの自動ロックを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-376">Indicates whether or not to allow device auto lock while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-377">kioskModeAllowColorInversionSettings</span><span class="sxs-lookup"><span data-stu-id="f45fd-377">kioskModeAllowColorInversionSettings</span></span>|<span data-ttu-id="f45fd-378">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-378">Boolean</span></span>|<span data-ttu-id="f45fd-379">キオスク モード時の色反転の設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-379">Indicates whether or not to allow access to the Color Inversion Settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-380">kioskModeAllowRingerSwitch</span><span class="sxs-lookup"><span data-stu-id="f45fd-380">kioskModeAllowRingerSwitch</span></span>|<span data-ttu-id="f45fd-381">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-381">Boolean</span></span>|<span data-ttu-id="f45fd-382">キオスク モード時の着信音スイッチの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-382">Indicates whether or not to allow use of the ringer switch while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-383">kioskModeAllowScreenRotation</span><span class="sxs-lookup"><span data-stu-id="f45fd-383">kioskModeAllowScreenRotation</span></span>|<span data-ttu-id="f45fd-384">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-384">Boolean</span></span>|<span data-ttu-id="f45fd-385">キオスク モード時の画面の回転を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-385">Indicates whether or not to allow screen rotation while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-386">kioskModeAllowSleepButton</span><span class="sxs-lookup"><span data-stu-id="f45fd-386">kioskModeAllowSleepButton</span></span>|<span data-ttu-id="f45fd-387">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-387">Boolean</span></span>|<span data-ttu-id="f45fd-388">キオスク モード時のスリープ ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-388">Indicates whether or not to allow use of the sleep button while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-389">kioskModeAllowTouchscreen</span><span class="sxs-lookup"><span data-stu-id="f45fd-389">kioskModeAllowTouchscreen</span></span>|<span data-ttu-id="f45fd-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-390">Boolean</span></span>|<span data-ttu-id="f45fd-391">キオスク モード時のタッチスクリーンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-391">Indicates whether or not to allow use of the touchscreen while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-392">kioskModeAllowVoiceOverSettings</span><span class="sxs-lookup"><span data-stu-id="f45fd-392">kioskModeAllowVoiceOverSettings</span></span>|<span data-ttu-id="f45fd-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-393">Boolean</span></span>|<span data-ttu-id="f45fd-394">キオスク モード時のボイス オーバーの設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-394">Indicates whether or not to allow access to the voice over settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-395">kioskModeAllowVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="f45fd-395">kioskModeAllowVolumeButtons</span></span>|<span data-ttu-id="f45fd-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-396">Boolean</span></span>|<span data-ttu-id="f45fd-397">キオスク モード時のボリューム ボタンの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-397">Indicates whether or not to allow use of the volume buttons while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-398">kioskModeBlockVolumeButtons</span><span class="sxs-lookup"><span data-stu-id="f45fd-398">kioskModeBlockVolumeButtons</span></span>|<span data-ttu-id="f45fd-399">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-399">Boolean</span></span>|<span data-ttu-id="f45fd-400">キオスク モード中にボリューム ボタンをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-400">Indicates whether or not to block the volume buttons while in Kiosk Mode.</span></span>|
|<span data-ttu-id="f45fd-401">kioskModeAllowZoomSettings</span><span class="sxs-lookup"><span data-stu-id="f45fd-401">kioskModeAllowZoomSettings</span></span>|<span data-ttu-id="f45fd-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-402">Boolean</span></span>|<span data-ttu-id="f45fd-403">キオスク モード時のズーム設定へのアクセスを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-403">Indicates whether or not to allow access to the zoom settings while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-404">kioskModeAppStoreUrl</span><span class="sxs-lookup"><span data-stu-id="f45fd-404">kioskModeAppStoreUrl</span></span>|<span data-ttu-id="f45fd-405">String</span><span class="sxs-lookup"><span data-stu-id="f45fd-405">String</span></span>|<span data-ttu-id="f45fd-406">キオスク モード用に使用するアプリへの、App Store 内の URL。</span><span class="sxs-lookup"><span data-stu-id="f45fd-406">URL in the app store to the app to use for kiosk mode.</span></span> <span data-ttu-id="f45fd-407">KioskModeManagedAppId が不明な場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-407">Use if KioskModeManagedAppId is not known.</span></span>|
|<span data-ttu-id="f45fd-408">kioskModeBuiltInAppId</span><span class="sxs-lookup"><span data-stu-id="f45fd-408">kioskModeBuiltInAppId</span></span>|<span data-ttu-id="f45fd-409">String</span><span class="sxs-lookup"><span data-stu-id="f45fd-409">String</span></span>|<span data-ttu-id="f45fd-410">キオスク モードを使用する組み込みアプリケーションの ID です。</span><span class="sxs-lookup"><span data-stu-id="f45fd-410">ID for built-in apps to use for kiosk mode.</span></span> <span data-ttu-id="f45fd-411">KioskModeManagedAppId と KioskModeAppStoreUrl が設定されていない場合に使用します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-411">Used when KioskModeManagedAppId and KioskModeAppStoreUrl are not set.</span></span>|
|<span data-ttu-id="f45fd-412">kioskModeRequireAssistiveTouch</span><span class="sxs-lookup"><span data-stu-id="f45fd-412">kioskModeRequireAssistiveTouch</span></span>|<span data-ttu-id="f45fd-413">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-413">Boolean</span></span>|<span data-ttu-id="f45fd-414">キオスク モード時に Assistive Touch が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-414">Indicates whether or not to require assistive touch while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-415">kioskModeRequireColorInversion</span><span class="sxs-lookup"><span data-stu-id="f45fd-415">kioskModeRequireColorInversion</span></span>|<span data-ttu-id="f45fd-416">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-416">Boolean</span></span>|<span data-ttu-id="f45fd-417">キオスク モード時に色反転が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-417">Indicates whether or not to require color inversion while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-418">kioskModeRequireMonoAudio</span><span class="sxs-lookup"><span data-stu-id="f45fd-418">kioskModeRequireMonoAudio</span></span>|<span data-ttu-id="f45fd-419">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-419">Boolean</span></span>|<span data-ttu-id="f45fd-420">キオスク モード時にモノラル オーディオが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-420">Indicates whether or not to require mono audio while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-421">kioskModeRequireVoiceOver</span><span class="sxs-lookup"><span data-stu-id="f45fd-421">kioskModeRequireVoiceOver</span></span>|<span data-ttu-id="f45fd-422">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-422">Boolean</span></span>|<span data-ttu-id="f45fd-423">キオスク モード時にボイス オーバーが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-423">Indicates whether or not to require voice over while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-424">kioskModeRequireZoom</span><span class="sxs-lookup"><span data-stu-id="f45fd-424">kioskModeRequireZoom</span></span>|<span data-ttu-id="f45fd-425">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-425">Boolean</span></span>|<span data-ttu-id="f45fd-426">キオスク モード時にズームが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-426">Indicates whether or not to require zoom while in kiosk mode.</span></span>|
|<span data-ttu-id="f45fd-427">kioskModeManagedAppId</span><span class="sxs-lookup"><span data-stu-id="f45fd-427">kioskModeManagedAppId</span></span>|<span data-ttu-id="f45fd-428">String</span><span class="sxs-lookup"><span data-stu-id="f45fd-428">String</span></span>|<span data-ttu-id="f45fd-429">キオスク モード用に使用するアプリの管理対象アプリ ID。</span><span class="sxs-lookup"><span data-stu-id="f45fd-429">Managed app id of the app to use for kiosk mode.</span></span> <span data-ttu-id="f45fd-430">KioskModeManagedAppId が指定されている場合は、KioskModeAppStoreUrl は無視されます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-430">If KioskModeManagedAppId is specified then KioskModeAppStoreUrl will be ignored.</span></span>|
|<span data-ttu-id="f45fd-431">lockScreenBlockControlCenter</span><span class="sxs-lookup"><span data-stu-id="f45fd-431">lockScreenBlockControlCenter</span></span>|<span data-ttu-id="f45fd-432">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-432">Boolean</span></span>|<span data-ttu-id="f45fd-433">ユーザーによるロック画面でのコントロール センターの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-433">Indicates whether or not to block the user from using control center on the lock screen.</span></span>|
|<span data-ttu-id="f45fd-434">lockScreenBlockNotificationView</span><span class="sxs-lookup"><span data-stu-id="f45fd-434">lockScreenBlockNotificationView</span></span>|<span data-ttu-id="f45fd-435">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-435">Boolean</span></span>|<span data-ttu-id="f45fd-436">ユーザーによるロック画面での通知ビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-436">Indicates whether or not to block the user from using the notification view on the lock screen.</span></span>|
|<span data-ttu-id="f45fd-437">lockScreenBlockPassbook</span><span class="sxs-lookup"><span data-stu-id="f45fd-437">lockScreenBlockPassbook</span></span>|<span data-ttu-id="f45fd-438">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-438">Boolean</span></span>|<span data-ttu-id="f45fd-439">デバイスがロックされているときに、ユーザーによる Passbook の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-439">Indicates whether or not to block the user from using passbook when the device is locked.</span></span>|
|<span data-ttu-id="f45fd-440">lockScreenBlockTodayView</span><span class="sxs-lookup"><span data-stu-id="f45fd-440">lockScreenBlockTodayView</span></span>|<span data-ttu-id="f45fd-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-441">Boolean</span></span>|<span data-ttu-id="f45fd-442">ユーザーによるロック画面での本日のビューの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-442">Indicates whether or not to block the user from using the Today View on the lock screen.</span></span>|
|<span data-ttu-id="f45fd-443">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="f45fd-443">mediaContentRatingAustralia</span></span>|[<span data-ttu-id="f45fd-444">mediaContentRatingAustralia</span><span class="sxs-lookup"><span data-stu-id="f45fd-444">mediaContentRatingAustralia</span></span>](../resources/intune-deviceconfig-mediacontentratingaustralia.md)|<span data-ttu-id="f45fd-445">メディア コンテンツの評価の設定 (オーストラリア向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-445">Media content rating settings for Australia</span></span>|
|<span data-ttu-id="f45fd-446">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="f45fd-446">mediaContentRatingCanada</span></span>|[<span data-ttu-id="f45fd-447">mediaContentRatingCanada</span><span class="sxs-lookup"><span data-stu-id="f45fd-447">mediaContentRatingCanada</span></span>](../resources/intune-deviceconfig-mediacontentratingcanada.md)|<span data-ttu-id="f45fd-448">メディア コンテンツの評価の設定 (カナダ向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-448">Media content rating settings for Canada</span></span>|
|<span data-ttu-id="f45fd-449">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f45fd-449">mediaContentRatingFrance</span></span>|[<span data-ttu-id="f45fd-450">mediaContentRatingFrance</span><span class="sxs-lookup"><span data-stu-id="f45fd-450">mediaContentRatingFrance</span></span>](../resources/intune-deviceconfig-mediacontentratingfrance.md)|<span data-ttu-id="f45fd-451">メディア コンテンツの評価の設定 (フランス向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-451">Media content rating settings for France</span></span>|
|<span data-ttu-id="f45fd-452">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="f45fd-452">mediaContentRatingGermany</span></span>|[<span data-ttu-id="f45fd-453">mediaContentRatingGermany</span><span class="sxs-lookup"><span data-stu-id="f45fd-453">mediaContentRatingGermany</span></span>](../resources/intune-deviceconfig-mediacontentratinggermany.md)|<span data-ttu-id="f45fd-454">メディア コンテンツの評価の設定 (ドイツ向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-454">Media content rating settings for Germany</span></span>|
|<span data-ttu-id="f45fd-455">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="f45fd-455">mediaContentRatingIreland</span></span>|[<span data-ttu-id="f45fd-456">mediaContentRatingIreland</span><span class="sxs-lookup"><span data-stu-id="f45fd-456">mediaContentRatingIreland</span></span>](../resources/intune-deviceconfig-mediacontentratingireland.md)|<span data-ttu-id="f45fd-457">メディア コンテンツの評価の設定 (アイルランド向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-457">Media content rating settings for Ireland</span></span>|
|<span data-ttu-id="f45fd-458">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="f45fd-458">mediaContentRatingJapan</span></span>|[<span data-ttu-id="f45fd-459">mediaContentRatingJapan</span><span class="sxs-lookup"><span data-stu-id="f45fd-459">mediaContentRatingJapan</span></span>](../resources/intune-deviceconfig-mediacontentratingjapan.md)|<span data-ttu-id="f45fd-460">メディア コンテンツの評価の設定 (日本向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-460">Media content rating settings for Japan</span></span>|
|<span data-ttu-id="f45fd-461">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="f45fd-461">mediaContentRatingNewZealand</span></span>|[<span data-ttu-id="f45fd-462">mediaContentRatingNewZealand</span><span class="sxs-lookup"><span data-stu-id="f45fd-462">mediaContentRatingNewZealand</span></span>](../resources/intune-deviceconfig-mediacontentratingnewzealand.md)|<span data-ttu-id="f45fd-463">メディア コンテンツの評価の設定 (ニュージーランド向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-463">Media content rating settings for New Zealand</span></span>|
|<span data-ttu-id="f45fd-464">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f45fd-464">mediaContentRatingUnitedKingdom</span></span>|[<span data-ttu-id="f45fd-465">mediaContentRatingUnitedKingdom</span><span class="sxs-lookup"><span data-stu-id="f45fd-465">mediaContentRatingUnitedKingdom</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedkingdom.md)|<span data-ttu-id="f45fd-466">メディア コンテンツの評価の設定 (英国向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-466">Media content rating settings for United Kingdom</span></span>|
|<span data-ttu-id="f45fd-467">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="f45fd-467">mediaContentRatingUnitedStates</span></span>|[<span data-ttu-id="f45fd-468">mediaContentRatingUnitedStates</span><span class="sxs-lookup"><span data-stu-id="f45fd-468">mediaContentRatingUnitedStates</span></span>](../resources/intune-deviceconfig-mediacontentratingunitedstates.md)|<span data-ttu-id="f45fd-469">メディア コンテンツの評価の設定 (米国向け)</span><span class="sxs-lookup"><span data-stu-id="f45fd-469">Media content rating settings for United States</span></span>|
|<span data-ttu-id="f45fd-470">networkUsageRules</span><span class="sxs-lookup"><span data-stu-id="f45fd-470">networkUsageRules</span></span>|<span data-ttu-id="f45fd-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="f45fd-471">[iosNetworkUsageRule](../resources/intune-deviceconfig-iosnetworkusagerule.md) collection</span></span>|<span data-ttu-id="f45fd-472">管理対象アプリと、それらに適用されるネットワーク ルールのリストです。</span><span class="sxs-lookup"><span data-stu-id="f45fd-472">List of managed apps and the network rules that applies to them.</span></span> <span data-ttu-id="f45fd-473">このコレクションには、最大で 1000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-473">This collection can contain a maximum of 1000 elements.</span></span>|
|<span data-ttu-id="f45fd-474">mediaContentRatingApps</span><span class="sxs-lookup"><span data-stu-id="f45fd-474">mediaContentRatingApps</span></span>|[<span data-ttu-id="f45fd-475">ratingAppsType</span><span class="sxs-lookup"><span data-stu-id="f45fd-475">ratingAppsType</span></span>](../resources/intune-deviceconfig-ratingappstype.md)|<span data-ttu-id="f45fd-476">メディア コンテンツのアプリケーションの設定を評価します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-476">Media content rating settings for Apps.</span></span> <span data-ttu-id="f45fd-477">使用可能な値: `allAllowed`、`allBlocked`、`agesAbove4`、`agesAbove9`、`agesAbove12`、`agesAbove17`。</span><span class="sxs-lookup"><span data-stu-id="f45fd-477">Possible values are: `allAllowed`, `allBlocked`, `agesAbove4`, `agesAbove9`, `agesAbove12`, `agesAbove17`.</span></span>|
|<span data-ttu-id="f45fd-478">messagesBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-478">messagesBlocked</span></span>|<span data-ttu-id="f45fd-479">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-479">Boolean</span></span>|<span data-ttu-id="f45fd-480">ユーザーによる監視対象デバイスでのメッセージ アプリの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-480">Indicates whether or not to block the user from using the Messages app on the supervised device.</span></span>|
|<span data-ttu-id="f45fd-481">notificationsBlockSettingsModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-481">notificationsBlockSettingsModification</span></span>|<span data-ttu-id="f45fd-482">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-482">Boolean</span></span>|<span data-ttu-id="f45fd-483">通知の設定の変更を許可するかどうかを示します (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-483">Indicates whether or not to allow notifications settings modification (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f45fd-484">passcodeBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f45fd-484">passcodeBlockFingerprintUnlock</span></span>|<span data-ttu-id="f45fd-485">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-485">Boolean</span></span>|<span data-ttu-id="f45fd-486">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-486">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="f45fd-487">passcodeBlockFingerprintModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-487">passcodeBlockFingerprintModification</span></span>|<span data-ttu-id="f45fd-488">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-488">Boolean</span></span>|<span data-ttu-id="f45fd-489">監視モードの際の、登録済みの Touch ID の指紋認証の修正を禁止します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-489">Block modification of registered Touch ID fingerprints when in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-490">passcodeBlockModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-490">passcodeBlockModification</span></span>|<span data-ttu-id="f45fd-491">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-491">Boolean</span></span>|<span data-ttu-id="f45fd-492">監視対象デバイスでのパスコードの変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-492">Indicates whether or not to allow passcode modification on the supervised device (iOS 9.0 and later).</span></span>|
|<span data-ttu-id="f45fd-493">passcodeBlockSimple</span><span class="sxs-lookup"><span data-stu-id="f45fd-493">passcodeBlockSimple</span></span>|<span data-ttu-id="f45fd-494">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-494">Boolean</span></span>|<span data-ttu-id="f45fd-495">単純なパスコードを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-495">Indicates whether or not to block simple passcodes.</span></span>|
|<span data-ttu-id="f45fd-496">passcodeExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f45fd-496">passcodeExpirationDays</span></span>|<span data-ttu-id="f45fd-497">Int32</span><span class="sxs-lookup"><span data-stu-id="f45fd-497">Int32</span></span>|<span data-ttu-id="f45fd-498">パスコードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="f45fd-498">Number of days before the passcode expires.</span></span> <span data-ttu-id="f45fd-499">有効な値は 1 から 65535 までです</span><span class="sxs-lookup"><span data-stu-id="f45fd-499">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="f45fd-500">passcodeMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f45fd-500">passcodeMinimumLength</span></span>|<span data-ttu-id="f45fd-501">Int32</span><span class="sxs-lookup"><span data-stu-id="f45fd-501">Int32</span></span>|<span data-ttu-id="f45fd-502">パスコードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="f45fd-502">Minimum length of passcode.</span></span> <span data-ttu-id="f45fd-503">有効な値は 4 から 14 までです</span><span class="sxs-lookup"><span data-stu-id="f45fd-503">Valid values 4 to 14</span></span>|
|<span data-ttu-id="f45fd-504">passcodeMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="f45fd-504">passcodeMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="f45fd-505">Int32</span><span class="sxs-lookup"><span data-stu-id="f45fd-505">Int32</span></span>|<span data-ttu-id="f45fd-506">パスコードが要求されるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-506">Minutes of inactivity before a passcode is required.</span></span>|
|<span data-ttu-id="f45fd-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f45fd-507">passcodeMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f45fd-508">Int32</span><span class="sxs-lookup"><span data-stu-id="f45fd-508">Int32</span></span>|<span data-ttu-id="f45fd-509">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-509">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f45fd-510">passcodeMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="f45fd-510">passcodeMinimumCharacterSetCount</span></span>|<span data-ttu-id="f45fd-511">Int32</span><span class="sxs-lookup"><span data-stu-id="f45fd-511">Int32</span></span>|<span data-ttu-id="f45fd-512">パスコードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="f45fd-512">Number of character sets a passcode must contain.</span></span> <span data-ttu-id="f45fd-513">有効な値は 0 から 4 までです</span><span class="sxs-lookup"><span data-stu-id="f45fd-513">Valid values 0 to 4</span></span>|
|<span data-ttu-id="f45fd-514">passcodePreviousPasscodeBlockCount</span><span class="sxs-lookup"><span data-stu-id="f45fd-514">passcodePreviousPasscodeBlockCount</span></span>|<span data-ttu-id="f45fd-515">Int32</span><span class="sxs-lookup"><span data-stu-id="f45fd-515">Int32</span></span>|<span data-ttu-id="f45fd-516">ブロックする、以前のパスコードの数。</span><span class="sxs-lookup"><span data-stu-id="f45fd-516">Number of previous passcodes to block.</span></span> <span data-ttu-id="f45fd-517">有効な値は 1 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="f45fd-517">Valid values 1 to 24</span></span>|
|<span data-ttu-id="f45fd-518">passcodeSignInFailureCountBeforeWipe</span><span class="sxs-lookup"><span data-stu-id="f45fd-518">passcodeSignInFailureCountBeforeWipe</span></span>|<span data-ttu-id="f45fd-519">Int32</span><span class="sxs-lookup"><span data-stu-id="f45fd-519">Int32</span></span>|<span data-ttu-id="f45fd-520">デバイスをワイプするまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="f45fd-520">Number of sign in failures allowed before wiping the device.</span></span> <span data-ttu-id="f45fd-521">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="f45fd-521">Valid values 4 to 11</span></span>|
|<span data-ttu-id="f45fd-522">passcodeRequiredType</span><span class="sxs-lookup"><span data-stu-id="f45fd-522">passcodeRequiredType</span></span>|[<span data-ttu-id="f45fd-523">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f45fd-523">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="f45fd-524">必要なパスコードの種類。</span><span class="sxs-lookup"><span data-stu-id="f45fd-524">Type of passcode that is required.</span></span> <span data-ttu-id="f45fd-525">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="f45fd-525">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="f45fd-526">passcodeRequired</span><span class="sxs-lookup"><span data-stu-id="f45fd-526">passcodeRequired</span></span>|<span data-ttu-id="f45fd-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-527">Boolean</span></span>|<span data-ttu-id="f45fd-528">パスコードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-528">Indicates whether or not to require a passcode.</span></span>|
|<span data-ttu-id="f45fd-529">podcastsBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-529">podcastsBlocked</span></span>|<span data-ttu-id="f45fd-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-530">Boolean</span></span>|<span data-ttu-id="f45fd-531">ユーザーによる監視対象デバイスでのポッドキャストの使用を禁止するかどうかを示します (iOS 8.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-531">Indicates whether or not to block the user from using podcasts on the supervised device (iOS 8.0 and later).</span></span>|
|<span data-ttu-id="f45fd-532">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="f45fd-532">safariBlockAutofill</span></span>|<span data-ttu-id="f45fd-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-533">Boolean</span></span>|<span data-ttu-id="f45fd-534">ユーザーによる Safari での自動入力の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-534">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="f45fd-535">safariBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="f45fd-535">safariBlockJavaScript</span></span>|<span data-ttu-id="f45fd-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-536">Boolean</span></span>|<span data-ttu-id="f45fd-537">Safari 内で JavaScript をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-537">Indicates whether or not to block JavaScript in Safari.</span></span>|
|<span data-ttu-id="f45fd-538">safariBlockPopups</span><span class="sxs-lookup"><span data-stu-id="f45fd-538">safariBlockPopups</span></span>|<span data-ttu-id="f45fd-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-539">Boolean</span></span>|<span data-ttu-id="f45fd-540">Safari 内でポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-540">Indicates whether or not to block popups in Safari.</span></span>|
|<span data-ttu-id="f45fd-541">safariBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-541">safariBlocked</span></span>|<span data-ttu-id="f45fd-542">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-542">Boolean</span></span>|<span data-ttu-id="f45fd-543">ユーザーによる Safari の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-543">Indicates whether or not to block the user from using Safari.</span></span>|
|<span data-ttu-id="f45fd-544">safariCookieSettings</span><span class="sxs-lookup"><span data-stu-id="f45fd-544">safariCookieSettings</span></span>|[<span data-ttu-id="f45fd-545">webBrowserCookieSettings</span><span class="sxs-lookup"><span data-stu-id="f45fd-545">webBrowserCookieSettings</span></span>](../resources/intune-deviceconfig-webbrowsercookiesettings.md)|<span data-ttu-id="f45fd-546">Safari の Cookie の設定。</span><span class="sxs-lookup"><span data-stu-id="f45fd-546">Cookie settings for Safari.</span></span> <span data-ttu-id="f45fd-547">可能な値は、`browserDefault`、`blockAlways`、`allowCurrentWebSite`、`allowFromWebsitesVisited`、`allowAlways` です。</span><span class="sxs-lookup"><span data-stu-id="f45fd-547">Possible values are: `browserDefault`, `blockAlways`, `allowCurrentWebSite`, `allowFromWebsitesVisited`, `allowAlways`.</span></span>|
|<span data-ttu-id="f45fd-548">safariManagedDomains</span><span class="sxs-lookup"><span data-stu-id="f45fd-548">safariManagedDomains</span></span>|<span data-ttu-id="f45fd-549">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f45fd-549">String collection</span></span>|<span data-ttu-id="f45fd-550">ここに記載されているパターンに一致する URL は管理対象と見なされます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-550">URLs matching the patterns listed here will be considered managed.</span></span>|
|<span data-ttu-id="f45fd-551">safariPasswordAutoFillDomains</span><span class="sxs-lookup"><span data-stu-id="f45fd-551">safariPasswordAutoFillDomains</span></span>|<span data-ttu-id="f45fd-552">String コレクション</span><span class="sxs-lookup"><span data-stu-id="f45fd-552">String collection</span></span>|<span data-ttu-id="f45fd-553">ユーザーは、ここに記載されているパターンに一致する URL からのみ、パスワードを Safari に保存できます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-553">Users can save passwords in Safari only from URLs matching the patterns listed here.</span></span> <span data-ttu-id="f45fd-554">監視モードのデバイスに適用されます (iOS 9.3 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-554">Applies to devices in supervised mode (iOS 9.3 and later).</span></span>|
|<span data-ttu-id="f45fd-555">safariRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="f45fd-555">safariRequireFraudWarning</span></span>|<span data-ttu-id="f45fd-556">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-556">Boolean</span></span>|<span data-ttu-id="f45fd-557">Safari での不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-557">Indicates whether or not to require fraud warning in Safari.</span></span>|
|<span data-ttu-id="f45fd-558">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-558">screenCaptureBlocked</span></span>|<span data-ttu-id="f45fd-559">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-559">Boolean</span></span>|<span data-ttu-id="f45fd-560">ユーザーがスクリーンショットを撮ることを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-560">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="f45fd-561">siriBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-561">siriBlocked</span></span>|<span data-ttu-id="f45fd-562">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-562">Boolean</span></span>|<span data-ttu-id="f45fd-563">ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-563">Indicates whether or not to block the user from using Siri.</span></span>|
|<span data-ttu-id="f45fd-564">siriBlockedWhenLocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-564">siriBlockedWhenLocked</span></span>|<span data-ttu-id="f45fd-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-565">Boolean</span></span>|<span data-ttu-id="f45fd-566">ロックされている場合に、ユーザーによる Siri の使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-566">Indicates whether or not to block the user from using Siri when locked.</span></span>|
|<span data-ttu-id="f45fd-567">siriBlockUserGeneratedContent</span><span class="sxs-lookup"><span data-stu-id="f45fd-567">siriBlockUserGeneratedContent</span></span>|<span data-ttu-id="f45fd-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-568">Boolean</span></span>|<span data-ttu-id="f45fd-569">監視対象デバイスでの使用時に、Siri による、ユーザー生成コンテンツに対するクエリの実行をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-569">Indicates whether or not to block Siri from querying user-generated content when used on a supervised device.</span></span>|
|<span data-ttu-id="f45fd-570">siriRequireProfanityFilter</span><span class="sxs-lookup"><span data-stu-id="f45fd-570">siriRequireProfanityFilter</span></span>|<span data-ttu-id="f45fd-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-571">Boolean</span></span>|<span data-ttu-id="f45fd-572">Siri が監視対象デバイスで不適切な言葉をディクテーションまたは読み上げないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-572">Indicates whether or not to prevent Siri from dictating, or speaking profane language on supervised device.</span></span>|
|<span data-ttu-id="f45fd-573">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="f45fd-573">spotlightBlockInternetResults</span></span>|<span data-ttu-id="f45fd-574">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-574">Boolean</span></span>|<span data-ttu-id="f45fd-575">監視対象デバイスで Spotlight 検索がインターネットでの結果を返すのをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-575">Indicates whether or not to block Spotlight search from returning internet results on supervised device.</span></span>|
|<span data-ttu-id="f45fd-576">voiceDialingBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-576">voiceDialingBlocked</span></span>|<span data-ttu-id="f45fd-577">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-577">Boolean</span></span>|<span data-ttu-id="f45fd-578">音声ダイヤルをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-578">Indicates whether or not to block voice dialing.</span></span>|
|<span data-ttu-id="f45fd-579">wallpaperBlockModification</span><span class="sxs-lookup"><span data-stu-id="f45fd-579">wallpaperBlockModification</span></span>|<span data-ttu-id="f45fd-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-580">Boolean</span></span>|<span data-ttu-id="f45fd-581">監視対象デバイスでの壁紙の変更を許可するかどうかを示します (iOS 9.0 以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-581">Indicates whether or not to allow wallpaper modification on supervised device (iOS 9.0 and later) .</span></span>|
|<span data-ttu-id="f45fd-582">wiFiConnectOnlyToConfiguredNetworks</span><span class="sxs-lookup"><span data-stu-id="f45fd-582">wiFiConnectOnlyToConfiguredNetworks</span></span>|<span data-ttu-id="f45fd-583">Boolean</span><span class="sxs-lookup"><span data-stu-id="f45fd-583">Boolean</span></span>|<span data-ttu-id="f45fd-584">デバイスが監視モードのときに、構成プロファイルからの Wi-Fi ネットワークのみを使用するようデバイスに強制するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-584">Indicates whether or not to force the device to use only Wi-Fi networks from configuration profiles when the device is in supervised mode.</span></span>|
|<span data-ttu-id="f45fd-585">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="f45fd-585">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="f45fd-586">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-586">Boolean</span></span>|<span data-ttu-id="f45fd-587">かどうか、受講者用の教室を使用してアンマネージのコースに登録されているアクセス許可を要求、教師コース (iOS 11.3 とそれ以降) のままにしようとしていますを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-587">Indicates whether a student enrolled in an unmanaged course via Classroom will request permission from the teacher when attempting to leave the course (iOS 11.3 and later).</span></span>|
|<span data-ttu-id="f45fd-588">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="f45fd-588">keychainBlockCloudSync</span></span>|<span data-ttu-id="f45fd-589">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-589">Boolean</span></span>|<span data-ttu-id="f45fd-590">ICloud キーチェーンの同期をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-590">Indicates whether or not iCloud keychain synchronization is blocked.</span></span>|
|<span data-ttu-id="f45fd-591">pkiBlockOTAUpdates</span><span class="sxs-lookup"><span data-stu-id="f45fd-591">pkiBlockOTAUpdates</span></span>|<span data-ttu-id="f45fd-592">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-592">Boolean</span></span>|<span data-ttu-id="f45fd-593">地上の PKI の更新プログラムがブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-593">Indicates whether or not over-the-air PKI updates are blocked.</span></span> <span data-ttu-id="f45fd-594">False の場合、CRL および OCSP のチェック (iOS 7.0 およびそれ以降) は無効に、この制限を設定します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-594">Setting this restriction to false does not disable CRL and OCSP checks (iOS 7.0 and later).</span></span>|
|<span data-ttu-id="f45fd-595">privacyForceLimitAdTracking</span><span class="sxs-lookup"><span data-stu-id="f45fd-595">privacyForceLimitAdTracking</span></span>|<span data-ttu-id="f45fd-596">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-596">Boolean</span></span>|<span data-ttu-id="f45fd-597">広告の追跡が限られたかどうかを示します。(iOS から 7.0 およびそれ以降)。</span><span class="sxs-lookup"><span data-stu-id="f45fd-597">Indicates if ad tracking is limited.(iOS 7.0 and later).</span></span>|
|<span data-ttu-id="f45fd-598">enterpriseBookBlockBackup</span><span class="sxs-lookup"><span data-stu-id="f45fd-598">enterpriseBookBlockBackup</span></span>|<span data-ttu-id="f45fd-599">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-599">Boolean</span></span>|<span data-ttu-id="f45fd-600">企業がバックアップを予約するかどうかがブロックされていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-600">Indicates whether or not Enterprise book back up is blocked.</span></span>|
|<span data-ttu-id="f45fd-601">enterpriseBookBlockMetadataSync</span><span class="sxs-lookup"><span data-stu-id="f45fd-601">enterpriseBookBlockMetadataSync</span></span>|<span data-ttu-id="f45fd-602">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-602">Boolean</span></span>|<span data-ttu-id="f45fd-603">エンタープライズ帳に関する注意事項を示し、同期がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-603">Indicates whether or not Enterprise book notes and highlights sync is blocked.</span></span>|
|<span data-ttu-id="f45fd-604">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="f45fd-604">airPrintBlocked</span></span>|<span data-ttu-id="f45fd-605">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-605">Boolean</span></span>|<span data-ttu-id="f45fd-606">AirPrint がブロックされている (iOS 11.0 とそれ以降) であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-606">Indicates whether or not AirPrint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f45fd-607">airPrintBlockCredentialsStorage</span><span class="sxs-lookup"><span data-stu-id="f45fd-607">airPrintBlockCredentialsStorage</span></span>|<span data-ttu-id="f45fd-608">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-608">Boolean</span></span>|<span data-ttu-id="f45fd-609">ユーザー名とパスワードの Airprint のキーチェーンの記憶域がブロックされている (iOS 11.0 とそれ以降) かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-609">Indicates whether or not keychain storage of username and password for Airprint is blocked (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f45fd-610">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="f45fd-610">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="f45fd-611">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-611">Boolean</span></span>|<span data-ttu-id="f45fd-612">信頼された証明書が TLS 印刷通信 (iOS 11.0 とそれ以降) に必要なかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-612">Indicates if trusted certificates are required for TLS printing communication (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f45fd-613">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="f45fd-613">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="f45fd-614">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-614">Boolean</span></span>|<span data-ttu-id="f45fd-615">AirPrint プリンターの検出を iBeacon がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-615">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="f45fd-616">これには、ネットワーク トラフィック (iOS 11.0 とそれ以降) のフィッシング詐欺からの見かけ上の AirPrint Bluetooth ビーコンができなくなります。</span><span class="sxs-lookup"><span data-stu-id="f45fd-616">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f45fd-617">blockSystemAppRemoval</span><span class="sxs-lookup"><span data-stu-id="f45fd-617">blockSystemAppRemoval</span></span>|<span data-ttu-id="f45fd-618">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-618">Boolean</span></span>|<span data-ttu-id="f45fd-619">コールを管理デバイス (iOS 11.0 とそれ以降) で、デバイスからシステムのアプリケーションの削除がブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-619">Indicates whether or not the removal of system apps from the device is blocked on a supervised device (iOS 11.0 and later).</span></span>|
|<span data-ttu-id="f45fd-620">vpnBlockCreation</span><span class="sxs-lookup"><span data-stu-id="f45fd-620">vpnBlockCreation</span></span>|<span data-ttu-id="f45fd-621">ブール型</span><span class="sxs-lookup"><span data-stu-id="f45fd-621">Boolean</span></span>|<span data-ttu-id="f45fd-622">VPN 構成の作成がブロックされている (iOS 11.0 とそれ以降) であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-622">Indicates whether or not the creation of VPN configurations is blocked (iOS 11.0 and later).</span></span>|



## <a name="response"></a><span data-ttu-id="f45fd-623">応答</span><span class="sxs-lookup"><span data-stu-id="f45fd-623">Response</span></span>
<span data-ttu-id="f45fd-624">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f45fd-624">If successful, this method returns a `200 OK` response code and an updated [iosGeneralDeviceConfiguration](../resources/intune-deviceconfig-iosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f45fd-625">例</span><span class="sxs-lookup"><span data-stu-id="f45fd-625">Example</span></span>
### <a name="request"></a><span data-ttu-id="f45fd-626">要求</span><span class="sxs-lookup"><span data-stu-id="f45fd-626">Request</span></span>
<span data-ttu-id="f45fd-627">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f45fd-627">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 8428

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "vpnBlockCreation": true
}
```

### <a name="response"></a><span data-ttu-id="f45fd-628">応答</span><span class="sxs-lookup"><span data-stu-id="f45fd-628">Response</span></span>
<span data-ttu-id="f45fd-p132">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f45fd-p132">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 8604

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
  "vpnBlockCreation": true
}
```





