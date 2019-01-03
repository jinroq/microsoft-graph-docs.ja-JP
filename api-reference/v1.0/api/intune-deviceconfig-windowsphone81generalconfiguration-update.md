---
title: Update windowsPhone81GeneralConfiguration
description: windowsPhone81GeneralConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: bbc7208465f625a105bc793681bfd28f8a4f6082
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352144"
---
# <a name="update-windowsphone81generalconfiguration"></a><span data-ttu-id="9d90e-103">Update windowsPhone81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="9d90e-103">Update windowsPhone81GeneralConfiguration</span></span>

> <span data-ttu-id="9d90e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9d90e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9d90e-105">[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-105">Update the properties of a [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9d90e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="9d90e-106">Prerequisites</span></span>
<span data-ttu-id="9d90e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9d90e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d90e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9d90e-109">Permission type</span></span>|<span data-ttu-id="9d90e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9d90e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9d90e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9d90e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9d90e-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9d90e-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9d90e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9d90e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9d90e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d90e-114">Not supported.</span></span>|
|<span data-ttu-id="9d90e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9d90e-115">Application</span></span>|<span data-ttu-id="9d90e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9d90e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9d90e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9d90e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9d90e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d90e-118">Request headers</span></span>
|<span data-ttu-id="9d90e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d90e-119">Header</span></span>|<span data-ttu-id="9d90e-120">値</span><span class="sxs-lookup"><span data-stu-id="9d90e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9d90e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d90e-121">Authorization</span></span>|<span data-ttu-id="9d90e-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9d90e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9d90e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9d90e-123">Accept</span></span>|<span data-ttu-id="9d90e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9d90e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9d90e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="9d90e-125">Request body</span></span>
<span data-ttu-id="9d90e-126">要求本文で、[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-126">In the request body, supply a JSON representation for the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object.</span></span>

<span data-ttu-id="9d90e-127">次の表に、[windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-127">The following table shows the properties that are required when you create the [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md).</span></span>

|<span data-ttu-id="9d90e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9d90e-128">Property</span></span>|<span data-ttu-id="9d90e-129">種類</span><span class="sxs-lookup"><span data-stu-id="9d90e-129">Type</span></span>|<span data-ttu-id="9d90e-130">説明</span><span class="sxs-lookup"><span data-stu-id="9d90e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d90e-131">ID</span><span class="sxs-lookup"><span data-stu-id="9d90e-131">id</span></span>|<span data-ttu-id="9d90e-132">String</span><span class="sxs-lookup"><span data-stu-id="9d90e-132">String</span></span>|<span data-ttu-id="9d90e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9d90e-133">Key of the entity.</span></span> <span data-ttu-id="9d90e-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9d90e-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d90e-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d90e-135">lastModifiedDateTime</span></span>|<span data-ttu-id="9d90e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d90e-136">DateTimeOffset</span></span>|<span data-ttu-id="9d90e-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9d90e-137">DateTime the object was last modified.</span></span> <span data-ttu-id="9d90e-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9d90e-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d90e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d90e-139">createdDateTime</span></span>|<span data-ttu-id="9d90e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d90e-140">DateTimeOffset</span></span>|<span data-ttu-id="9d90e-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9d90e-141">DateTime the object was created.</span></span> <span data-ttu-id="9d90e-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9d90e-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d90e-143">説明</span><span class="sxs-lookup"><span data-stu-id="9d90e-143">description</span></span>|<span data-ttu-id="9d90e-144">String</span><span class="sxs-lookup"><span data-stu-id="9d90e-144">String</span></span>|<span data-ttu-id="9d90e-145">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9d90e-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9d90e-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9d90e-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d90e-147">displayName</span><span class="sxs-lookup"><span data-stu-id="9d90e-147">displayName</span></span>|<span data-ttu-id="9d90e-148">String</span><span class="sxs-lookup"><span data-stu-id="9d90e-148">String</span></span>|<span data-ttu-id="9d90e-149">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9d90e-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9d90e-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9d90e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d90e-151">version</span><span class="sxs-lookup"><span data-stu-id="9d90e-151">version</span></span>|<span data-ttu-id="9d90e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="9d90e-152">Int32</span></span>|<span data-ttu-id="9d90e-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9d90e-153">Version of the device configuration.</span></span> <span data-ttu-id="9d90e-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9d90e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9d90e-155">applyOnlyToWindowsPhone81</span><span class="sxs-lookup"><span data-stu-id="9d90e-155">applyOnlyToWindowsPhone81</span></span>|<span data-ttu-id="9d90e-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-156">Boolean</span></span>|<span data-ttu-id="9d90e-157">このポリシーを Windows Phone 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="9d90e-157">Value indicating whether this policy only applies to Windows Phone 8.1.</span></span> <span data-ttu-id="9d90e-158">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9d90e-158">This property is read-only.</span></span>|
|<span data-ttu-id="9d90e-159">appsBlockCopyPaste</span><span class="sxs-lookup"><span data-stu-id="9d90e-159">appsBlockCopyPaste</span></span>|<span data-ttu-id="9d90e-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-160">Boolean</span></span>|<span data-ttu-id="9d90e-161">コピー/貼り付けを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-161">Indicates whether or not to block copy paste.</span></span>|
|<span data-ttu-id="9d90e-162">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-162">bluetoothBlocked</span></span>|<span data-ttu-id="9d90e-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-163">Boolean</span></span>|<span data-ttu-id="9d90e-164">Bluetooth をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-164">Indicates whether or not to block bluetooth.</span></span>|
|<span data-ttu-id="9d90e-165">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-165">cameraBlocked</span></span>|<span data-ttu-id="9d90e-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-166">Boolean</span></span>|<span data-ttu-id="9d90e-167">カメラをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-167">Indicates whether or not to block camera.</span></span>|
|<span data-ttu-id="9d90e-168">cellularBlockWifiTethering</span><span class="sxs-lookup"><span data-stu-id="9d90e-168">cellularBlockWifiTethering</span></span>|<span data-ttu-id="9d90e-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-169">Boolean</span></span>|<span data-ttu-id="9d90e-170">Wi-Fi テザリングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-170">Indicates whether or not to block Wi-Fi tethering.</span></span> <span data-ttu-id="9d90e-171">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="9d90e-171">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="9d90e-172">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="9d90e-172">compliantAppsList</span></span>|<span data-ttu-id="9d90e-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="9d90e-173">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="9d90e-174">コンプライアンス内のアプリのリスト (CompliantAppListType によって制御される、許可リストまたは禁止リスト)。</span><span class="sxs-lookup"><span data-stu-id="9d90e-174">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="9d90e-175">このコレクションには、最大で 10000 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9d90e-175">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="9d90e-176">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="9d90e-176">compliantAppListType</span></span>|[<span data-ttu-id="9d90e-177">appListType</span><span class="sxs-lookup"><span data-stu-id="9d90e-177">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="9d90e-178">AppComplianceList 内にあるリスト。</span><span class="sxs-lookup"><span data-stu-id="9d90e-178">List that is in the AppComplianceList.</span></span> <span data-ttu-id="9d90e-179">可能な値は、`none`、`appsInListCompliant`、`appsNotInListCompliant` です。</span><span class="sxs-lookup"><span data-stu-id="9d90e-179">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="9d90e-180">diagnosticDataBlockSubmission</span><span class="sxs-lookup"><span data-stu-id="9d90e-180">diagnosticDataBlockSubmission</span></span>|<span data-ttu-id="9d90e-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-181">Boolean</span></span>|<span data-ttu-id="9d90e-182">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-182">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="9d90e-183">emailBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="9d90e-183">emailBlockAddingAccounts</span></span>|<span data-ttu-id="9d90e-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-184">Boolean</span></span>|<span data-ttu-id="9d90e-185">カスタム電子メール アカウントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-185">Indicates whether or not to block custom email accounts.</span></span>|
|<span data-ttu-id="9d90e-186">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-186">locationServicesBlocked</span></span>|<span data-ttu-id="9d90e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-187">Boolean</span></span>|<span data-ttu-id="9d90e-188">位置情報サービスをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-188">Indicates whether or not to block location services.</span></span>|
|<span data-ttu-id="9d90e-189">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-189">microsoftAccountBlocked</span></span>|<span data-ttu-id="9d90e-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-190">Boolean</span></span>|<span data-ttu-id="9d90e-191">Microsoft アカウントの使用を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-191">Indicates whether or not to block using a Microsoft Account.</span></span>|
|<span data-ttu-id="9d90e-192">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-192">nfcBlocked</span></span>|<span data-ttu-id="9d90e-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-193">Boolean</span></span>|<span data-ttu-id="9d90e-194">近距離無線通信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-194">Indicates whether or not to block Near-Field Communication.</span></span>|
|<span data-ttu-id="9d90e-195">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="9d90e-195">passwordBlockSimple</span></span>|<span data-ttu-id="9d90e-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-196">Boolean</span></span>|<span data-ttu-id="9d90e-197">カレンダーの同期を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-197">Indicates whether or not to block syncing the calendar.</span></span>|
|<span data-ttu-id="9d90e-198">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9d90e-198">passwordExpirationDays</span></span>|<span data-ttu-id="9d90e-199">Int32</span><span class="sxs-lookup"><span data-stu-id="9d90e-199">Int32</span></span>|<span data-ttu-id="9d90e-200">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="9d90e-200">Number of days before the password expires.</span></span>|
|<span data-ttu-id="9d90e-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9d90e-201">passwordMinimumLength</span></span>|<span data-ttu-id="9d90e-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9d90e-202">Int32</span></span>|<span data-ttu-id="9d90e-203">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="9d90e-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="9d90e-204">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9d90e-204">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9d90e-205">Int32</span><span class="sxs-lookup"><span data-stu-id="9d90e-205">Int32</span></span>|<span data-ttu-id="9d90e-206">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="9d90e-206">Minutes of inactivity before screen timeout.</span></span>|
|<span data-ttu-id="9d90e-207">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9d90e-207">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9d90e-208">Int32</span><span class="sxs-lookup"><span data-stu-id="9d90e-208">Int32</span></span>|<span data-ttu-id="9d90e-209">パスワードが含まなければならない文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="9d90e-209">Number of character sets a password must contain.</span></span>|
|<span data-ttu-id="9d90e-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9d90e-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9d90e-211">Int32</span><span class="sxs-lookup"><span data-stu-id="9d90e-211">Int32</span></span>|<span data-ttu-id="9d90e-212">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="9d90e-212">Number of previous passwords to block.</span></span> <span data-ttu-id="9d90e-213">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="9d90e-213">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9d90e-214">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9d90e-214">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9d90e-215">Int32</span><span class="sxs-lookup"><span data-stu-id="9d90e-215">Int32</span></span>|<span data-ttu-id="9d90e-216">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="9d90e-216">Number of sign in failures allowed before factory reset.</span></span>|
|<span data-ttu-id="9d90e-217">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9d90e-217">passwordRequiredType</span></span>|[<span data-ttu-id="9d90e-218">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="9d90e-218">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9d90e-219">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="9d90e-219">Password type that is required.</span></span> <span data-ttu-id="9d90e-220">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="9d90e-220">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9d90e-221">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="9d90e-221">passwordRequired</span></span>|<span data-ttu-id="9d90e-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-222">Boolean</span></span>|<span data-ttu-id="9d90e-223">パスワードを要求するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-223">Indicates whether or not to require a password.</span></span>|
|<span data-ttu-id="9d90e-224">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-224">screenCaptureBlocked</span></span>|<span data-ttu-id="9d90e-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-225">Boolean</span></span>|<span data-ttu-id="9d90e-226">スクリーンショットを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-226">Indicates whether or not to block screenshots.</span></span>|
|<span data-ttu-id="9d90e-227">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="9d90e-227">storageBlockRemovableStorage</span></span>|<span data-ttu-id="9d90e-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-228">Boolean</span></span>|<span data-ttu-id="9d90e-229">リムーバブル記憶域をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-229">Indicates whether or not to block removable storage.</span></span>|
|<span data-ttu-id="9d90e-230">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="9d90e-230">storageRequireEncryption</span></span>|<span data-ttu-id="9d90e-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-231">Boolean</span></span>|<span data-ttu-id="9d90e-232">暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-232">Indicates whether or not to require encryption.</span></span>|
|<span data-ttu-id="9d90e-233">webBrowserBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-233">webBrowserBlocked</span></span>|<span data-ttu-id="9d90e-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-234">Boolean</span></span>|<span data-ttu-id="9d90e-235">Web ブラウザーをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-235">Indicates whether or not to block the web browser.</span></span>|
|<span data-ttu-id="9d90e-236">wifiBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-236">wifiBlocked</span></span>|<span data-ttu-id="9d90e-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-237">Boolean</span></span>|<span data-ttu-id="9d90e-238">Wi-Fi をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-238">Indicates whether or not to block Wi-Fi.</span></span>|
|<span data-ttu-id="9d90e-239">wifiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="9d90e-239">wifiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="9d90e-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-240">Boolean</span></span>|<span data-ttu-id="9d90e-241">Wi-Fi ホットスポットへの自動接続をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-241">Indicates whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="9d90e-242">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="9d90e-242">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="9d90e-243">wifiBlockHotspotReporting</span><span class="sxs-lookup"><span data-stu-id="9d90e-243">wifiBlockHotspotReporting</span></span>|<span data-ttu-id="9d90e-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-244">Boolean</span></span>|<span data-ttu-id="9d90e-245">Wi-Fi ホットスポット レポートをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-245">Indicates whether or not to block Wi-Fi hotspot reporting.</span></span> <span data-ttu-id="9d90e-246">Wi-Fi がブロックされていれば、この値は関係ありません。</span><span class="sxs-lookup"><span data-stu-id="9d90e-246">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="9d90e-247">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="9d90e-247">windowsStoreBlocked</span></span>|<span data-ttu-id="9d90e-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="9d90e-248">Boolean</span></span>|<span data-ttu-id="9d90e-249">Windows ストアをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-249">Indicates whether or not to block the Windows Store.</span></span>|



## <a name="response"></a><span data-ttu-id="9d90e-250">応答</span><span class="sxs-lookup"><span data-stu-id="9d90e-250">Response</span></span>
<span data-ttu-id="9d90e-251">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9d90e-251">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81GeneralConfiguration](../resources/intune-deviceconfig-windowsphone81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9d90e-252">例</span><span class="sxs-lookup"><span data-stu-id="9d90e-252">Example</span></span>
### <a name="request"></a><span data-ttu-id="9d90e-253">要求</span><span class="sxs-lookup"><span data-stu-id="9d90e-253">Request</span></span>
<span data-ttu-id="9d90e-254">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9d90e-254">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1461

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
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

### <a name="response"></a><span data-ttu-id="9d90e-255">応答</span><span class="sxs-lookup"><span data-stu-id="9d90e-255">Response</span></span>
<span data-ttu-id="9d90e-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9d90e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1633

{
  "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
  "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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


