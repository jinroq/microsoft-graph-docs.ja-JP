---
title: AndroidForWorkGeneralDeviceConfiguration を作成します。
description: 新しい androidForWorkGeneralDeviceConfiguration オブジェクトを作成します。
ms.openlocfilehash: e04f2071fff39e8030d38203d3c2fc8bb550ac48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072734"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="02dcf-103">AndroidForWorkGeneralDeviceConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="02dcf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02dcf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02dcf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02dcf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="02dcf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="02dcf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="02dcf-107">新しい[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-107">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="02dcf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="02dcf-108">Prerequisites</span></span>
<span data-ttu-id="02dcf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02dcf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02dcf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02dcf-111">Permission type</span></span>|<span data-ttu-id="02dcf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="02dcf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02dcf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02dcf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02dcf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02dcf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="02dcf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02dcf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02dcf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02dcf-116">Not supported.</span></span>|
|<span data-ttu-id="02dcf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02dcf-117">Application</span></span>|<span data-ttu-id="02dcf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02dcf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02dcf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02dcf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="02dcf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02dcf-120">Request headers</span></span>
|<span data-ttu-id="02dcf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02dcf-121">Header</span></span>|<span data-ttu-id="02dcf-122">値</span><span class="sxs-lookup"><span data-stu-id="02dcf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02dcf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02dcf-123">Authorization</span></span>|<span data-ttu-id="02dcf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="02dcf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02dcf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="02dcf-125">Accept</span></span>|<span data-ttu-id="02dcf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02dcf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02dcf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="02dcf-127">Request body</span></span>
<span data-ttu-id="02dcf-128">要求の本文に androidForWorkGeneralDeviceConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-128">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="02dcf-129">次の表は、androidForWorkGeneralDeviceConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-129">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="02dcf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02dcf-130">Property</span></span>|<span data-ttu-id="02dcf-131">型</span><span class="sxs-lookup"><span data-stu-id="02dcf-131">Type</span></span>|<span data-ttu-id="02dcf-132">説明</span><span class="sxs-lookup"><span data-stu-id="02dcf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02dcf-133">id</span><span class="sxs-lookup"><span data-stu-id="02dcf-133">id</span></span>|<span data-ttu-id="02dcf-134">String</span><span class="sxs-lookup"><span data-stu-id="02dcf-134">String</span></span>|<span data-ttu-id="02dcf-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="02dcf-135">Key of the entity.</span></span> <span data-ttu-id="02dcf-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02dcf-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02dcf-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02dcf-137">lastModifiedDateTime</span></span>|<span data-ttu-id="02dcf-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02dcf-138">DateTimeOffset</span></span>|<span data-ttu-id="02dcf-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="02dcf-139">DateTime the object was last modified.</span></span> <span data-ttu-id="02dcf-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02dcf-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02dcf-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="02dcf-141">roleScopeTagIds</span></span>|<span data-ttu-id="02dcf-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="02dcf-142">String collection</span></span>|<span data-ttu-id="02dcf-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="02dcf-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="02dcf-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02dcf-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02dcf-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="02dcf-145">supportsScopeTags</span></span>|<span data-ttu-id="02dcf-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-146">Boolean</span></span>|<span data-ttu-id="02dcf-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="02dcf-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="02dcf-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="02dcf-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="02dcf-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="02dcf-150">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-150">This property is read-only.</span></span> <span data-ttu-id="02dcf-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02dcf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02dcf-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02dcf-152">createdDateTime</span></span>|<span data-ttu-id="02dcf-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02dcf-153">DateTimeOffset</span></span>|<span data-ttu-id="02dcf-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="02dcf-154">DateTime the object was created.</span></span> <span data-ttu-id="02dcf-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02dcf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02dcf-156">説明</span><span class="sxs-lookup"><span data-stu-id="02dcf-156">description</span></span>|<span data-ttu-id="02dcf-157">String</span><span class="sxs-lookup"><span data-stu-id="02dcf-157">String</span></span>|<span data-ttu-id="02dcf-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="02dcf-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="02dcf-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02dcf-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02dcf-160">displayName</span><span class="sxs-lookup"><span data-stu-id="02dcf-160">displayName</span></span>|<span data-ttu-id="02dcf-161">String</span><span class="sxs-lookup"><span data-stu-id="02dcf-161">String</span></span>|<span data-ttu-id="02dcf-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="02dcf-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="02dcf-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02dcf-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02dcf-164">version</span><span class="sxs-lookup"><span data-stu-id="02dcf-164">version</span></span>|<span data-ttu-id="02dcf-165">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-165">Int32</span></span>|<span data-ttu-id="02dcf-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="02dcf-166">Version of the device configuration.</span></span> <span data-ttu-id="02dcf-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02dcf-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="02dcf-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="02dcf-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="02dcf-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-169">Boolean</span></span>|<span data-ttu-id="02dcf-170">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="02dcf-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="02dcf-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="02dcf-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-172">Boolean</span></span>|<span data-ttu-id="02dcf-173">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="02dcf-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="02dcf-174">passwordExpirationDays</span></span>|<span data-ttu-id="02dcf-175">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-175">Int32</span></span>|<span data-ttu-id="02dcf-176">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="02dcf-176">Number of days before the password expires.</span></span> <span data-ttu-id="02dcf-177">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="02dcf-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="02dcf-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="02dcf-178">passwordMinimumLength</span></span>|<span data-ttu-id="02dcf-179">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-179">Int32</span></span>|<span data-ttu-id="02dcf-180">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="02dcf-180">Minimum length of passwords.</span></span> <span data-ttu-id="02dcf-181">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="02dcf-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="02dcf-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="02dcf-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="02dcf-183">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-183">Int32</span></span>|<span data-ttu-id="02dcf-184">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="02dcf-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="02dcf-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="02dcf-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="02dcf-186">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-186">Int32</span></span>|<span data-ttu-id="02dcf-187">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="02dcf-187">Number of previous passwords to block.</span></span> <span data-ttu-id="02dcf-188">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="02dcf-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="02dcf-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="02dcf-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="02dcf-190">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-190">Int32</span></span>|<span data-ttu-id="02dcf-191">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="02dcf-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="02dcf-192">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="02dcf-192">Valid values 4 to 11</span></span>|
|<span data-ttu-id="02dcf-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="02dcf-193">passwordRequiredType</span></span>|[<span data-ttu-id="02dcf-194">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="02dcf-194">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="02dcf-195">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="02dcf-195">Type of password that is required.</span></span> <span data-ttu-id="02dcf-196">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="02dcf-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="02dcf-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="02dcf-198">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="02dcf-198">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="02dcf-199">共有するデータの種類を許可します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="02dcf-200">可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="02dcf-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="02dcf-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="02dcf-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-202">Boolean</span></span>|<span data-ttu-id="02dcf-203">デバイスがロックされているときに通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="02dcf-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="02dcf-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="02dcf-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-205">Boolean</span></span>|<span data-ttu-id="02dcf-206">作業プロファイル内のアカウントを追加または削除したり、ユーザーをブロックします。</span><span class="sxs-lookup"><span data-stu-id="02dcf-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="02dcf-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="02dcf-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="02dcf-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-208">Boolean</span></span>|<span data-ttu-id="02dcf-209">企業の連絡先にアクセスするための bluetooth デバイスを使用できます。</span><span class="sxs-lookup"><span data-stu-id="02dcf-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="02dcf-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="02dcf-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="02dcf-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-211">Boolean</span></span>|<span data-ttu-id="02dcf-212">作業プロファイルで、画面の取り込みをブロックします。</span><span class="sxs-lookup"><span data-stu-id="02dcf-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="02dcf-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="02dcf-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="02dcf-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-214">Boolean</span></span>|<span data-ttu-id="02dcf-215">ブロックでは、作業プロファイル呼び出し元 ID を表示個人プロファイルにします。</span><span class="sxs-lookup"><span data-stu-id="02dcf-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="02dcf-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="02dcf-216">workProfileBlockCamera</span></span>|<span data-ttu-id="02dcf-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-217">Boolean</span></span>|<span data-ttu-id="02dcf-218">ブロック プロファイル カメラが動作します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-218">Block work profile camera.</span></span>|
|<span data-ttu-id="02dcf-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="02dcf-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="02dcf-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-220">Boolean</span></span>|<span data-ttu-id="02dcf-221">個人プロファイルでは、作業プロファイルの連絡先可用性ブロックです。</span><span class="sxs-lookup"><span data-stu-id="02dcf-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="02dcf-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="02dcf-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="02dcf-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-223">Boolean</span></span>|<span data-ttu-id="02dcf-224">プロファイルのコピーと貼り付けが有効になっている間の設定を許可しない場合を示すブール値です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="02dcf-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="02dcf-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="02dcf-226">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="02dcf-226">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="02dcf-227">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="02dcf-227">Type of password that is required.</span></span> <span data-ttu-id="02dcf-228">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="02dcf-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="02dcf-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="02dcf-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-230">Boolean</span></span>|<span data-ttu-id="02dcf-231">指紋をブロックするかどうかを示す作業プロファイルのロックを解除します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="02dcf-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="02dcf-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="02dcf-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-233">Boolean</span></span>|<span data-ttu-id="02dcf-234">スマート ロックと作業プロファイルを他の信頼のエージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="02dcf-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="02dcf-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="02dcf-236">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-236">Int32</span></span>|<span data-ttu-id="02dcf-237">日前作業プロファイルのパスワードに、の有効期限が切れます。</span><span class="sxs-lookup"><span data-stu-id="02dcf-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="02dcf-238">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="02dcf-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="02dcf-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="02dcf-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="02dcf-240">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-240">Int32</span></span>|<span data-ttu-id="02dcf-241">作業プロファイル パスワードの最小長。</span><span class="sxs-lookup"><span data-stu-id="02dcf-241">Minimum length of work profile password.</span></span> <span data-ttu-id="02dcf-242">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="02dcf-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="02dcf-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="02dcf-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="02dcf-244">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-244">Int32</span></span>|<span data-ttu-id="02dcf-245">プロファイル パスワードの作業に必要な数字の最小数です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="02dcf-246">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="02dcf-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="02dcf-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="02dcf-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="02dcf-248">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-248">Int32</span></span>|<span data-ttu-id="02dcf-249">プロファイル パスワードの作業に必要なアルファベット以外の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="02dcf-250">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="02dcf-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="02dcf-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="02dcf-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="02dcf-252">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-252">Int32</span></span>|<span data-ttu-id="02dcf-253">プロファイル パスワードの作業で必要な文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="02dcf-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="02dcf-254">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="02dcf-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="02dcf-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="02dcf-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="02dcf-256">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-256">Int32</span></span>|<span data-ttu-id="02dcf-257">作業プロファイルのパスワードに必要な小文字の文字数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="02dcf-258">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="02dcf-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="02dcf-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="02dcf-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="02dcf-260">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-260">Int32</span></span>|<span data-ttu-id="02dcf-261">プロファイル パスワードの作業に必要な大文字の文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="02dcf-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="02dcf-262">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="02dcf-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="02dcf-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="02dcf-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="02dcf-264">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-264">Int32</span></span>|<span data-ttu-id="02dcf-265">プロファイル パスワードの作業で必要なシンボル数の最小値です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="02dcf-266">有効な値 1 ~ 10</span><span class="sxs-lookup"><span data-stu-id="02dcf-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="02dcf-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="02dcf-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="02dcf-268">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-268">Int32</span></span>|<span data-ttu-id="02dcf-269">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="02dcf-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="02dcf-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="02dcf-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="02dcf-271">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-271">Int32</span></span>|<span data-ttu-id="02dcf-272">ブロックする前の作業プロファイル パスワードの数です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="02dcf-273">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="02dcf-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="02dcf-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="02dcf-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="02dcf-275">Int32</span><span class="sxs-lookup"><span data-stu-id="02dcf-275">Int32</span></span>|<span data-ttu-id="02dcf-276">作業プロファイルが削除されるまでに許容される障害および削除されたすべての企業データの記号の数です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="02dcf-277">有効な値は 4 から 11 までです</span><span class="sxs-lookup"><span data-stu-id="02dcf-277">Valid values 4 to 11</span></span>|
|<span data-ttu-id="02dcf-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="02dcf-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="02dcf-279">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="02dcf-279">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="02dcf-280">必要な作業プロファイル パスワードの種類です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-280">Type of work profile password that is required.</span></span> <span data-ttu-id="02dcf-281">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="02dcf-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="02dcf-282">workProfileRequirePassword</span></span>|<span data-ttu-id="02dcf-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-283">Boolean</span></span>|<span data-ttu-id="02dcf-284">パスワードが必要な作業プロファイルを</span><span class="sxs-lookup"><span data-stu-id="02dcf-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="02dcf-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="02dcf-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="02dcf-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-286">Boolean</span></span>|<span data-ttu-id="02dcf-287">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="02dcf-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="02dcf-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="02dcf-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="02dcf-289">String</span><span class="sxs-lookup"><span data-stu-id="02dcf-289">String</span></span>|<span data-ttu-id="02dcf-290">常時接続で VPN には、ロックダウン モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="02dcf-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="02dcf-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="02dcf-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="02dcf-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="02dcf-292">Boolean</span></span>|<span data-ttu-id="02dcf-293">常時接続で VPN には、ロックダウン モードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="02dcf-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="02dcf-294">応答</span><span class="sxs-lookup"><span data-stu-id="02dcf-294">Response</span></span>
<span data-ttu-id="02dcf-295">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="02dcf-295">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02dcf-296">例</span><span class="sxs-lookup"><span data-stu-id="02dcf-296">Example</span></span>
### <a name="request"></a><span data-ttu-id="02dcf-297">要求</span><span class="sxs-lookup"><span data-stu-id="02dcf-297">Request</span></span>
<span data-ttu-id="02dcf-298">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02dcf-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2102

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a><span data-ttu-id="02dcf-299">応答</span><span class="sxs-lookup"><span data-stu-id="02dcf-299">Response</span></span>
<span data-ttu-id="02dcf-p129">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02dcf-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2210

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```





