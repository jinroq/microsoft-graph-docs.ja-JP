---
title: androidwork profile、devic/デバイスの更新
description: androidwork profile、devic/オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7568bd59aa728391779dda6ee24a5e15d5c165ea
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32519921"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="2f2dc-103">androidwork profile、devic/デバイスの更新</span><span class="sxs-lookup"><span data-stu-id="2f2dc-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="2f2dc-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f2dc-105">[androidwork profile、devic/](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2f2dc-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2f2dc-106">Prerequisites</span></span>
<span data-ttu-id="2f2dc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f2dc-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2f2dc-109">Permission type</span></span>|<span data-ttu-id="2f2dc-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2f2dc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2f2dc-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2f2dc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2f2dc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2dc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2f2dc-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2f2dc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2f2dc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-114">Not supported.</span></span>|
|<span data-ttu-id="2f2dc-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2f2dc-115">Application</span></span>|<span data-ttu-id="2f2dc-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2f2dc-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2f2dc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2f2dc-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f2dc-118">Request headers</span></span>
|<span data-ttu-id="2f2dc-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2f2dc-119">Header</span></span>|<span data-ttu-id="2f2dc-120">値</span><span class="sxs-lookup"><span data-stu-id="2f2dc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2f2dc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f2dc-121">Authorization</span></span>|<span data-ttu-id="2f2dc-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2f2dc-123">承諾</span><span class="sxs-lookup"><span data-stu-id="2f2dc-123">Accept</span></span>|<span data-ttu-id="2f2dc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f2dc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2f2dc-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2f2dc-125">Request body</span></span>
<span data-ttu-id="2f2dc-126">要求本文で、 [androidwork profileの devic/devicオブジェクト](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="2f2dc-127">次の表に、 [androidwork profile[devic]](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="2f2dc-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f2dc-128">Property</span></span>|<span data-ttu-id="2f2dc-129">型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-129">Type</span></span>|<span data-ttu-id="2f2dc-130">説明</span><span class="sxs-lookup"><span data-stu-id="2f2dc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f2dc-131">id</span><span class="sxs-lookup"><span data-stu-id="2f2dc-131">id</span></span>|<span data-ttu-id="2f2dc-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2f2dc-132">String</span></span>|<span data-ttu-id="2f2dc-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-133">Key of the entity.</span></span> <span data-ttu-id="2f2dc-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f2dc-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f2dc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f2dc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="2f2dc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f2dc-136">DateTimeOffset</span></span>|<span data-ttu-id="2f2dc-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-137">DateTime the object was last modified.</span></span> <span data-ttu-id="2f2dc-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f2dc-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f2dc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f2dc-139">createdDateTime</span></span>|<span data-ttu-id="2f2dc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f2dc-140">DateTimeOffset</span></span>|<span data-ttu-id="2f2dc-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-141">DateTime the object was created.</span></span> <span data-ttu-id="2f2dc-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f2dc-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f2dc-143">説明</span><span class="sxs-lookup"><span data-stu-id="2f2dc-143">description</span></span>|<span data-ttu-id="2f2dc-144">String</span><span class="sxs-lookup"><span data-stu-id="2f2dc-144">String</span></span>|<span data-ttu-id="2f2dc-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2f2dc-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f2dc-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f2dc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="2f2dc-147">displayName</span></span>|<span data-ttu-id="2f2dc-148">String</span><span class="sxs-lookup"><span data-stu-id="2f2dc-148">String</span></span>|<span data-ttu-id="2f2dc-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2f2dc-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f2dc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f2dc-151">version</span><span class="sxs-lookup"><span data-stu-id="2f2dc-151">version</span></span>|<span data-ttu-id="2f2dc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-152">Int32</span></span>|<span data-ttu-id="2f2dc-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-153">Version of the device configuration.</span></span> <span data-ttu-id="2f2dc-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f2dc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2f2dc-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="2f2dc-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2f2dc-156">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-156">Boolean</span></span>|<span data-ttu-id="2f2dc-157">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="2f2dc-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2f2dc-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="2f2dc-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f2dc-159">Boolean</span></span>|<span data-ttu-id="2f2dc-160">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="2f2dc-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2f2dc-161">passwordExpirationDays</span></span>|<span data-ttu-id="2f2dc-162">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-162">Int32</span></span>|<span data-ttu-id="2f2dc-163">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-163">Number of days before the password expires.</span></span> <span data-ttu-id="2f2dc-164">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2f2dc-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2f2dc-165">passwordMinimumLength</span></span>|<span data-ttu-id="2f2dc-166">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-166">Int32</span></span>|<span data-ttu-id="2f2dc-167">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-167">Minimum length of passwords.</span></span> <span data-ttu-id="2f2dc-168">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2f2dc-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2f2dc-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2f2dc-170">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-170">Int32</span></span>|<span data-ttu-id="2f2dc-171">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2f2dc-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2f2dc-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2f2dc-173">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-173">Int32</span></span>|<span data-ttu-id="2f2dc-174">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-174">Number of previous passwords to block.</span></span> <span data-ttu-id="2f2dc-175">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2f2dc-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2f2dc-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2f2dc-177">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-177">Int32</span></span>|<span data-ttu-id="2f2dc-178">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="2f2dc-179">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2f2dc-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2f2dc-180">passwordRequiredType</span></span>|[<span data-ttu-id="2f2dc-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2f2dc-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2f2dc-182">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-182">Type of password that is required.</span></span> <span data-ttu-id="2f2dc-183">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2f2dc-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2f2dc-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="2f2dc-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="2f2dc-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="2f2dc-186">許可されているデータ共有の種類。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="2f2dc-187">可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="2f2dc-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="2f2dc-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="2f2dc-189">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-189">Boolean</span></span>|<span data-ttu-id="2f2dc-190">デバイスがロックされているときに通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="2f2dc-191">ワークワークプロファイルのアカウント</span><span class="sxs-lookup"><span data-stu-id="2f2dc-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="2f2dc-192">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-192">Boolean</span></span>|<span data-ttu-id="2f2dc-193">ユーザーが作業プロファイルでアカウントを追加または削除することを禁止します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="2f2dc-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="2f2dc-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="2f2dc-195">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-195">Boolean</span></span>|<span data-ttu-id="2f2dc-196">bluetooth デバイスがエンタープライズの連絡先にアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="2f2dc-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="2f2dc-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="2f2dc-198">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-198">Boolean</span></span>|<span data-ttu-id="2f2dc-199">作業プロファイルの画面キャプチャをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="2f2dc-200">work profileblockクロスバープロファイル ecallerid</span><span class="sxs-lookup"><span data-stu-id="2f2dc-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="2f2dc-201">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-201">Boolean</span></span>|<span data-ttu-id="2f2dc-202">[ブロック表示作業プロファイルの発信者番号を個人プロファイルに表示する。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="2f2dc-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="2f2dc-203">workProfileBlockCamera</span></span>|<span data-ttu-id="2f2dc-204">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-204">Boolean</span></span>|<span data-ttu-id="2f2dc-205">作業プロファイルカメラをブロックします。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-205">Block work profile camera.</span></span>|
|<span data-ttu-id="2f2dc-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="2f2dc-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="2f2dc-207">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-207">Boolean</span></span>|<span data-ttu-id="2f2dc-208">個人用プロファイルでの作業プロファイルの連絡先の使用を禁止します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="2f2dc-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="2f2dc-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="2f2dc-210">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-210">Boolean</span></span>|<span data-ttu-id="2f2dc-211">[クロスプロファイルコピー/貼り付けを許可する] の設定が有効になっているかどうかを示すブール値。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="2f2dc-212">work profiledefaultapppermissionpolicy</span><span class="sxs-lookup"><span data-stu-id="2f2dc-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="2f2dc-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="2f2dc-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="2f2dc-214">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-214">Type of password that is required.</span></span> <span data-ttu-id="2f2dc-215">可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="2f2dc-216">。 workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="2f2dc-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="2f2dc-217">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-217">Boolean</span></span>|<span data-ttu-id="2f2dc-218">ワークプロファイルの指紋のロック解除をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="2f2dc-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="2f2dc-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="2f2dc-220">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-220">Boolean</span></span>|<span data-ttu-id="2f2dc-221">ワークプロファイルのスマートロックおよびその他の信頼エージェントを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="2f2dc-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="2f2dc-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="2f2dc-223">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-223">Int32</span></span>|<span data-ttu-id="2f2dc-224">作業プロファイルのパスワードが期限切れになるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="2f2dc-225">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="2f2dc-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="2f2dc-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="2f2dc-227">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-227">Int32</span></span>|<span data-ttu-id="2f2dc-228">ワークプロファイルのパスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-228">Minimum length of work profile password.</span></span> <span data-ttu-id="2f2dc-229">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="2f2dc-230">ワークプロファイルのパスワード minnumericcharacters</span><span class="sxs-lookup"><span data-stu-id="2f2dc-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="2f2dc-231">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-231">Int32</span></span>|<span data-ttu-id="2f2dc-232">作業プロファイルのパスワードに必要な数字の最小数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="2f2dc-233">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f2dc-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2f2dc-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="2f2dc-235">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-235">Int32</span></span>|<span data-ttu-id="2f2dc-236">作業プロファイルのパスワードに必要な文字以外の文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="2f2dc-237">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f2dc-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="2f2dc-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="2f2dc-239">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-239">Int32</span></span>|<span data-ttu-id="2f2dc-240">作業プロファイルのパスワードに必要な文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="2f2dc-241">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f2dc-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2f2dc-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="2f2dc-243">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-243">Int32</span></span>|<span data-ttu-id="2f2dc-244">作業プロファイルのパスワードに必要な小文字の最小文字数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="2f2dc-245">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f2dc-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="2f2dc-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="2f2dc-247">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-247">Int32</span></span>|<span data-ttu-id="2f2dc-248">作業プロファイルのパスワードに必要な大文字と小文字の最小値。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="2f2dc-249">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f2dc-250">ワークスペースのパスワードを入力する</span><span class="sxs-lookup"><span data-stu-id="2f2dc-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="2f2dc-251">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-251">Int32</span></span>|<span data-ttu-id="2f2dc-252">作業プロファイルのパスワードに必要な記号の最小数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="2f2dc-253">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="2f2dc-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="2f2dc-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="2f2dc-255">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-255">Int32</span></span>|<span data-ttu-id="2f2dc-256">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="2f2dc-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="2f2dc-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="2f2dc-258">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-258">Int32</span></span>|<span data-ttu-id="2f2dc-259">ブロックする、以前の作業プロファイルのパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="2f2dc-260">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="2f2dc-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="2f2dc-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="2f2dc-262">Int32</span><span class="sxs-lookup"><span data-stu-id="2f2dc-262">Int32</span></span>|<span data-ttu-id="2f2dc-263">作業プロファイルが削除され、すべての企業データが削除されるまでに許可されるサインイン失敗回数。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="2f2dc-264">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="2f2dc-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="2f2dc-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="2f2dc-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="2f2dc-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="2f2dc-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="2f2dc-267">必要な業務プロファイルのパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-267">Type of work profile password that is required.</span></span> <span data-ttu-id="2f2dc-268">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="2f2dc-269">次</span><span class="sxs-lookup"><span data-stu-id="2f2dc-269">workProfileRequirePassword</span></span>|<span data-ttu-id="2f2dc-270">ブール型</span><span class="sxs-lookup"><span data-stu-id="2f2dc-270">Boolean</span></span>|<span data-ttu-id="2f2dc-271">パスワードが必要です。または職場プロファイルでは使用できません</span><span class="sxs-lookup"><span data-stu-id="2f2dc-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="2f2dc-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="2f2dc-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="2f2dc-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="2f2dc-273">Boolean</span></span>|<span data-ttu-id="2f2dc-274">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="2f2dc-275">応答</span><span class="sxs-lookup"><span data-stu-id="2f2dc-275">Response</span></span>
<span data-ttu-id="2f2dc-276">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[androidwork profileprofiledevicオブジェクト](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f2dc-277">例</span><span class="sxs-lookup"><span data-stu-id="2f2dc-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="2f2dc-278">要求</span><span class="sxs-lookup"><span data-stu-id="2f2dc-278">Request</span></span>
<span data-ttu-id="2f2dc-279">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-279">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="2f2dc-280">応答</span><span class="sxs-lookup"><span data-stu-id="2f2dc-280">Response</span></span>
<span data-ttu-id="2f2dc-p126">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2f2dc-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "securityRequireVerifyApps": true
}
```



