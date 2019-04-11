---
title: windowsIdentityProtectionConfiguration を作成する
description: 新しい windowsIdentityProtectionConfiguration オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7d1ef9c923cf894531951fbaea2c4cc98b4258d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31798965"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="76e57-103">windowsIdentityProtectionConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="76e57-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="76e57-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76e57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76e57-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76e57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76e57-106">新しい[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="76e57-106">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76e57-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="76e57-107">Prerequisites</span></span>
<span data-ttu-id="76e57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76e57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76e57-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76e57-110">Permission type</span></span>|<span data-ttu-id="76e57-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="76e57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76e57-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76e57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76e57-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76e57-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76e57-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76e57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76e57-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76e57-115">Not supported.</span></span>|
|<span data-ttu-id="76e57-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76e57-116">Application</span></span>|<span data-ttu-id="76e57-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76e57-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76e57-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76e57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="76e57-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76e57-119">Request headers</span></span>
|<span data-ttu-id="76e57-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76e57-120">Header</span></span>|<span data-ttu-id="76e57-121">値</span><span class="sxs-lookup"><span data-stu-id="76e57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76e57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76e57-122">Authorization</span></span>|<span data-ttu-id="76e57-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="76e57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76e57-124">承諾</span><span class="sxs-lookup"><span data-stu-id="76e57-124">Accept</span></span>|<span data-ttu-id="76e57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76e57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76e57-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="76e57-126">Request body</span></span>
<span data-ttu-id="76e57-127">要求本文で、windowsIdentityProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="76e57-127">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="76e57-128">次の表に、windowsIdentityProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="76e57-128">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="76e57-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76e57-129">Property</span></span>|<span data-ttu-id="76e57-130">型</span><span class="sxs-lookup"><span data-stu-id="76e57-130">Type</span></span>|<span data-ttu-id="76e57-131">説明</span><span class="sxs-lookup"><span data-stu-id="76e57-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76e57-132">id</span><span class="sxs-lookup"><span data-stu-id="76e57-132">id</span></span>|<span data-ttu-id="76e57-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="76e57-133">String</span></span>|<span data-ttu-id="76e57-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="76e57-134">Key of the entity.</span></span> <span data-ttu-id="76e57-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="76e57-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76e57-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76e57-136">lastModifiedDateTime</span></span>|<span data-ttu-id="76e57-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76e57-137">DateTimeOffset</span></span>|<span data-ttu-id="76e57-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="76e57-138">DateTime the object was last modified.</span></span> <span data-ttu-id="76e57-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="76e57-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76e57-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="76e57-140">roleScopeTagIds</span></span>|<span data-ttu-id="76e57-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="76e57-141">String collection</span></span>|<span data-ttu-id="76e57-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="76e57-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="76e57-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="76e57-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76e57-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="76e57-144">supportsScopeTags</span></span>|<span data-ttu-id="76e57-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="76e57-145">Boolean</span></span>|<span data-ttu-id="76e57-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="76e57-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="76e57-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="76e57-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="76e57-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="76e57-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="76e57-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="76e57-149">This property is read-only.</span></span> <span data-ttu-id="76e57-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="76e57-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76e57-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76e57-151">createdDateTime</span></span>|<span data-ttu-id="76e57-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76e57-152">DateTimeOffset</span></span>|<span data-ttu-id="76e57-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="76e57-153">DateTime the object was created.</span></span> <span data-ttu-id="76e57-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="76e57-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76e57-155">説明</span><span class="sxs-lookup"><span data-stu-id="76e57-155">description</span></span>|<span data-ttu-id="76e57-156">String</span><span class="sxs-lookup"><span data-stu-id="76e57-156">String</span></span>|<span data-ttu-id="76e57-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="76e57-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76e57-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="76e57-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76e57-159">displayName</span><span class="sxs-lookup"><span data-stu-id="76e57-159">displayName</span></span>|<span data-ttu-id="76e57-160">String</span><span class="sxs-lookup"><span data-stu-id="76e57-160">String</span></span>|<span data-ttu-id="76e57-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="76e57-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76e57-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="76e57-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76e57-163">version</span><span class="sxs-lookup"><span data-stu-id="76e57-163">version</span></span>|<span data-ttu-id="76e57-164">Int32</span><span class="sxs-lookup"><span data-stu-id="76e57-164">Int32</span></span>|<span data-ttu-id="76e57-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="76e57-165">Version of the device configuration.</span></span> <span data-ttu-id="76e57-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="76e57-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76e57-167">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="76e57-167">useSecurityKeyForSignin</span></span>|<span data-ttu-id="76e57-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="76e57-168">Boolean</span></span>|<span data-ttu-id="76e57-169">ログオン資格情報として Windows Hello セキュリティキーを有効にするために使用されるブール値。</span><span class="sxs-lookup"><span data-stu-id="76e57-169">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="76e57-170">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="76e57-170">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="76e57-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="76e57-171">Boolean</span></span>|<span data-ttu-id="76e57-172">Windows Hello 顔認証で顔機能認識の強化されたスプーフィング対策を有効にするために使用するブール値。</span><span class="sxs-lookup"><span data-stu-id="76e57-172">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="76e57-173">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="76e57-173">pinMinimumLength</span></span>|<span data-ttu-id="76e57-174">Int32</span><span class="sxs-lookup"><span data-stu-id="76e57-174">Int32</span></span>|<span data-ttu-id="76e57-175">Windows Hello for business の PIN に必要な最小文字数を設定する整数値。</span><span class="sxs-lookup"><span data-stu-id="76e57-175">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="76e57-176">有効な値は、4 ~ 127 の範囲で、最大 PIN の値を設定します。</span><span class="sxs-lookup"><span data-stu-id="76e57-176">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="76e57-177">有効な値は 4 ~ 127</span><span class="sxs-lookup"><span data-stu-id="76e57-177">Valid values 4 to 127</span></span>|
|<span data-ttu-id="76e57-178">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="76e57-178">pinMaximumLength</span></span>|<span data-ttu-id="76e57-179">Int32</span><span class="sxs-lookup"><span data-stu-id="76e57-179">Int32</span></span>|<span data-ttu-id="76e57-180">作業 PIN に使用できる最大文字数を設定する整数値。</span><span class="sxs-lookup"><span data-stu-id="76e57-180">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="76e57-181">有効な値は、最小 PIN で設定された値以上の4から127の範囲です。</span><span class="sxs-lookup"><span data-stu-id="76e57-181">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="76e57-182">有効な値は 4 ~ 127</span><span class="sxs-lookup"><span data-stu-id="76e57-182">Valid values 4 to 127</span></span>|
|<span data-ttu-id="76e57-183">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="76e57-183">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="76e57-184">configurationusage</span><span class="sxs-lookup"><span data-stu-id="76e57-184">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="76e57-185">この値は、Windows Hello for Business の PIN での大文字の使用を構成します。</span><span class="sxs-lookup"><span data-stu-id="76e57-185">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="76e57-186">使用可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="76e57-186">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="76e57-187">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="76e57-187">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="76e57-188">configurationusage</span><span class="sxs-lookup"><span data-stu-id="76e57-188">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="76e57-189">この値は、Windows Hello for Business の PIN に小文字を使用するように構成します。</span><span class="sxs-lookup"><span data-stu-id="76e57-189">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="76e57-190">使用可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="76e57-190">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="76e57-191">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="76e57-191">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="76e57-192">configurationusage</span><span class="sxs-lookup"><span data-stu-id="76e57-192">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="76e57-193">Windows Hello for Business の PIN で特殊文字を使用する機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="76e57-193">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="76e57-194">使用可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="76e57-194">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="76e57-195">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="76e57-195">pinExpirationInDays</span></span>|<span data-ttu-id="76e57-196">Int32</span><span class="sxs-lookup"><span data-stu-id="76e57-196">Int32</span></span>|<span data-ttu-id="76e57-197">[整数値] PIN の変更をユーザーに要求する前に PIN を使用できる期間 (日数) を指定します。</span><span class="sxs-lookup"><span data-stu-id="76e57-197">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="76e57-198">有効な値は0から730の範囲です。</span><span class="sxs-lookup"><span data-stu-id="76e57-198">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="76e57-199">有効な値は 0 から 730 までです</span><span class="sxs-lookup"><span data-stu-id="76e57-199">Valid values 0 to 730</span></span>|
|<span data-ttu-id="76e57-200">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="76e57-200">pinPreviousBlockCount</span></span>|<span data-ttu-id="76e57-201">Int32</span><span class="sxs-lookup"><span data-stu-id="76e57-201">Int32</span></span>|<span data-ttu-id="76e57-202">ユーザーが過去の pin を使用できないようにする機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="76e57-202">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="76e57-203">0 ~ 50 の範囲で設定する必要があり、ユーザーの現在の PIN がその数に含まれています。</span><span class="sxs-lookup"><span data-stu-id="76e57-203">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="76e57-204">0に設定すると、以前の pin は保存されません。</span><span class="sxs-lookup"><span data-stu-id="76e57-204">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="76e57-205">pin をリセットすると、pin 履歴は保持されません。</span><span class="sxs-lookup"><span data-stu-id="76e57-205">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="76e57-206">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="76e57-206">Valid values 0 to 50</span></span>|
|<span data-ttu-id="76e57-207">pinrecoveryenabled</span><span class="sxs-lookup"><span data-stu-id="76e57-207">pinRecoveryEnabled</span></span>|<span data-ttu-id="76e57-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="76e57-208">Boolean</span></span>|<span data-ttu-id="76e57-209">ユーザーが Windows Hello for business pin 回復サービスを使用して pin を変更できるようにするブール値。</span><span class="sxs-lookup"><span data-stu-id="76e57-209">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="76e57-210">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="76e57-210">securityDeviceRequired</span></span>|<span data-ttu-id="76e57-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="76e57-211">Boolean</span></span>|<span data-ttu-id="76e57-212">Windows Hello for business のプロビジョニングにトラステッドプラットフォームモジュール (TPM) を必要とするかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="76e57-212">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="76e57-213">TPM に格納されたデータは、他のデバイスでは使用できないため、追加のセキュリティ上の利点があります。</span><span class="sxs-lookup"><span data-stu-id="76e57-213">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="76e57-214">False に設定されている場合は、使用可能な TPM がない場合でも、すべてのデバイスが Windows Hello for business をプロビジョニングできます。</span><span class="sxs-lookup"><span data-stu-id="76e57-214">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="76e57-215">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="76e57-215">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="76e57-216">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="76e57-216">Boolean</span></span>|<span data-ttu-id="76e57-217">Windows Hello for Business PIN の代わりに、顔文字や指紋などのバイオメトリクスジェスチャの使用を制御します。</span><span class="sxs-lookup"><span data-stu-id="76e57-217">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="76e57-218">False に設定すると、生体認証ジェスチャは許可されません。</span><span class="sxs-lookup"><span data-stu-id="76e57-218">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="76e57-219">ユーザーは、障害が発生した場合に、バックアップとして PIN を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="76e57-219">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="76e57-220">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="76e57-220">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="76e57-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="76e57-221">Boolean</span></span>|<span data-ttu-id="76e57-222">Windows Hello for business が証明書を使用してオンプレミスのリソースを認証できるようにするブール値。</span><span class="sxs-lookup"><span data-stu-id="76e57-222">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="76e57-223">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="76e57-223">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="76e57-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="76e57-224">Boolean</span></span>|<span data-ttu-id="76e57-225">windows Hello for business を windows にサインインするための方法としてブロックするブール値。</span><span class="sxs-lookup"><span data-stu-id="76e57-225">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="76e57-226">応答</span><span class="sxs-lookup"><span data-stu-id="76e57-226">Response</span></span>
<span data-ttu-id="76e57-227">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="76e57-227">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76e57-228">例</span><span class="sxs-lookup"><span data-stu-id="76e57-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="76e57-229">要求</span><span class="sxs-lookup"><span data-stu-id="76e57-229">Request</span></span>
<span data-ttu-id="76e57-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76e57-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 810

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="76e57-231">応答</span><span class="sxs-lookup"><span data-stu-id="76e57-231">Response</span></span>
<span data-ttu-id="76e57-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="76e57-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 982

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "useSecurityKeyForSignin": true,
  "enhancedAntiSpoofingForFacialFeaturesEnabled": true,
  "pinMinimumLength": 0,
  "pinMaximumLength": 0,
  "pinUppercaseCharactersUsage": "required",
  "pinLowercaseCharactersUsage": "required",
  "pinSpecialCharactersUsage": "required",
  "pinExpirationInDays": 3,
  "pinPreviousBlockCount": 5,
  "pinRecoveryEnabled": true,
  "securityDeviceRequired": true,
  "unlockWithBiometricsEnabled": true,
  "useCertificatesForOnPremisesAuthEnabled": true,
  "windowsHelloForBusinessBlocked": true
}
```





