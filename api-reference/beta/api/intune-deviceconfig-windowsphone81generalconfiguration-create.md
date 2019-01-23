---
title: Create windowsPhone81GeneralConfiguration
description: 新しい windowsPhone81GeneralConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 470e319c9640a0052df96730371fbaf4ff1f153c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421915"
---
# <a name="create-windowsphone81generalconfiguration"></a><span data-ttu-id="4fb16-103">Create windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="4fb16-103">Create windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="4fb16-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4fb16-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4fb16-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4fb16-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fb16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fb16-107">新しい [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-107">Create a new [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fb16-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4fb16-108">Prerequisites</span></span>
<span data-ttu-id="4fb16-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fb16-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4fb16-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4fb16-111">Permission type</span></span>|<span data-ttu-id="4fb16-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4fb16-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fb16-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4fb16-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fb16-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fb16-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4fb16-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4fb16-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fb16-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb16-116">Not supported.</span></span>|
|<span data-ttu-id="4fb16-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4fb16-117">Application</span></span>|<span data-ttu-id="4fb16-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fb16-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fb16-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fb16-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4fb16-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fb16-120">Request headers</span></span>
|<span data-ttu-id="4fb16-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fb16-121">Header</span></span>|<span data-ttu-id="4fb16-122">値</span><span class="sxs-lookup"><span data-stu-id="4fb16-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fb16-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fb16-123">Authorization</span></span>|<span data-ttu-id="4fb16-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4fb16-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fb16-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4fb16-125">Accept</span></span>|<span data-ttu-id="4fb16-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fb16-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fb16-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fb16-127">Request body</span></span>
<span data-ttu-id="4fb16-128">要求本文で、windowsPhone81GeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-128">In the request body, supply a JSON representation for the windowsPhone81GeneralConfiguration object.</span></span>

<span data-ttu-id="4fb16-129">次の表に、windowsPhone81GeneralConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-129">The following table shows the properties that are required when you create the windowsPhone81GeneralConfiguration.</span></span>

|<span data-ttu-id="4fb16-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fb16-130">Property</span></span>|<span data-ttu-id="4fb16-131">型</span><span class="sxs-lookup"><span data-stu-id="4fb16-131">Type</span></span>|<span data-ttu-id="4fb16-132">説明</span><span class="sxs-lookup"><span data-stu-id="4fb16-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fb16-133">id</span><span class="sxs-lookup"><span data-stu-id="4fb16-133">id</span></span>|<span data-ttu-id="4fb16-134">String</span><span class="sxs-lookup"><span data-stu-id="4fb16-134">String</span></span>|<span data-ttu-id="4fb16-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4fb16-135">Key of the entity.</span></span> <span data-ttu-id="4fb16-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fb16-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fb16-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fb16-137">lastModifiedDateTime</span></span>|<span data-ttu-id="4fb16-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fb16-138">DateTimeOffset</span></span>|<span data-ttu-id="4fb16-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4fb16-139">DateTime the object was last modified.</span></span> <span data-ttu-id="4fb16-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fb16-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fb16-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4fb16-141">roleScopeTagIds</span></span>|<span data-ttu-id="4fb16-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb16-142">String collection</span></span>|<span data-ttu-id="4fb16-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="4fb16-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4fb16-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fb16-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fb16-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4fb16-145">supportsScopeTags</span></span>|<span data-ttu-id="4fb16-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-146">Boolean</span></span>|<span data-ttu-id="4fb16-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4fb16-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="4fb16-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4fb16-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="4fb16-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4fb16-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="4fb16-150">This property is read-only.</span></span> <span data-ttu-id="4fb16-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fb16-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fb16-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fb16-152">createdDateTime</span></span>|<span data-ttu-id="4fb16-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fb16-153">DateTimeOffset</span></span>|<span data-ttu-id="4fb16-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4fb16-154">DateTime the object was created.</span></span> <span data-ttu-id="4fb16-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fb16-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fb16-156">説明</span><span class="sxs-lookup"><span data-stu-id="4fb16-156">description</span></span>|<span data-ttu-id="4fb16-157">String</span><span class="sxs-lookup"><span data-stu-id="4fb16-157">String</span></span>|<span data-ttu-id="4fb16-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="4fb16-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4fb16-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fb16-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fb16-160">displayName</span><span class="sxs-lookup"><span data-stu-id="4fb16-160">displayName</span></span>|<span data-ttu-id="4fb16-161">String</span><span class="sxs-lookup"><span data-stu-id="4fb16-161">String</span></span>|<span data-ttu-id="4fb16-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="4fb16-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4fb16-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fb16-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fb16-164">version</span><span class="sxs-lookup"><span data-stu-id="4fb16-164">version</span></span>|<span data-ttu-id="4fb16-165">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb16-165">Int32</span></span>|<span data-ttu-id="4fb16-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4fb16-166">Version of the device configuration.</span></span> <span data-ttu-id="4fb16-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fb16-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4fb16-168">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="4fb16-168">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="4fb16-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-169">Boolean</span></span>|<span data-ttu-id="4fb16-170">このポリシーを Windows Phone 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="4fb16-170">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="4fb16-171">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="4fb16-171">This property is read-only.</span></span>|
|<span data-ttu-id="4fb16-172">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4fb16-172">appsBlockCopyPaste</span></span>|<span data-ttu-id="4fb16-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-173">Boolean</span></span>|<span data-ttu-id="4fb16-174">コピー/貼り付けを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-174">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="4fb16-175">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-175">bluetoothBlocked</span></span>|<span data-ttu-id="4fb16-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-176">Boolean</span></span>|<span data-ttu-id="4fb16-177">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-177">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="4fb16-178">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-178">cameraBlocked</span></span>|<span data-ttu-id="4fb16-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-179">Boolean</span></span>|<span data-ttu-id="4fb16-180">カメラをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-180">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="4fb16-181">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="4fb16-181">cellularBlockWifiTethering</span></span>|<span data-ttu-id="4fb16-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-182">Boolean</span></span>|<span data-ttu-id="4fb16-183">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-183">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="4fb16-184">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="4fb16-184">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4fb16-185">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4fb16-185">compliantAppsList</span></span>|<span data-ttu-id="4fb16-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4fb16-186">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4fb16-187">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="4fb16-187">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4fb16-188">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="4fb16-188">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4fb16-189">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4fb16-189">compliantAppListType</span></span>|[<span data-ttu-id="4fb16-190">appListType</span><span class="sxs-lookup"><span data-stu-id="4fb16-190">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="4fb16-191">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="4fb16-191">List that is in the AppComplianceList.</span></span> <span data-ttu-id="4fb16-192">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="4fb16-192">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4fb16-193">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="4fb16-193">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="4fb16-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-194">Boolean</span></span>|<span data-ttu-id="4fb16-195">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-195">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="4fb16-196">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="4fb16-196">emailBlockAddingAccounts</span></span>|<span data-ttu-id="4fb16-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-197">Boolean</span></span>|<span data-ttu-id="4fb16-198">カスタム電子メール アカウントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-198">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="4fb16-199">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-199">locationServicesBlocked</span></span>|<span data-ttu-id="4fb16-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-200">Boolean</span></span>|<span data-ttu-id="4fb16-201">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-201">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="4fb16-202">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-202">microsoftAccountBlocked</span></span>|<span data-ttu-id="4fb16-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-203">Boolean</span></span>|<span data-ttu-id="4fb16-204">Microsoft アカウントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-204">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="4fb16-205">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-205">nfcBlocked</span></span>|<span data-ttu-id="4fb16-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-206">Boolean</span></span>|<span data-ttu-id="4fb16-207">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-207">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="4fb16-208">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4fb16-208">passwordBlockSimple</span></span>|<span data-ttu-id="4fb16-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-209">Boolean</span></span>|<span data-ttu-id="4fb16-210">カレンダーの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-210">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="4fb16-211">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4fb16-211">passwordExpirationDays</span></span>|<span data-ttu-id="4fb16-212">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb16-212">Int32</span></span>|<span data-ttu-id="4fb16-213">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="4fb16-213">Number of days before the password expires.</span></span>|
|<span data-ttu-id="4fb16-214">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4fb16-214">passwordMinimumLength</span></span>|<span data-ttu-id="4fb16-215">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb16-215">Int32</span></span>|<span data-ttu-id="4fb16-216">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="4fb16-216">Minimum length of passwords.</span></span>|
|<span data-ttu-id="4fb16-217">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4fb16-217">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4fb16-218">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb16-218">Int32</span></span>|<span data-ttu-id="4fb16-219">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="4fb16-219">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="4fb16-220">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4fb16-220">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4fb16-221">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb16-221">Int32</span></span>|<span data-ttu-id="4fb16-222">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="4fb16-222">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="4fb16-223">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4fb16-223">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4fb16-224">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb16-224">Int32</span></span>|<span data-ttu-id="4fb16-225">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="4fb16-225">Number of previous passwords to block.</span></span> <span data-ttu-id="4fb16-226">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="4fb16-226">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4fb16-227">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4fb16-227">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4fb16-228">Int32</span><span class="sxs-lookup"><span data-stu-id="4fb16-228">Int32</span></span>|<span data-ttu-id="4fb16-229">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="4fb16-229">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="4fb16-230">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4fb16-230">passwordRequiredType</span></span>|[<span data-ttu-id="4fb16-231">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4fb16-231">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4fb16-232">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="4fb16-232">Password type that is required.</span></span> <span data-ttu-id="4fb16-233">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="4fb16-233">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4fb16-234">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4fb16-234">passwordRequired</span></span>|<span data-ttu-id="4fb16-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-235">Boolean</span></span>|<span data-ttu-id="4fb16-236">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-236">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="4fb16-237">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-237">screenCaptureBlocked</span></span>|<span data-ttu-id="4fb16-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-238">Boolean</span></span>|<span data-ttu-id="4fb16-239">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-239">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="4fb16-240">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="4fb16-240">storageBlockRemovableStorage</span></span>|<span data-ttu-id="4fb16-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-241">Boolean</span></span>|<span data-ttu-id="4fb16-242">リムーバブル記憶域をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-242">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="4fb16-243">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="4fb16-243">storageRequireEncryption</span></span>|<span data-ttu-id="4fb16-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-244">Boolean</span></span>|<span data-ttu-id="4fb16-245">暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-245">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="4fb16-246">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-246">webBrowserBlocked</span></span>|<span data-ttu-id="4fb16-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-247">Boolean</span></span>|<span data-ttu-id="4fb16-248">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-248">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="4fb16-249">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-249">wifiBlocked</span></span>|<span data-ttu-id="4fb16-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-250">Boolean</span></span>|<span data-ttu-id="4fb16-251">Wi-Fi をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-251">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="4fb16-252">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="4fb16-252">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="4fb16-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-253">Boolean</span></span>|<span data-ttu-id="4fb16-254">Wi-Fi ホットスポットへの自動接続をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-254">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="4fb16-255">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="4fb16-255">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4fb16-256">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="4fb16-256">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="4fb16-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-257">Boolean</span></span>|<span data-ttu-id="4fb16-258">Wi-Fi ホットスポット レポートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-258">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="4fb16-259">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="4fb16-259">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="4fb16-260">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="4fb16-260">windowsStoreBlocked</span></span>|<span data-ttu-id="4fb16-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fb16-261">Boolean</span></span>|<span data-ttu-id="4fb16-262">Windows ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-262">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="4fb16-263">応答</span><span class="sxs-lookup"><span data-stu-id="4fb16-263">Response</span></span>
<span data-ttu-id="4fb16-264">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4fb16-264">If successful, this method returns a `201 Created` response code and a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fb16-265">例</span><span class="sxs-lookup"><span data-stu-id="4fb16-265">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fb16-266">要求</span><span class="sxs-lookup"><span data-stu-id="4fb16-266">Request</span></span>
<span data-ttu-id="4fb16-267">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fb16-267">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4fb16-268">応答</span><span class="sxs-lookup"><span data-stu-id="4fb16-268">Response</span></span>
<span data-ttu-id="4fb16-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4fb16-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




