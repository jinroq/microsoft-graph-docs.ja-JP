---
title: Update windowsPhone81GeneralConfiguration
description: windowsPhone81GeneralConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3e8f0aa1c3ba924769bec41231019f76739b23be
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789676"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="065d8-103">Update windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="065d8-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="065d8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="065d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="065d8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="065d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="065d8-106">[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="065d8-106">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="065d8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="065d8-107">Prerequisites</span></span>
<span data-ttu-id="065d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="065d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="065d8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="065d8-110">Permission type</span></span>|<span data-ttu-id="065d8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="065d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="065d8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="065d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="065d8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="065d8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="065d8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="065d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="065d8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="065d8-115">Not supported.</span></span>|
|<span data-ttu-id="065d8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="065d8-116">Application</span></span>|<span data-ttu-id="065d8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="065d8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="065d8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="065d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="065d8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="065d8-119">Request headers</span></span>
|<span data-ttu-id="065d8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="065d8-120">Header</span></span>|<span data-ttu-id="065d8-121">値</span><span class="sxs-lookup"><span data-stu-id="065d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="065d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="065d8-122">Authorization</span></span>|<span data-ttu-id="065d8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="065d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="065d8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="065d8-124">Accept</span></span>|<span data-ttu-id="065d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="065d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="065d8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="065d8-126">Request body</span></span>
<span data-ttu-id="065d8-127">要求本文で、[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="065d8-127">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="065d8-128">次の表に、[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-128">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="065d8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="065d8-129">Property</span></span>|<span data-ttu-id="065d8-130">型</span><span class="sxs-lookup"><span data-stu-id="065d8-130">Type</span></span>|<span data-ttu-id="065d8-131">説明</span><span class="sxs-lookup"><span data-stu-id="065d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="065d8-132">id</span><span class="sxs-lookup"><span data-stu-id="065d8-132">id</span></span>|<span data-ttu-id="065d8-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="065d8-133">String</span></span>|<span data-ttu-id="065d8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="065d8-134">Key of the entity.</span></span> <span data-ttu-id="065d8-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="065d8-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="065d8-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="065d8-136">lastModifiedDateTime</span></span>|<span data-ttu-id="065d8-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="065d8-137">DateTimeOffset</span></span>|<span data-ttu-id="065d8-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="065d8-138">DateTime the object was last modified.</span></span> <span data-ttu-id="065d8-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="065d8-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="065d8-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="065d8-140">roleScopeTagIds</span></span>|<span data-ttu-id="065d8-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="065d8-141">String collection</span></span>|<span data-ttu-id="065d8-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="065d8-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="065d8-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="065d8-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="065d8-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="065d8-144">supportsScopeTags</span></span>|<span data-ttu-id="065d8-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-145">Boolean</span></span>|<span data-ttu-id="065d8-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="065d8-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="065d8-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="065d8-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="065d8-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="065d8-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="065d8-149">This property is read-only.</span></span> <span data-ttu-id="065d8-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="065d8-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="065d8-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="065d8-151">createdDateTime</span></span>|<span data-ttu-id="065d8-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="065d8-152">DateTimeOffset</span></span>|<span data-ttu-id="065d8-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="065d8-153">DateTime the object was created.</span></span> <span data-ttu-id="065d8-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="065d8-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="065d8-155">説明</span><span class="sxs-lookup"><span data-stu-id="065d8-155">description</span></span>|<span data-ttu-id="065d8-156">String</span><span class="sxs-lookup"><span data-stu-id="065d8-156">String</span></span>|<span data-ttu-id="065d8-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="065d8-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="065d8-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="065d8-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="065d8-159">displayName</span><span class="sxs-lookup"><span data-stu-id="065d8-159">displayName</span></span>|<span data-ttu-id="065d8-160">String</span><span class="sxs-lookup"><span data-stu-id="065d8-160">String</span></span>|<span data-ttu-id="065d8-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="065d8-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="065d8-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="065d8-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="065d8-163">version</span><span class="sxs-lookup"><span data-stu-id="065d8-163">version</span></span>|<span data-ttu-id="065d8-164">Int32</span><span class="sxs-lookup"><span data-stu-id="065d8-164">Int32</span></span>|<span data-ttu-id="065d8-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="065d8-165">Version of the device configuration.</span></span> <span data-ttu-id="065d8-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="065d8-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="065d8-167">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="065d8-167">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="065d8-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-168">Boolean</span></span>|<span data-ttu-id="065d8-169">このポリシーを Windows Phone 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="065d8-169">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="065d8-170">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="065d8-170">This property is read-only.</span></span>|
|<span data-ttu-id="065d8-171">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="065d8-171">appsBlockCopyPaste</span></span>|<span data-ttu-id="065d8-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-172">Boolean</span></span>|<span data-ttu-id="065d8-173">コピー/貼り付けを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-173">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="065d8-174">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-174">bluetoothBlocked</span></span>|<span data-ttu-id="065d8-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-175">Boolean</span></span>|<span data-ttu-id="065d8-176">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-176">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="065d8-177">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-177">cameraBlocked</span></span>|<span data-ttu-id="065d8-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-178">Boolean</span></span>|<span data-ttu-id="065d8-179">カメラをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-179">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="065d8-180">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="065d8-180">cellularBlockWifiTethering</span></span>|<span data-ttu-id="065d8-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-181">Boolean</span></span>|<span data-ttu-id="065d8-182">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-182">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="065d8-183">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="065d8-183">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="065d8-184">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="065d8-184">compliantAppsList</span></span>|<span data-ttu-id="065d8-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="065d8-185">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="065d8-186">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="065d8-186">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="065d8-187">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="065d8-187">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="065d8-188">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="065d8-188">compliantAppListType</span></span>|[<span data-ttu-id="065d8-189">アプライアンスの種類</span><span class="sxs-lookup"><span data-stu-id="065d8-189">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="065d8-190">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="065d8-190">List that is in the AppComplianceList.</span></span> <span data-ttu-id="065d8-191">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="065d8-191">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="065d8-192">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="065d8-192">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="065d8-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-193">Boolean</span></span>|<span data-ttu-id="065d8-194">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-194">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="065d8-195">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="065d8-195">emailBlockAddingAccounts</span></span>|<span data-ttu-id="065d8-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-196">Boolean</span></span>|<span data-ttu-id="065d8-197">カスタム電子メール アカウントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-197">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="065d8-198">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-198">locationServicesBlocked</span></span>|<span data-ttu-id="065d8-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-199">Boolean</span></span>|<span data-ttu-id="065d8-200">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-200">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="065d8-201">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-201">microsoftAccountBlocked</span></span>|<span data-ttu-id="065d8-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-202">Boolean</span></span>|<span data-ttu-id="065d8-203">Microsoft アカウントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-203">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="065d8-204">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-204">nfcBlocked</span></span>|<span data-ttu-id="065d8-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-205">Boolean</span></span>|<span data-ttu-id="065d8-206">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-206">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="065d8-207">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="065d8-207">passwordBlockSimple</span></span>|<span data-ttu-id="065d8-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-208">Boolean</span></span>|<span data-ttu-id="065d8-209">カレンダーの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-209">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="065d8-210">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="065d8-210">passwordExpirationDays</span></span>|<span data-ttu-id="065d8-211">Int32</span><span class="sxs-lookup"><span data-stu-id="065d8-211">Int32</span></span>|<span data-ttu-id="065d8-212">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="065d8-212">Number of days before the password expires.</span></span>|
|<span data-ttu-id="065d8-213">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="065d8-213">passwordMinimumLength</span></span>|<span data-ttu-id="065d8-214">Int32</span><span class="sxs-lookup"><span data-stu-id="065d8-214">Int32</span></span>|<span data-ttu-id="065d8-215">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="065d8-215">Minimum length of passwords.</span></span>|
|<span data-ttu-id="065d8-216">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="065d8-216">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="065d8-217">Int32</span><span class="sxs-lookup"><span data-stu-id="065d8-217">Int32</span></span>|<span data-ttu-id="065d8-218">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="065d8-218">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="065d8-219">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="065d8-219">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="065d8-220">Int32</span><span class="sxs-lookup"><span data-stu-id="065d8-220">Int32</span></span>|<span data-ttu-id="065d8-221">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="065d8-221">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="065d8-222">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="065d8-222">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="065d8-223">Int32</span><span class="sxs-lookup"><span data-stu-id="065d8-223">Int32</span></span>|<span data-ttu-id="065d8-224">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="065d8-224">Number of previous passwords to block.</span></span> <span data-ttu-id="065d8-225">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="065d8-225">Valid values 0 to 24</span></span>|
|<span data-ttu-id="065d8-226">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="065d8-226">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="065d8-227">Int32</span><span class="sxs-lookup"><span data-stu-id="065d8-227">Int32</span></span>|<span data-ttu-id="065d8-228">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="065d8-228">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="065d8-229">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="065d8-229">passwordRequiredType</span></span>|[<span data-ttu-id="065d8-230">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="065d8-230">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="065d8-231">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="065d8-231">Password type that is required.</span></span> <span data-ttu-id="065d8-232">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="065d8-232">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="065d8-233">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="065d8-233">passwordRequired</span></span>|<span data-ttu-id="065d8-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-234">Boolean</span></span>|<span data-ttu-id="065d8-235">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="065d8-235">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="065d8-236">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-236">screenCaptureBlocked</span></span>|<span data-ttu-id="065d8-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-237">Boolean</span></span>|<span data-ttu-id="065d8-238">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-238">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="065d8-239">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="065d8-239">storageBlockRemovableStorage</span></span>|<span data-ttu-id="065d8-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-240">Boolean</span></span>|<span data-ttu-id="065d8-241">リムーバブル記憶域をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-241">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="065d8-242">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="065d8-242">storageRequireEncryption</span></span>|<span data-ttu-id="065d8-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-243">Boolean</span></span>|<span data-ttu-id="065d8-244">暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-244">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="065d8-245">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-245">webBrowserBlocked</span></span>|<span data-ttu-id="065d8-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-246">Boolean</span></span>|<span data-ttu-id="065d8-247">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-247">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="065d8-248">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-248">wifiBlocked</span></span>|<span data-ttu-id="065d8-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-249">Boolean</span></span>|<span data-ttu-id="065d8-250">Wi-Fi をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-250">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="065d8-251">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="065d8-251">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="065d8-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-252">Boolean</span></span>|<span data-ttu-id="065d8-253">Wi-Fi ホットスポットへの自動接続をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-253">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="065d8-254">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="065d8-254">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="065d8-255">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="065d8-255">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="065d8-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-256">Boolean</span></span>|<span data-ttu-id="065d8-257">Wi-Fi ホットスポット レポートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-257">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="065d8-258">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="065d8-258">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="065d8-259">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="065d8-259">windowsStoreBlocked</span></span>|<span data-ttu-id="065d8-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="065d8-260">Boolean</span></span>|<span data-ttu-id="065d8-261">Windows ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="065d8-261">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="065d8-262">応答</span><span class="sxs-lookup"><span data-stu-id="065d8-262">Response</span></span>
<span data-ttu-id="065d8-263">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="065d8-263">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="065d8-264">例</span><span class="sxs-lookup"><span data-stu-id="065d8-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="065d8-265">要求</span><span class="sxs-lookup"><span data-stu-id="065d8-265">Request</span></span>
<span data-ttu-id="065d8-266">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="065d8-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1553

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="065d8-267">応答</span><span class="sxs-lookup"><span data-stu-id="065d8-267">Response</span></span>
<span data-ttu-id="065d8-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="065d8-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1725

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "applyOnlyToWindowsPhone81": true,
  "appsBlockCopyPaste": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "cellularBlockWifiTethering": true,
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
  "diagnosticDataBlockSubmission": true,
  "emailBlockAddingAccounts": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "nfcBlocked": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireEncryption": true,
  "webBrowserBlocked": true,
  "wifiBlocked": true,
  "wifiBlockAutomaticConnectHotspots": true,
  "wifiBlockHotspotReporting": true,
  "windowsStoreBlocked": true
}
```





