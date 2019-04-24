---
title: androidwork profileて devicの種類を作成する
description: 新しい androidwork profileの devic/オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de10918fad9ba8ca6ee1d2f8c08ac65ee8c91862
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32475075"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="e7d63-103">androidwork profileて devicの種類を作成する</span><span class="sxs-lookup"><span data-stu-id="e7d63-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e7d63-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7d63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7d63-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7d63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7d63-106">新しい[androidwork profileの devic/](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7d63-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e7d63-107">Prerequisites</span></span>
<span data-ttu-id="e7d63-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7d63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7d63-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7d63-110">Permission type</span></span>|<span data-ttu-id="e7d63-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7d63-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7d63-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7d63-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e7d63-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7d63-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7d63-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7d63-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7d63-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7d63-115">Not supported.</span></span>|
|<span data-ttu-id="e7d63-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7d63-116">Application</span></span>|<span data-ttu-id="e7d63-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7d63-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7d63-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7d63-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e7d63-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7d63-119">Request headers</span></span>
|<span data-ttu-id="e7d63-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7d63-120">Header</span></span>|<span data-ttu-id="e7d63-121">値</span><span class="sxs-lookup"><span data-stu-id="e7d63-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7d63-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7d63-122">Authorization</span></span>|<span data-ttu-id="e7d63-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7d63-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7d63-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e7d63-124">Accept</span></span>|<span data-ttu-id="e7d63-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e7d63-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7d63-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7d63-126">Request body</span></span>
<span data-ttu-id="e7d63-127">要求本文で、androidwork profileの devic/devicオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="e7d63-128">次の表に、androidwork profile[devic] の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="e7d63-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7d63-129">Property</span></span>|<span data-ttu-id="e7d63-130">型</span><span class="sxs-lookup"><span data-stu-id="e7d63-130">Type</span></span>|<span data-ttu-id="e7d63-131">説明</span><span class="sxs-lookup"><span data-stu-id="e7d63-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d63-132">id</span><span class="sxs-lookup"><span data-stu-id="e7d63-132">id</span></span>|<span data-ttu-id="e7d63-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e7d63-133">String</span></span>|<span data-ttu-id="e7d63-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e7d63-134">Key of the entity.</span></span> <span data-ttu-id="e7d63-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d63-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7d63-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d63-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e7d63-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7d63-137">DateTimeOffset</span></span>|<span data-ttu-id="e7d63-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="e7d63-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e7d63-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d63-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7d63-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e7d63-140">roleScopeTagIds</span></span>|<span data-ttu-id="e7d63-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e7d63-141">String collection</span></span>|<span data-ttu-id="e7d63-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="e7d63-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e7d63-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d63-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7d63-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e7d63-144">supportsScopeTags</span></span>|<span data-ttu-id="e7d63-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-145">Boolean</span></span>|<span data-ttu-id="e7d63-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e7d63-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="e7d63-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e7d63-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="e7d63-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e7d63-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-149">This property is read-only.</span></span> <span data-ttu-id="e7d63-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d63-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7d63-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d63-151">createdDateTime</span></span>|<span data-ttu-id="e7d63-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7d63-152">DateTimeOffset</span></span>|<span data-ttu-id="e7d63-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e7d63-153">DateTime the object was created.</span></span> <span data-ttu-id="e7d63-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d63-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7d63-155">説明</span><span class="sxs-lookup"><span data-stu-id="e7d63-155">description</span></span>|<span data-ttu-id="e7d63-156">String</span><span class="sxs-lookup"><span data-stu-id="e7d63-156">String</span></span>|<span data-ttu-id="e7d63-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="e7d63-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e7d63-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d63-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7d63-159">displayName</span><span class="sxs-lookup"><span data-stu-id="e7d63-159">displayName</span></span>|<span data-ttu-id="e7d63-160">String</span><span class="sxs-lookup"><span data-stu-id="e7d63-160">String</span></span>|<span data-ttu-id="e7d63-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="e7d63-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e7d63-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d63-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7d63-163">version</span><span class="sxs-lookup"><span data-stu-id="e7d63-163">version</span></span>|<span data-ttu-id="e7d63-164">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-164">Int32</span></span>|<span data-ttu-id="e7d63-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="e7d63-165">Version of the device configuration.</span></span> <span data-ttu-id="e7d63-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d63-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e7d63-167">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e7d63-167">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e7d63-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-168">Boolean</span></span>|<span data-ttu-id="e7d63-169">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-169">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e7d63-170">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e7d63-170">passwordBlockTrustAgents</span></span>|<span data-ttu-id="e7d63-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-171">Boolean</span></span>|<span data-ttu-id="e7d63-172">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-172">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="e7d63-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e7d63-173">passwordExpirationDays</span></span>|<span data-ttu-id="e7d63-174">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-174">Int32</span></span>|<span data-ttu-id="e7d63-175">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-175">Number of days before the password expires.</span></span> <span data-ttu-id="e7d63-176">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-176">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e7d63-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e7d63-177">passwordMinimumLength</span></span>|<span data-ttu-id="e7d63-178">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-178">Int32</span></span>|<span data-ttu-id="e7d63-179">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="e7d63-179">Minimum length of passwords.</span></span> <span data-ttu-id="e7d63-180">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-180">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e7d63-181">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e7d63-181">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e7d63-182">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-182">Int32</span></span>|<span data-ttu-id="e7d63-183">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="e7d63-183">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e7d63-184">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e7d63-184">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e7d63-185">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-185">Int32</span></span>|<span data-ttu-id="e7d63-186">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-186">Number of previous passwords to block.</span></span> <span data-ttu-id="e7d63-187">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-187">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e7d63-188">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e7d63-188">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e7d63-189">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-189">Int32</span></span>|<span data-ttu-id="e7d63-190">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-190">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="e7d63-191">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e7d63-192">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e7d63-192">passwordRequiredType</span></span>|[<span data-ttu-id="e7d63-193">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e7d63-193">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="e7d63-194">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="e7d63-194">Type of password that is required.</span></span> <span data-ttu-id="e7d63-195">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="e7d63-195">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e7d63-196">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e7d63-196">workProfileDataSharingType</span></span>|[<span data-ttu-id="e7d63-197">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e7d63-197">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="e7d63-198">許可されているデータ共有の種類。</span><span class="sxs-lookup"><span data-stu-id="e7d63-198">Type of data sharing that is allowed.</span></span> <span data-ttu-id="e7d63-199">可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="e7d63-199">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="e7d63-200">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e7d63-200">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="e7d63-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-201">Boolean</span></span>|<span data-ttu-id="e7d63-202">デバイスがロックされているときに通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-202">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="e7d63-203">ワークワークプロファイルのアカウント</span><span class="sxs-lookup"><span data-stu-id="e7d63-203">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="e7d63-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-204">Boolean</span></span>|<span data-ttu-id="e7d63-205">ユーザーが作業プロファイルでアカウントを追加または削除することを禁止します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-205">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="e7d63-206">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="e7d63-206">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="e7d63-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-207">Boolean</span></span>|<span data-ttu-id="e7d63-208">bluetooth デバイスがエンタープライズの連絡先にアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="e7d63-208">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="e7d63-209">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="e7d63-209">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="e7d63-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-210">Boolean</span></span>|<span data-ttu-id="e7d63-211">作業プロファイルの画面キャプチャをブロックします。</span><span class="sxs-lookup"><span data-stu-id="e7d63-211">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="e7d63-212">work profileblockクロスバープロファイル ecallerid</span><span class="sxs-lookup"><span data-stu-id="e7d63-212">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="e7d63-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-213">Boolean</span></span>|<span data-ttu-id="e7d63-214">[ブロック表示作業プロファイルの発信者番号を個人プロファイルに表示する。</span><span class="sxs-lookup"><span data-stu-id="e7d63-214">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="e7d63-215">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="e7d63-215">workProfileBlockCamera</span></span>|<span data-ttu-id="e7d63-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-216">Boolean</span></span>|<span data-ttu-id="e7d63-217">作業プロファイルカメラをブロックします。</span><span class="sxs-lookup"><span data-stu-id="e7d63-217">Block work profile camera.</span></span>|
|<span data-ttu-id="e7d63-218">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="e7d63-218">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="e7d63-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-219">Boolean</span></span>|<span data-ttu-id="e7d63-220">個人用プロファイルでの作業プロファイルの連絡先の使用を禁止します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-220">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="e7d63-221">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="e7d63-221">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="e7d63-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-222">Boolean</span></span>|<span data-ttu-id="e7d63-223">[クロスプロファイルコピー/貼り付けを許可する] の設定が有効になっているかどうかを示すブール値。</span><span class="sxs-lookup"><span data-stu-id="e7d63-223">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="e7d63-224">work profiledefaultapppermissionpolicy</span><span class="sxs-lookup"><span data-stu-id="e7d63-224">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="e7d63-225">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e7d63-225">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="e7d63-226">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="e7d63-226">Type of password that is required.</span></span> <span data-ttu-id="e7d63-227">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="e7d63-227">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e7d63-228">。 workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="e7d63-228">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e7d63-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-229">Boolean</span></span>|<span data-ttu-id="e7d63-230">ワークプロファイルの指紋のロック解除をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-230">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="e7d63-231">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e7d63-231">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="e7d63-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-232">Boolean</span></span>|<span data-ttu-id="e7d63-233">ワークプロファイルのスマートロックおよびその他の信頼エージェントを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-233">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="e7d63-234">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e7d63-234">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="e7d63-235">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-235">Int32</span></span>|<span data-ttu-id="e7d63-236">作業プロファイルのパスワードが期限切れになるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-236">Number of days before the work profile password expires.</span></span> <span data-ttu-id="e7d63-237">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-237">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e7d63-238">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e7d63-238">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="e7d63-239">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-239">Int32</span></span>|<span data-ttu-id="e7d63-240">ワークプロファイルのパスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="e7d63-240">Minimum length of work profile password.</span></span> <span data-ttu-id="e7d63-241">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-241">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e7d63-242">ワークプロファイルのパスワード minnumericcharacters</span><span class="sxs-lookup"><span data-stu-id="e7d63-242">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="e7d63-243">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-243">Int32</span></span>|<span data-ttu-id="e7d63-244">作業プロファイルのパスワードに必要な数字の最小数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-244">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="e7d63-245">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e7d63-246">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e7d63-246">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="e7d63-247">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-247">Int32</span></span>|<span data-ttu-id="e7d63-248">作業プロファイルのパスワードに必要な文字以外の文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="e7d63-248">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="e7d63-249">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e7d63-250">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e7d63-250">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="e7d63-251">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-251">Int32</span></span>|<span data-ttu-id="e7d63-252">作業プロファイルのパスワードに必要な文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="e7d63-252">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="e7d63-253">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e7d63-254">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e7d63-254">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="e7d63-255">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-255">Int32</span></span>|<span data-ttu-id="e7d63-256">作業プロファイルのパスワードに必要な小文字の最小文字数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-256">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="e7d63-257">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e7d63-258">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e7d63-258">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="e7d63-259">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-259">Int32</span></span>|<span data-ttu-id="e7d63-260">作業プロファイルのパスワードに必要な大文字と小文字の最小値。</span><span class="sxs-lookup"><span data-stu-id="e7d63-260">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="e7d63-261">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e7d63-262">ワークスペースのパスワードを入力する</span><span class="sxs-lookup"><span data-stu-id="e7d63-262">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="e7d63-263">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-263">Int32</span></span>|<span data-ttu-id="e7d63-264">作業プロファイルのパスワードに必要な記号の最小数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-264">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="e7d63-265">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e7d63-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e7d63-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e7d63-267">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-267">Int32</span></span>|<span data-ttu-id="e7d63-268">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="e7d63-268">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e7d63-269">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e7d63-269">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e7d63-270">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-270">Int32</span></span>|<span data-ttu-id="e7d63-271">ブロックする、以前の作業プロファイルのパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-271">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="e7d63-272">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-272">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e7d63-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e7d63-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e7d63-274">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d63-274">Int32</span></span>|<span data-ttu-id="e7d63-275">作業プロファイルが削除され、すべての企業データが削除されるまでに許可されるサインイン失敗回数。</span><span class="sxs-lookup"><span data-stu-id="e7d63-275">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="e7d63-276">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="e7d63-276">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e7d63-277">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e7d63-277">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="e7d63-278">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e7d63-278">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="e7d63-279">必要な業務プロファイルのパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="e7d63-279">Type of work profile password that is required.</span></span> <span data-ttu-id="e7d63-280">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="e7d63-280">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e7d63-281">次</span><span class="sxs-lookup"><span data-stu-id="e7d63-281">workProfileRequirePassword</span></span>|<span data-ttu-id="e7d63-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-282">Boolean</span></span>|<span data-ttu-id="e7d63-283">パスワードが必要です。または職場プロファイルでは使用できません</span><span class="sxs-lookup"><span data-stu-id="e7d63-283">Password is required or not for work profile</span></span>|
|<span data-ttu-id="e7d63-284">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e7d63-284">securityRequireVerifyApps</span></span>|<span data-ttu-id="e7d63-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-285">Boolean</span></span>|<span data-ttu-id="e7d63-286">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-286">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="e7d63-287">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="e7d63-287">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="e7d63-288">String</span><span class="sxs-lookup"><span data-stu-id="e7d63-288">String</span></span>|<span data-ttu-id="e7d63-289">always on VPN のロックダウンモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="e7d63-289">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="e7d63-290">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="e7d63-290">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="e7d63-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d63-291">Boolean</span></span>|<span data-ttu-id="e7d63-292">always on VPN のロックダウンモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="e7d63-292">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="e7d63-293">応答</span><span class="sxs-lookup"><span data-stu-id="e7d63-293">Response</span></span>
<span data-ttu-id="e7d63-294">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidwork profileの devic/](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7d63-294">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7d63-295">例</span><span class="sxs-lookup"><span data-stu-id="e7d63-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7d63-296">要求</span><span class="sxs-lookup"><span data-stu-id="e7d63-296">Request</span></span>
<span data-ttu-id="e7d63-297">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7d63-297">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="e7d63-298">応答</span><span class="sxs-lookup"><span data-stu-id="e7d63-298">Response</span></span>
<span data-ttu-id="e7d63-p128">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7d63-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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





