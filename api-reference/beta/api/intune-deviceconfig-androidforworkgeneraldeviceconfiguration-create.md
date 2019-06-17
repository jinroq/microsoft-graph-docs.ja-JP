---
title: Androidforwork の各 Devicの作成
description: 新しい Androidforwork の Devic/オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 66e33e800250a182a1d25aba8d1952af98d19d33
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34970850"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="f5427-103">Androidforwork の各 Devicの作成</span><span class="sxs-lookup"><span data-stu-id="f5427-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f5427-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5427-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5427-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5427-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5427-106">新しい[Androidforwork](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)の devic/オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f5427-106">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5427-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f5427-107">Prerequisites</span></span>
<span data-ttu-id="f5427-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f5427-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5427-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f5427-110">Permission type</span></span>|<span data-ttu-id="f5427-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f5427-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5427-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f5427-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f5427-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5427-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5427-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f5427-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5427-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5427-115">Not supported.</span></span>|
|<span data-ttu-id="f5427-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f5427-116">Application</span></span>|<span data-ttu-id="f5427-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f5427-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5427-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f5427-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f5427-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5427-119">Request headers</span></span>
|<span data-ttu-id="f5427-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f5427-120">Header</span></span>|<span data-ttu-id="f5427-121">値</span><span class="sxs-lookup"><span data-stu-id="f5427-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5427-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5427-122">Authorization</span></span>|<span data-ttu-id="f5427-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f5427-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5427-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f5427-124">Accept</span></span>|<span data-ttu-id="f5427-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f5427-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5427-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f5427-126">Request body</span></span>
<span data-ttu-id="f5427-127">要求本文で、Androidforwork の Devic/オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f5427-127">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="f5427-128">次の表に、Androidforwork の各プロパティを作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f5427-128">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="f5427-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5427-129">Property</span></span>|<span data-ttu-id="f5427-130">型</span><span class="sxs-lookup"><span data-stu-id="f5427-130">Type</span></span>|<span data-ttu-id="f5427-131">説明</span><span class="sxs-lookup"><span data-stu-id="f5427-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5427-132">id</span><span class="sxs-lookup"><span data-stu-id="f5427-132">id</span></span>|<span data-ttu-id="f5427-133">文字列</span><span class="sxs-lookup"><span data-stu-id="f5427-133">String</span></span>|<span data-ttu-id="f5427-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f5427-134">Key of the entity.</span></span> <span data-ttu-id="f5427-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5427-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f5427-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5427-137">DateTimeOffset</span></span>|<span data-ttu-id="f5427-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="f5427-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f5427-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f5427-140">roleScopeTagIds</span></span>|<span data-ttu-id="f5427-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="f5427-141">String collection</span></span>|<span data-ttu-id="f5427-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="f5427-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f5427-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f5427-144">supportsScopeTags</span></span>|<span data-ttu-id="f5427-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-145">Boolean</span></span>|<span data-ttu-id="f5427-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5427-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f5427-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="f5427-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f5427-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="f5427-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f5427-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="f5427-149">This property is read-only.</span></span> <span data-ttu-id="f5427-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5427-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f5427-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5427-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f5427-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="f5427-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f5427-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5427-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f5427-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5427-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f5427-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f5427-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f5427-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f5427-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f5427-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="f5427-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f5427-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="f5427-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f5427-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5427-163">createdDateTime</span></span>|<span data-ttu-id="f5427-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5427-164">DateTimeOffset</span></span>|<span data-ttu-id="f5427-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="f5427-165">DateTime the object was created.</span></span> <span data-ttu-id="f5427-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-167">description</span><span class="sxs-lookup"><span data-stu-id="f5427-167">description</span></span>|<span data-ttu-id="f5427-168">String</span><span class="sxs-lookup"><span data-stu-id="f5427-168">String</span></span>|<span data-ttu-id="f5427-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="f5427-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f5427-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-171">displayName</span><span class="sxs-lookup"><span data-stu-id="f5427-171">displayName</span></span>|<span data-ttu-id="f5427-172">String</span><span class="sxs-lookup"><span data-stu-id="f5427-172">String</span></span>|<span data-ttu-id="f5427-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="f5427-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f5427-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-175">version</span><span class="sxs-lookup"><span data-stu-id="f5427-175">version</span></span>|<span data-ttu-id="f5427-176">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-176">Int32</span></span>|<span data-ttu-id="f5427-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="f5427-177">Version of the device configuration.</span></span> <span data-ttu-id="f5427-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="f5427-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5427-179">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f5427-179">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="f5427-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-180">Boolean</span></span>|<span data-ttu-id="f5427-181">指紋によるロック解除を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5427-181">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="f5427-182">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="f5427-182">passwordBlockTrustAgents</span></span>|<span data-ttu-id="f5427-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-183">Boolean</span></span>|<span data-ttu-id="f5427-184">Smart Lock や他の信頼エージェントをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5427-184">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="f5427-185">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f5427-185">passwordExpirationDays</span></span>|<span data-ttu-id="f5427-186">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-186">Int32</span></span>|<span data-ttu-id="f5427-187">パスワードの有効期限が切れるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="f5427-187">Number of days before the password expires.</span></span> <span data-ttu-id="f5427-188">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="f5427-188">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f5427-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f5427-189">passwordMinimumLength</span></span>|<span data-ttu-id="f5427-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-190">Int32</span></span>|<span data-ttu-id="f5427-191">パスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="f5427-191">Minimum length of passwords.</span></span> <span data-ttu-id="f5427-192">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="f5427-192">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f5427-193">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f5427-193">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f5427-194">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-194">Int32</span></span>|<span data-ttu-id="f5427-195">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="f5427-195">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f5427-196">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f5427-196">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f5427-197">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-197">Int32</span></span>|<span data-ttu-id="f5427-198">ブロックする、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="f5427-198">Number of previous passwords to block.</span></span> <span data-ttu-id="f5427-199">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="f5427-199">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f5427-200">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f5427-200">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f5427-201">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-201">Int32</span></span>|<span data-ttu-id="f5427-202">出荷時の設定にリセットされるまでの、失敗が許可されるサインインの回数。</span><span class="sxs-lookup"><span data-stu-id="f5427-202">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="f5427-203">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="f5427-203">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f5427-204">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f5427-204">passwordRequiredType</span></span>|[<span data-ttu-id="f5427-205">Androidforwork Requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="f5427-205">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="f5427-206">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="f5427-206">Type of password that is required.</span></span> <span data-ttu-id="f5427-207">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="f5427-207">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="f5427-208">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="f5427-208">workProfileDataSharingType</span></span>|[<span data-ttu-id="f5427-209">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="f5427-209">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="f5427-210">許可されているデータ共有の種類。</span><span class="sxs-lookup"><span data-stu-id="f5427-210">Type of data sharing that is allowed.</span></span> <span data-ttu-id="f5427-211">使用可能な値は、`deviceDefault`、`preventAny`、`allowPersonalToWork`、`noRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="f5427-211">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="f5427-212">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="f5427-212">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="f5427-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-213">Boolean</span></span>|<span data-ttu-id="f5427-214">デバイスがロックされているときに通知をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5427-214">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="f5427-215">ワークワークプロファイルのアカウント</span><span class="sxs-lookup"><span data-stu-id="f5427-215">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="f5427-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-216">Boolean</span></span>|<span data-ttu-id="f5427-217">ユーザーが作業プロファイルでアカウントを追加または削除することを禁止します。</span><span class="sxs-lookup"><span data-stu-id="f5427-217">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="f5427-218">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="f5427-218">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="f5427-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-219">Boolean</span></span>|<span data-ttu-id="f5427-220">Bluetooth デバイスがエンタープライズの連絡先にアクセスできるようにします。</span><span class="sxs-lookup"><span data-stu-id="f5427-220">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="f5427-221">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="f5427-221">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="f5427-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-222">Boolean</span></span>|<span data-ttu-id="f5427-223">作業プロファイルの画面キャプチャをブロックします。</span><span class="sxs-lookup"><span data-stu-id="f5427-223">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="f5427-224">work Profileblockクロスバープロファイル Ecallerid</span><span class="sxs-lookup"><span data-stu-id="f5427-224">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="f5427-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-225">Boolean</span></span>|<span data-ttu-id="f5427-226">[ブロック表示作業プロファイルの発信者番号を個人プロファイルに表示する。</span><span class="sxs-lookup"><span data-stu-id="f5427-226">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="f5427-227">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="f5427-227">workProfileBlockCamera</span></span>|<span data-ttu-id="f5427-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-228">Boolean</span></span>|<span data-ttu-id="f5427-229">作業プロファイルカメラをブロックします。</span><span class="sxs-lookup"><span data-stu-id="f5427-229">Block work profile camera.</span></span>|
|<span data-ttu-id="f5427-230">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="f5427-230">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="f5427-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-231">Boolean</span></span>|<span data-ttu-id="f5427-232">個人用プロファイルでの作業プロファイルの連絡先の使用を禁止します。</span><span class="sxs-lookup"><span data-stu-id="f5427-232">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="f5427-233">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="f5427-233">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="f5427-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-234">Boolean</span></span>|<span data-ttu-id="f5427-235">[クロスプロファイルコピー/貼り付けを許可する] の設定が有効になっているかどうかを示すブール値。</span><span class="sxs-lookup"><span data-stu-id="f5427-235">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="f5427-236">work Profiledefaultapppermissionpolicy</span><span class="sxs-lookup"><span data-stu-id="f5427-236">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="f5427-237">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="f5427-237">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="f5427-238">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="f5427-238">Type of password that is required.</span></span> <span data-ttu-id="f5427-239">使用可能な値は、`deviceDefault`、`prompt`、`autoGrant`、`autoDeny` です。</span><span class="sxs-lookup"><span data-stu-id="f5427-239">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="f5427-240">。 Workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="f5427-240">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="f5427-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-241">Boolean</span></span>|<span data-ttu-id="f5427-242">ワークプロファイルの指紋のロック解除をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5427-242">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="f5427-243">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="f5427-243">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="f5427-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-244">Boolean</span></span>|<span data-ttu-id="f5427-245">ワークプロファイルのスマートロックおよびその他の信頼エージェントを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="f5427-245">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="f5427-246">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f5427-246">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="f5427-247">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-247">Int32</span></span>|<span data-ttu-id="f5427-248">作業プロファイルのパスワードが期限切れになるまでの日数。</span><span class="sxs-lookup"><span data-stu-id="f5427-248">Number of days before the work profile password expires.</span></span> <span data-ttu-id="f5427-249">有効な値は 1 から 365 までです</span><span class="sxs-lookup"><span data-stu-id="f5427-249">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f5427-250">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f5427-250">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="f5427-251">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-251">Int32</span></span>|<span data-ttu-id="f5427-252">ワークプロファイルのパスワードの最小の長さ。</span><span class="sxs-lookup"><span data-stu-id="f5427-252">Minimum length of work profile password.</span></span> <span data-ttu-id="f5427-253">有効な値は 4 から 16 までです</span><span class="sxs-lookup"><span data-stu-id="f5427-253">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f5427-254">ワークプロファイルのパスワード Minnumericcharacters</span><span class="sxs-lookup"><span data-stu-id="f5427-254">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="f5427-255">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-255">Int32</span></span>|<span data-ttu-id="f5427-256">作業プロファイルのパスワードに必要な数字の最小数。</span><span class="sxs-lookup"><span data-stu-id="f5427-256">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="f5427-257">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="f5427-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f5427-258">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f5427-258">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="f5427-259">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-259">Int32</span></span>|<span data-ttu-id="f5427-260">作業プロファイルのパスワードに必要な文字以外の文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="f5427-260">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="f5427-261">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="f5427-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f5427-262">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f5427-262">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="f5427-263">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-263">Int32</span></span>|<span data-ttu-id="f5427-264">作業プロファイルのパスワードに必要な文字数の最小値。</span><span class="sxs-lookup"><span data-stu-id="f5427-264">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="f5427-265">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="f5427-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f5427-266">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f5427-266">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="f5427-267">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-267">Int32</span></span>|<span data-ttu-id="f5427-268">作業プロファイルのパスワードに必要な小文字の最小文字数。</span><span class="sxs-lookup"><span data-stu-id="f5427-268">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="f5427-269">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="f5427-269">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f5427-270">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f5427-270">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="f5427-271">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-271">Int32</span></span>|<span data-ttu-id="f5427-272">作業プロファイルのパスワードに必要な大文字と小文字の最小値。</span><span class="sxs-lookup"><span data-stu-id="f5427-272">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="f5427-273">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="f5427-273">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f5427-274">ワークスペースのパスワードを入力する</span><span class="sxs-lookup"><span data-stu-id="f5427-274">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="f5427-275">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-275">Int32</span></span>|<span data-ttu-id="f5427-276">作業プロファイルのパスワードに必要な記号の最小数。</span><span class="sxs-lookup"><span data-stu-id="f5427-276">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="f5427-277">有効な値は1から10までです</span><span class="sxs-lookup"><span data-stu-id="f5427-277">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f5427-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f5427-278">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f5427-279">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-279">Int32</span></span>|<span data-ttu-id="f5427-280">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="f5427-280">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f5427-281">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f5427-281">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f5427-282">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-282">Int32</span></span>|<span data-ttu-id="f5427-283">ブロックする、以前の作業プロファイルのパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="f5427-283">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="f5427-284">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="f5427-284">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f5427-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f5427-285">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f5427-286">Int32</span><span class="sxs-lookup"><span data-stu-id="f5427-286">Int32</span></span>|<span data-ttu-id="f5427-287">作業プロファイルが削除され、すべての企業データが削除されるまでに許可されるサインイン失敗回数。</span><span class="sxs-lookup"><span data-stu-id="f5427-287">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="f5427-288">有効な値は1から16までです</span><span class="sxs-lookup"><span data-stu-id="f5427-288">Valid values 1 to 16</span></span>|
|<span data-ttu-id="f5427-289">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f5427-289">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="f5427-290">Androidforwork Requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="f5427-290">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="f5427-291">必要な業務プロファイルのパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="f5427-291">Type of work profile password that is required.</span></span> <span data-ttu-id="f5427-292">可能な値は、`deviceDefault`、`lowSecurityBiometric`、`required`、`atLeastNumeric`、`numericComplex`、`atLeastAlphabetic`、`atLeastAlphanumeric`、`alphanumericWithSymbols` です。</span><span class="sxs-lookup"><span data-stu-id="f5427-292">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="f5427-293">次</span><span class="sxs-lookup"><span data-stu-id="f5427-293">workProfileRequirePassword</span></span>|<span data-ttu-id="f5427-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-294">Boolean</span></span>|<span data-ttu-id="f5427-295">パスワードが必要です。または職場プロファイルでは使用できません</span><span class="sxs-lookup"><span data-stu-id="f5427-295">Password is required or not for work profile</span></span>|
|<span data-ttu-id="f5427-296">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f5427-296">securityRequireVerifyApps</span></span>|<span data-ttu-id="f5427-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-297">Boolean</span></span>|<span data-ttu-id="f5427-298">Android の検証アプリ機能をオンにするよう要求します。</span><span class="sxs-lookup"><span data-stu-id="f5427-298">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="f5427-299">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="f5427-299">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="f5427-300">String</span><span class="sxs-lookup"><span data-stu-id="f5427-300">String</span></span>|<span data-ttu-id="f5427-301">Always on VPN のロックダウンモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f5427-301">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="f5427-302">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="f5427-302">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="f5427-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5427-303">Boolean</span></span>|<span data-ttu-id="f5427-304">Always on VPN のロックダウンモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="f5427-304">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="f5427-305">応答</span><span class="sxs-lookup"><span data-stu-id="f5427-305">Response</span></span>
<span data-ttu-id="f5427-306">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androidforwork](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md)の各概要オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f5427-306">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5427-307">例</span><span class="sxs-lookup"><span data-stu-id="f5427-307">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5427-308">要求</span><span class="sxs-lookup"><span data-stu-id="f5427-308">Request</span></span>
<span data-ttu-id="f5427-309">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f5427-309">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2811

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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

### <a name="response"></a><span data-ttu-id="f5427-310">応答</span><span class="sxs-lookup"><span data-stu-id="f5427-310">Response</span></span>
<span data-ttu-id="f5427-p131">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f5427-p131">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2983

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
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





