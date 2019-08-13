---
title: WindowsIdentityProtectionConfiguration を作成する
description: 新しい windowsIdentityProtectionConfiguration オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d0be8bc0b5447a12ed962cd69eed3a2e59d8ea9e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36344414"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="66849-103">WindowsIdentityProtectionConfiguration を作成する</span><span class="sxs-lookup"><span data-stu-id="66849-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="66849-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66849-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66849-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="66849-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66849-106">新しい[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="66849-106">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66849-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="66849-107">Prerequisites</span></span>
<span data-ttu-id="66849-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66849-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66849-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66849-110">Permission type</span></span>|<span data-ttu-id="66849-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="66849-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66849-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66849-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66849-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66849-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="66849-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66849-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66849-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66849-115">Not supported.</span></span>|
|<span data-ttu-id="66849-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66849-116">Application</span></span>|<span data-ttu-id="66849-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66849-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="66849-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66849-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="66849-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66849-119">Request headers</span></span>
|<span data-ttu-id="66849-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66849-120">Header</span></span>|<span data-ttu-id="66849-121">値</span><span class="sxs-lookup"><span data-stu-id="66849-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66849-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66849-122">Authorization</span></span>|<span data-ttu-id="66849-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="66849-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66849-124">承諾</span><span class="sxs-lookup"><span data-stu-id="66849-124">Accept</span></span>|<span data-ttu-id="66849-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66849-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66849-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="66849-126">Request body</span></span>
<span data-ttu-id="66849-127">要求本文で、windowsIdentityProtectionConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="66849-127">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="66849-128">次の表に、windowsIdentityProtectionConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="66849-128">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="66849-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66849-129">Property</span></span>|<span data-ttu-id="66849-130">型</span><span class="sxs-lookup"><span data-stu-id="66849-130">Type</span></span>|<span data-ttu-id="66849-131">説明</span><span class="sxs-lookup"><span data-stu-id="66849-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66849-132">id</span><span class="sxs-lookup"><span data-stu-id="66849-132">id</span></span>|<span data-ttu-id="66849-133">文字列</span><span class="sxs-lookup"><span data-stu-id="66849-133">String</span></span>|<span data-ttu-id="66849-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="66849-134">Key of the entity.</span></span> <span data-ttu-id="66849-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="66849-136">lastModifiedDateTime</span></span>|<span data-ttu-id="66849-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66849-137">DateTimeOffset</span></span>|<span data-ttu-id="66849-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="66849-138">DateTime the object was last modified.</span></span> <span data-ttu-id="66849-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="66849-140">roleScopeTagIds</span></span>|<span data-ttu-id="66849-141">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="66849-141">String collection</span></span>|<span data-ttu-id="66849-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="66849-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="66849-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="66849-144">supportsScopeTags</span></span>|<span data-ttu-id="66849-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="66849-145">Boolean</span></span>|<span data-ttu-id="66849-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="66849-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="66849-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="66849-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="66849-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="66849-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="66849-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="66849-149">This property is read-only.</span></span> <span data-ttu-id="66849-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="66849-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="66849-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="66849-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="66849-153">このポリシーの OS エディションの適用。</span><span class="sxs-lookup"><span data-stu-id="66849-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="66849-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="66849-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="66849-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="66849-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="66849-157">このポリシーの OS バージョン適用ルール。</span><span class="sxs-lookup"><span data-stu-id="66849-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="66849-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-159">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="66849-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="66849-160">Devicemanagementの信頼性ルール Devicemode</span><span class="sxs-lookup"><span data-stu-id="66849-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="66849-161">このポリシーのデバイスモード適用ルール。</span><span class="sxs-lookup"><span data-stu-id="66849-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="66849-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66849-163">createdDateTime</span></span>|<span data-ttu-id="66849-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66849-164">DateTimeOffset</span></span>|<span data-ttu-id="66849-165">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="66849-165">DateTime the object was created.</span></span> <span data-ttu-id="66849-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-167">description</span><span class="sxs-lookup"><span data-stu-id="66849-167">description</span></span>|<span data-ttu-id="66849-168">String</span><span class="sxs-lookup"><span data-stu-id="66849-168">String</span></span>|<span data-ttu-id="66849-169">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="66849-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="66849-170">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-171">displayName</span><span class="sxs-lookup"><span data-stu-id="66849-171">displayName</span></span>|<span data-ttu-id="66849-172">String</span><span class="sxs-lookup"><span data-stu-id="66849-172">String</span></span>|<span data-ttu-id="66849-173">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="66849-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="66849-174">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-175">version</span><span class="sxs-lookup"><span data-stu-id="66849-175">version</span></span>|<span data-ttu-id="66849-176">Int32</span><span class="sxs-lookup"><span data-stu-id="66849-176">Int32</span></span>|<span data-ttu-id="66849-177">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="66849-177">Version of the device configuration.</span></span> <span data-ttu-id="66849-178">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="66849-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="66849-179">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="66849-179">useSecurityKeyForSignin</span></span>|<span data-ttu-id="66849-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="66849-180">Boolean</span></span>|<span data-ttu-id="66849-181">ログオン資格情報として Windows Hello セキュリティキーを有効にするために使用されるブール値。</span><span class="sxs-lookup"><span data-stu-id="66849-181">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="66849-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="66849-182">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="66849-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="66849-183">Boolean</span></span>|<span data-ttu-id="66849-184">Windows Hello 顔認証で顔機能認識の強化されたスプーフィング対策を有効にするために使用するブール値。</span><span class="sxs-lookup"><span data-stu-id="66849-184">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="66849-185">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="66849-185">pinMinimumLength</span></span>|<span data-ttu-id="66849-186">Int32</span><span class="sxs-lookup"><span data-stu-id="66849-186">Int32</span></span>|<span data-ttu-id="66849-187">Windows Hello for Business の PIN に必要な最小文字数を設定する整数値。</span><span class="sxs-lookup"><span data-stu-id="66849-187">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="66849-188">有効な値は、4 ~ 127 の範囲で、最大 PIN の値を設定します。</span><span class="sxs-lookup"><span data-stu-id="66849-188">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="66849-189">有効な値は 4 ~ 127</span><span class="sxs-lookup"><span data-stu-id="66849-189">Valid values 4 to 127</span></span>|
|<span data-ttu-id="66849-190">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="66849-190">pinMaximumLength</span></span>|<span data-ttu-id="66849-191">Int32</span><span class="sxs-lookup"><span data-stu-id="66849-191">Int32</span></span>|<span data-ttu-id="66849-192">作業 PIN に使用できる最大文字数を設定する整数値。</span><span class="sxs-lookup"><span data-stu-id="66849-192">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="66849-193">有効な値は、最小 PIN で設定された値以上の4から127の範囲です。</span><span class="sxs-lookup"><span data-stu-id="66849-193">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="66849-194">有効な値は 4 ~ 127</span><span class="sxs-lookup"><span data-stu-id="66849-194">Valid values 4 to 127</span></span>|
|<span data-ttu-id="66849-195">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="66849-195">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="66849-196">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="66849-196">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="66849-197">この値は、Windows Hello for Business の PIN での大文字の使用を構成します。</span><span class="sxs-lookup"><span data-stu-id="66849-197">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="66849-198">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="66849-198">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="66849-199">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="66849-199">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="66849-200">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="66849-200">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="66849-201">この値は、Windows Hello for Business の PIN に小文字を使用するように構成します。</span><span class="sxs-lookup"><span data-stu-id="66849-201">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="66849-202">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="66849-202">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="66849-203">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="66849-203">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="66849-204">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="66849-204">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="66849-205">Windows Hello for Business の PIN で特殊文字を使用する機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="66849-205">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="66849-206">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="66849-206">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="66849-207">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="66849-207">pinExpirationInDays</span></span>|<span data-ttu-id="66849-208">Int32</span><span class="sxs-lookup"><span data-stu-id="66849-208">Int32</span></span>|<span data-ttu-id="66849-209">[整数値] PIN の変更をユーザーに要求する前に PIN を使用できる期間 (日数) を指定します。</span><span class="sxs-lookup"><span data-stu-id="66849-209">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="66849-210">有効な値は0から730の範囲です。</span><span class="sxs-lookup"><span data-stu-id="66849-210">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="66849-211">有効な値は 0 から 730 までです</span><span class="sxs-lookup"><span data-stu-id="66849-211">Valid values 0 to 730</span></span>|
|<span data-ttu-id="66849-212">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="66849-212">pinPreviousBlockCount</span></span>|<span data-ttu-id="66849-213">Int32</span><span class="sxs-lookup"><span data-stu-id="66849-213">Int32</span></span>|<span data-ttu-id="66849-214">ユーザーが過去の Pin を使用できないようにする機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="66849-214">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="66849-215">0 ~ 50 の範囲で設定する必要があり、ユーザーの現在の PIN がその数に含まれています。</span><span class="sxs-lookup"><span data-stu-id="66849-215">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="66849-216">0に設定すると、以前の Pin は保存されません。</span><span class="sxs-lookup"><span data-stu-id="66849-216">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="66849-217">Pin をリセットすると、PIN 履歴は保持されません。</span><span class="sxs-lookup"><span data-stu-id="66849-217">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="66849-218">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="66849-218">Valid values 0 to 50</span></span>|
|<span data-ttu-id="66849-219">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="66849-219">pinRecoveryEnabled</span></span>|<span data-ttu-id="66849-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="66849-220">Boolean</span></span>|<span data-ttu-id="66849-221">ユーザーが Windows Hello for Business PIN 回復サービスを使用して PIN を変更できるようにするブール値。</span><span class="sxs-lookup"><span data-stu-id="66849-221">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="66849-222">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="66849-222">securityDeviceRequired</span></span>|<span data-ttu-id="66849-223">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="66849-223">Boolean</span></span>|<span data-ttu-id="66849-224">Windows Hello for Business のプロビジョニングにトラステッドプラットフォームモジュール (TPM) を必要とするかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="66849-224">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="66849-225">TPM に格納されたデータは、他のデバイスでは使用できないため、追加のセキュリティ上の利点があります。</span><span class="sxs-lookup"><span data-stu-id="66849-225">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="66849-226">False に設定されている場合は、使用可能な TPM がない場合でも、すべてのデバイスが Windows Hello for Business をプロビジョニングできます。</span><span class="sxs-lookup"><span data-stu-id="66849-226">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="66849-227">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="66849-227">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="66849-228">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="66849-228">Boolean</span></span>|<span data-ttu-id="66849-229">Windows Hello for Business PIN の代わりに、顔文字や指紋などのバイオメトリクスジェスチャの使用を制御します。</span><span class="sxs-lookup"><span data-stu-id="66849-229">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="66849-230">False に設定すると、生体認証ジェスチャは許可されません。</span><span class="sxs-lookup"><span data-stu-id="66849-230">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="66849-231">ユーザーは、障害が発生した場合に、バックアップとして PIN を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="66849-231">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="66849-232">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="66849-232">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="66849-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="66849-233">Boolean</span></span>|<span data-ttu-id="66849-234">Windows Hello for Business が証明書を使用してオンプレミスのリソースを認証できるようにするブール値。</span><span class="sxs-lookup"><span data-stu-id="66849-234">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="66849-235">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="66849-235">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="66849-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="66849-236">Boolean</span></span>|<span data-ttu-id="66849-237">Windows Hello for Business を Windows にサインインするための方法としてブロックするブール値。</span><span class="sxs-lookup"><span data-stu-id="66849-237">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="66849-238">応答</span><span class="sxs-lookup"><span data-stu-id="66849-238">Response</span></span>
<span data-ttu-id="66849-239">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66849-239">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66849-240">例</span><span class="sxs-lookup"><span data-stu-id="66849-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="66849-241">要求</span><span class="sxs-lookup"><span data-stu-id="66849-241">Request</span></span>
<span data-ttu-id="66849-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="66849-242">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1583

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
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

### <a name="response"></a><span data-ttu-id="66849-243">応答</span><span class="sxs-lookup"><span data-stu-id="66849-243">Response</span></span>
<span data-ttu-id="66849-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="66849-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1755

{
  "@odata.type": "#microsoft.graph.windowsIdentityProtectionConfiguration",
  "id": "b2e64303-4303-b2e6-0343-e6b20343e6b2",
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






