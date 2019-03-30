---
title: androidwork profileて devicの種類を作成する
description: 新しい androidwork profileの devic/オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d6cce3fa9a874cbd6e055dc89e0e2a7ea624cf47
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30988204"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="4aec2-103">androidwork profileて devicの種類を作成する</span><span class="sxs-lookup"><span data-stu-id="4aec2-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="4aec2-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4aec2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4aec2-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4aec2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4aec2-106">新しい[androidwork profileの devic/](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4aec2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4aec2-107">Prerequisites</span></span>
<span data-ttu-id="4aec2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4aec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4aec2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4aec2-110">Permission type</span></span>|<span data-ttu-id="4aec2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4aec2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4aec2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4aec2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4aec2-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4aec2-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4aec2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4aec2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4aec2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4aec2-115">Not supported.</span></span>|
|<span data-ttu-id="4aec2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4aec2-116">Application</span></span>|<span data-ttu-id="4aec2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4aec2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4aec2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4aec2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4aec2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4aec2-119">Request headers</span></span>
|<span data-ttu-id="4aec2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4aec2-120">Header</span></span>|<span data-ttu-id="4aec2-121">値</span><span class="sxs-lookup"><span data-stu-id="4aec2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4aec2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4aec2-122">Authorization</span></span>|<span data-ttu-id="4aec2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4aec2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4aec2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4aec2-124">Accept</span></span>|<span data-ttu-id="4aec2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4aec2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4aec2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4aec2-126">Request body</span></span>
<span data-ttu-id="4aec2-127">要求本文で、androidwork profileの devic/devicオブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="4aec2-128">次の表に、androidwork profile[devic] の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="4aec2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4aec2-129">Property</span></span>|<span data-ttu-id="4aec2-130">型</span><span class="sxs-lookup"><span data-stu-id="4aec2-130">Type</span></span>|<span data-ttu-id="4aec2-131">説明</span><span class="sxs-lookup"><span data-stu-id="4aec2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4aec2-132">id</span><span class="sxs-lookup"><span data-stu-id="4aec2-132">id</span></span>|<span data-ttu-id="4aec2-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4aec2-133">String</span></span>|<span data-ttu-id="4aec2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4aec2-134">Key of the entity.</span></span> <span data-ttu-id="4aec2-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4aec2-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4aec2-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4aec2-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4aec2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4aec2-137">DateTimeOffset</span></span>|<span data-ttu-id="4aec2-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="4aec2-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4aec2-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4aec2-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4aec2-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4aec2-140">roleScopeTagIds</span></span>|<span data-ttu-id="4aec2-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4aec2-141">String collection</span></span>|<span data-ttu-id="4aec2-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="4aec2-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4aec2-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4aec2-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4aec2-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4aec2-144">supportsScopeTags</span></span>|<span data-ttu-id="4aec2-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-145">Boolean</span></span>|<span data-ttu-id="4aec2-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4aec2-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="4aec2-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4aec2-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="4aec2-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4aec2-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-149">This property is read-only.</span></span> <span data-ttu-id="4aec2-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4aec2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4aec2-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4aec2-151">createdDateTime</span></span>|<span data-ttu-id="4aec2-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4aec2-152">DateTimeOffset</span></span>|<span data-ttu-id="4aec2-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4aec2-153">DateTime the object was created.</span></span> <span data-ttu-id="4aec2-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4aec2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4aec2-155">description</span><span class="sxs-lookup"><span data-stu-id="4aec2-155">description</span></span>|<span data-ttu-id="4aec2-156">String</span><span class="sxs-lookup"><span data-stu-id="4aec2-156">String</span></span>|<span data-ttu-id="4aec2-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="4aec2-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4aec2-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4aec2-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4aec2-159">displayName</span><span class="sxs-lookup"><span data-stu-id="4aec2-159">displayName</span></span>|<span data-ttu-id="4aec2-160">String</span><span class="sxs-lookup"><span data-stu-id="4aec2-160">String</span></span>|<span data-ttu-id="4aec2-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="4aec2-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4aec2-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4aec2-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4aec2-163">version</span><span class="sxs-lookup"><span data-stu-id="4aec2-163">version</span></span>|<span data-ttu-id="4aec2-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-164">Int32</span></span>|<span data-ttu-id="4aec2-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="4aec2-165">Version of the device configuration.</span></span> <span data-ttu-id="4aec2-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4aec2-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4aec2-167">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="4aec2-167">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="4aec2-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-168">Boolean</span></span>|<span data-ttu-id="4aec2-169">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-169">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="4aec2-170">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="4aec2-170">passwordBlockTrustAgents</span></span>|<span data-ttu-id="4aec2-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-171">Boolean</span></span>|<span data-ttu-id="4aec2-172">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-172">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="4aec2-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4aec2-173">passwordExpirationDays</span></span>|<span data-ttu-id="4aec2-174">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-174">Int32</span></span>|<span data-ttu-id="4aec2-175">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-175">Number of days before the password expires.</span></span> <span data-ttu-id="4aec2-176">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-176">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4aec2-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4aec2-177">passwordMinimumLength</span></span>|<span data-ttu-id="4aec2-178">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-178">Int32</span></span>|<span data-ttu-id="4aec2-179">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="4aec2-179">Minimum length of passwords.</span></span> <span data-ttu-id="4aec2-180">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-180">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4aec2-181">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4aec2-181">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4aec2-182">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-182">Int32</span></span>|<span data-ttu-id="4aec2-183">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="4aec2-183">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4aec2-184">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4aec2-184">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4aec2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-185">Int32</span></span>|<span data-ttu-id="4aec2-186">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-186">Number of previous passwords to block.</span></span> <span data-ttu-id="4aec2-187">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-187">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4aec2-188">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4aec2-188">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4aec2-189">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-189">Int32</span></span>|<span data-ttu-id="4aec2-190">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-190">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="4aec2-191">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4aec2-192">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4aec2-192">passwordRequiredType</span></span>|[<span data-ttu-id="4aec2-193">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4aec2-193">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="4aec2-194">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="4aec2-194">Type of password that is required.</span></span> <span data-ttu-id="4aec2-195">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="4aec2-195">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="4aec2-196">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="4aec2-196">workProfileDataSharingType</span></span>|[<span data-ttu-id="4aec2-197">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="4aec2-197">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="4aec2-198">許可されているデータ共有の種類。</span><span class="sxs-lookup"><span data-stu-id="4aec2-198">Type of data sharing that is allowed.</span></span> <span data-ttu-id="4aec2-199">可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="4aec2-199">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="4aec2-200">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="4aec2-200">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="4aec2-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-201">Boolean</span></span>|<span data-ttu-id="4aec2-202">デバイスがロックされているときに通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-202">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="4aec2-203">ワークワークプロファイルのアカウント</span><span class="sxs-lookup"><span data-stu-id="4aec2-203">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="4aec2-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-204">Boolean</span></span>|<span data-ttu-id="4aec2-205">ユーザーが作業プロファイルでアカウントを追加または削除することを禁止します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-205">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="4aec2-206">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="4aec2-206">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="4aec2-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-207">Boolean</span></span>|<span data-ttu-id="4aec2-208">bluetooth デバイスがエンタープライズの連絡先にアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="4aec2-208">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="4aec2-209">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="4aec2-209">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="4aec2-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-210">Boolean</span></span>|<span data-ttu-id="4aec2-211">作業プロファイルの画面キャプチャをブロックします。</span><span class="sxs-lookup"><span data-stu-id="4aec2-211">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="4aec2-212">work profileblockクロスバープロファイル ecallerid</span><span class="sxs-lookup"><span data-stu-id="4aec2-212">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="4aec2-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-213">Boolean</span></span>|<span data-ttu-id="4aec2-214">[ブロック表示作業プロファイルの発信者番号を個人プロファイルに表示する。</span><span class="sxs-lookup"><span data-stu-id="4aec2-214">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="4aec2-215">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="4aec2-215">workProfileBlockCamera</span></span>|<span data-ttu-id="4aec2-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-216">Boolean</span></span>|<span data-ttu-id="4aec2-217">作業プロファイルカメラをブロックします。</span><span class="sxs-lookup"><span data-stu-id="4aec2-217">Block work profile camera.</span></span>|
|<span data-ttu-id="4aec2-218">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="4aec2-218">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="4aec2-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-219">Boolean</span></span>|<span data-ttu-id="4aec2-220">個人用プロファイルでの作業プロファイルの連絡先の使用を禁止します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-220">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="4aec2-221">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="4aec2-221">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="4aec2-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-222">Boolean</span></span>|<span data-ttu-id="4aec2-223">[クロスプロファイルコピー/貼り付けを許可する] の設定が有効になっているかどうかを示すブール値。</span><span class="sxs-lookup"><span data-stu-id="4aec2-223">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="4aec2-224">work profiledefaultapppermissionpolicy</span><span class="sxs-lookup"><span data-stu-id="4aec2-224">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="4aec2-225">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="4aec2-225">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="4aec2-226">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="4aec2-226">Type of password that is required.</span></span> <span data-ttu-id="4aec2-227">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="4aec2-227">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="4aec2-228">。 workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="4aec2-228">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="4aec2-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-229">Boolean</span></span>|<span data-ttu-id="4aec2-230">ワークプロファイルの指紋のロック解除をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-230">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="4aec2-231">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="4aec2-231">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="4aec2-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-232">Boolean</span></span>|<span data-ttu-id="4aec2-233">ワークプロファイルのスマートロックおよびその他の信頼エージェントを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-233">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="4aec2-234">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4aec2-234">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="4aec2-235">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-235">Int32</span></span>|<span data-ttu-id="4aec2-236">作業プロファイルのパスワードが期限切れになるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-236">Number of days before the work profile password expires.</span></span> <span data-ttu-id="4aec2-237">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-237">Valid values 1 to 365</span></span>|
|<span data-ttu-id="4aec2-238">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4aec2-238">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="4aec2-239">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-239">Int32</span></span>|<span data-ttu-id="4aec2-240">ワークプロファイルのパスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="4aec2-240">Minimum length of work profile password.</span></span> <span data-ttu-id="4aec2-241">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-241">Valid values 4 to 16</span></span>|
|<span data-ttu-id="4aec2-242">ワークプロファイルのパスワード minnumericcharacters</span><span class="sxs-lookup"><span data-stu-id="4aec2-242">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="4aec2-243">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-243">Int32</span></span>|<span data-ttu-id="4aec2-244">作業プロファイルのパスワードに必要な数字の最小数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-244">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="4aec2-245">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4aec2-246">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="4aec2-246">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="4aec2-247">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-247">Int32</span></span>|<span data-ttu-id="4aec2-248">作業プロファイルのパスワードに必要な文字以外の文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="4aec2-248">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="4aec2-249">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4aec2-250">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="4aec2-250">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="4aec2-251">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-251">Int32</span></span>|<span data-ttu-id="4aec2-252">作業プロファイルのパスワードに必要な文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="4aec2-252">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="4aec2-253">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4aec2-254">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="4aec2-254">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="4aec2-255">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-255">Int32</span></span>|<span data-ttu-id="4aec2-256">作業プロファイルのパスワードに必要な小文字の最小文字数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-256">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="4aec2-257">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4aec2-258">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="4aec2-258">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="4aec2-259">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-259">Int32</span></span>|<span data-ttu-id="4aec2-260">作業プロファイルのパスワードに必要な大文字と小文字の最小値。</span><span class="sxs-lookup"><span data-stu-id="4aec2-260">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="4aec2-261">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4aec2-262">ワークスペースのパスワードを入力する</span><span class="sxs-lookup"><span data-stu-id="4aec2-262">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="4aec2-263">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-263">Int32</span></span>|<span data-ttu-id="4aec2-264">作業プロファイルのパスワードに必要な記号の最小数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-264">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="4aec2-265">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="4aec2-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4aec2-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4aec2-267">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-267">Int32</span></span>|<span data-ttu-id="4aec2-268">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="4aec2-268">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="4aec2-269">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4aec2-269">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4aec2-270">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-270">Int32</span></span>|<span data-ttu-id="4aec2-271">ブロックする、以前の作業プロファイルのパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-271">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="4aec2-272">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-272">Valid values 0 to 24</span></span>|
|<span data-ttu-id="4aec2-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="4aec2-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="4aec2-274">Int32</span><span class="sxs-lookup"><span data-stu-id="4aec2-274">Int32</span></span>|<span data-ttu-id="4aec2-275">作業プロファイルが削除され、すべての企業データが削除されるまでに許可されるサインイン失敗回数。</span><span class="sxs-lookup"><span data-stu-id="4aec2-275">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="4aec2-276">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="4aec2-276">Valid values 1 to 16</span></span>|
|<span data-ttu-id="4aec2-277">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4aec2-277">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="4aec2-278">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4aec2-278">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="4aec2-279">必要な業務プロファイルのパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="4aec2-279">Type of work profile password that is required.</span></span> <span data-ttu-id="4aec2-280">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="4aec2-280">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="4aec2-281">次</span><span class="sxs-lookup"><span data-stu-id="4aec2-281">workProfileRequirePassword</span></span>|<span data-ttu-id="4aec2-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-282">Boolean</span></span>|<span data-ttu-id="4aec2-283">パスワードが必要です。または職場プロファイルでは使用できません</span><span class="sxs-lookup"><span data-stu-id="4aec2-283">Password is required or not for work profile</span></span>|
|<span data-ttu-id="4aec2-284">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="4aec2-284">securityRequireVerifyApps</span></span>|<span data-ttu-id="4aec2-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-285">Boolean</span></span>|<span data-ttu-id="4aec2-286">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-286">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="4aec2-287">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="4aec2-287">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="4aec2-288">String</span><span class="sxs-lookup"><span data-stu-id="4aec2-288">String</span></span>|<span data-ttu-id="4aec2-289">always on VPN のロックダウンモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="4aec2-289">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="4aec2-290">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="4aec2-290">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="4aec2-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="4aec2-291">Boolean</span></span>|<span data-ttu-id="4aec2-292">always on VPN のロックダウンモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="4aec2-292">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="4aec2-293">応答</span><span class="sxs-lookup"><span data-stu-id="4aec2-293">Response</span></span>
<span data-ttu-id="4aec2-294">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidwork profileの devic/](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4aec2-294">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4aec2-295">例</span><span class="sxs-lookup"><span data-stu-id="4aec2-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="4aec2-296">要求</span><span class="sxs-lookup"><span data-stu-id="4aec2-296">Request</span></span>
<span data-ttu-id="4aec2-297">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4aec2-297">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4aec2-298">応答</span><span class="sxs-lookup"><span data-stu-id="4aec2-298">Response</span></span>
<span data-ttu-id="4aec2-p128">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4aec2-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




