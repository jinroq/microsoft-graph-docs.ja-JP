---
title: WindowsIdentityProtectionConfiguration を作成します。
description: 新しい windowsIdentityProtectionConfiguration オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be9c6ad30eb869bfd47b20863fc41e103eabe1c2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408993"
---
# <a name="create-windowsidentityprotectionconfiguration"></a><span data-ttu-id="9ead2-103">WindowsIdentityProtectionConfiguration を作成します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-103">Create windowsIdentityProtectionConfiguration</span></span>

> <span data-ttu-id="9ead2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ead2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ead2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ead2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ead2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ead2-107">新しい[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-107">Create a new [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ead2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9ead2-108">Prerequisites</span></span>
<span data-ttu-id="9ead2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ead2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9ead2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9ead2-111">Permission type</span></span>|<span data-ttu-id="9ead2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9ead2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ead2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9ead2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ead2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ead2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ead2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9ead2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ead2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ead2-116">Not supported.</span></span>|
|<span data-ttu-id="9ead2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9ead2-117">Application</span></span>|<span data-ttu-id="9ead2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ead2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ead2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9ead2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9ead2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ead2-120">Request headers</span></span>
|<span data-ttu-id="9ead2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9ead2-121">Header</span></span>|<span data-ttu-id="9ead2-122">値</span><span class="sxs-lookup"><span data-stu-id="9ead2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ead2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ead2-123">Authorization</span></span>|<span data-ttu-id="9ead2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9ead2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ead2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9ead2-125">Accept</span></span>|<span data-ttu-id="9ead2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ead2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ead2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9ead2-127">Request body</span></span>
<span data-ttu-id="9ead2-128">要求の本文に windowsIdentityProtectionConfiguration オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-128">In the request body, supply a JSON representation for the windowsIdentityProtectionConfiguration object.</span></span>

<span data-ttu-id="9ead2-129">次の表は、windowsIdentityProtectionConfiguration を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-129">The following table shows the properties that are required when you create the windowsIdentityProtectionConfiguration.</span></span>

|<span data-ttu-id="9ead2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9ead2-130">Property</span></span>|<span data-ttu-id="9ead2-131">型</span><span class="sxs-lookup"><span data-stu-id="9ead2-131">Type</span></span>|<span data-ttu-id="9ead2-132">説明</span><span class="sxs-lookup"><span data-stu-id="9ead2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ead2-133">id</span><span class="sxs-lookup"><span data-stu-id="9ead2-133">id</span></span>|<span data-ttu-id="9ead2-134">String</span><span class="sxs-lookup"><span data-stu-id="9ead2-134">String</span></span>|<span data-ttu-id="9ead2-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9ead2-135">Key of the entity.</span></span> <span data-ttu-id="9ead2-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ead2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9ead2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="9ead2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ead2-138">DateTimeOffset</span></span>|<span data-ttu-id="9ead2-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9ead2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="9ead2-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ead2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9ead2-141">roleScopeTagIds</span></span>|<span data-ttu-id="9ead2-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9ead2-142">String collection</span></span>|<span data-ttu-id="9ead2-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="9ead2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9ead2-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ead2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9ead2-145">supportsScopeTags</span></span>|<span data-ttu-id="9ead2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ead2-146">Boolean</span></span>|<span data-ttu-id="9ead2-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9ead2-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="9ead2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9ead2-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="9ead2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9ead2-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-150">This property is read-only.</span></span> <span data-ttu-id="9ead2-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ead2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9ead2-152">createdDateTime</span></span>|<span data-ttu-id="9ead2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9ead2-153">DateTimeOffset</span></span>|<span data-ttu-id="9ead2-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9ead2-154">DateTime the object was created.</span></span> <span data-ttu-id="9ead2-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ead2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead2-156">説明</span><span class="sxs-lookup"><span data-stu-id="9ead2-156">description</span></span>|<span data-ttu-id="9ead2-157">String</span><span class="sxs-lookup"><span data-stu-id="9ead2-157">String</span></span>|<span data-ttu-id="9ead2-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="9ead2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9ead2-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ead2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="9ead2-160">displayName</span></span>|<span data-ttu-id="9ead2-161">String</span><span class="sxs-lookup"><span data-stu-id="9ead2-161">String</span></span>|<span data-ttu-id="9ead2-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="9ead2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9ead2-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ead2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead2-164">version</span><span class="sxs-lookup"><span data-stu-id="9ead2-164">version</span></span>|<span data-ttu-id="9ead2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9ead2-165">Int32</span></span>|<span data-ttu-id="9ead2-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9ead2-166">Version of the device configuration.</span></span> <span data-ttu-id="9ead2-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9ead2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9ead2-168">useSecurityKeyForSignin</span><span class="sxs-lookup"><span data-stu-id="9ead2-168">useSecurityKeyForSignin</span></span>|<span data-ttu-id="9ead2-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ead2-169">Boolean</span></span>|<span data-ttu-id="9ead2-170">ログオン資格情報として Windows こんにちはセキュリティ キーを有効にするために使用するブール値です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-170">Boolean value used to enable the Windows Hello security key as a logon credential.</span></span>|
|<span data-ttu-id="9ead2-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span><span class="sxs-lookup"><span data-stu-id="9ead2-171">enhancedAntiSpoofingForFacialFeaturesEnabled</span></span>|<span data-ttu-id="9ead2-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ead2-172">Boolean</span></span>|<span data-ttu-id="9ead2-173">拡張スプーフィング対策 Windows こんにちは顔認証の facial の機能の認識を有効にするために使用するブール値です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-173">Boolean value used to enable enhanced anti-spoofing for facial feature recognition on Windows Hello face authentication.</span></span>|
|<span data-ttu-id="9ead2-174">pinMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9ead2-174">pinMinimumLength</span></span>|<span data-ttu-id="9ead2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="9ead2-175">Int32</span></span>|<span data-ttu-id="9ead2-176">ビジネスの暗証番号 (pin) は、Windows こんにちはに必要な文字の最小数を設定する整数値。</span><span class="sxs-lookup"><span data-stu-id="9ead2-176">Integer value that sets the minimum number of characters required for the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9ead2-177">有効な値は 4 ~ 127 包括的で、最大の暗証番号 (pin) の設定値に等しいかそれより小さい。</span><span class="sxs-lookup"><span data-stu-id="9ead2-177">Valid values are 4 to 127 inclusive and less than or equal to the value set for the maximum PIN.</span></span> <span data-ttu-id="9ead2-178">有効な値 4 ~ 127</span><span class="sxs-lookup"><span data-stu-id="9ead2-178">Valid values 4 to 127</span></span>|
|<span data-ttu-id="9ead2-179">pinMaximumLength</span><span class="sxs-lookup"><span data-stu-id="9ead2-179">pinMaximumLength</span></span>|<span data-ttu-id="9ead2-180">Int32</span><span class="sxs-lookup"><span data-stu-id="9ead2-180">Int32</span></span>|<span data-ttu-id="9ead2-181">暗証番号 (pin) の作業に使用できる文字の最大数を設定する整数値。</span><span class="sxs-lookup"><span data-stu-id="9ead2-181">Integer value that sets the maximum number of characters allowed for the work PIN.</span></span> <span data-ttu-id="9ead2-182">有効な値は、4 ~ 127 包括的以上の最小の暗証番号 (pin) の設定値と同じです。</span><span class="sxs-lookup"><span data-stu-id="9ead2-182">Valid values are 4 to 127 inclusive and greater than or equal to the value set for the minimum PIN.</span></span> <span data-ttu-id="9ead2-183">有効な値 4 ~ 127</span><span class="sxs-lookup"><span data-stu-id="9ead2-183">Valid values 4 to 127</span></span>|
|<span data-ttu-id="9ead2-184">pinUppercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9ead2-184">pinUppercaseCharactersUsage</span></span>|[<span data-ttu-id="9ead2-185">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9ead2-185">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9ead2-186">この値は、ビジネスの暗証番号 (pin) の Windows こんにちはの文字の大文字の使用を構成します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-186">This value configures the use of uppercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9ead2-187">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-187">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="9ead2-188">pinLowercaseCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9ead2-188">pinLowercaseCharactersUsage</span></span>|[<span data-ttu-id="9ead2-189">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9ead2-189">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9ead2-190">この値は、ビジネスの暗証番号 (pin) の Windows こんにちはで小文字の使用を構成します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-190">This value configures the use of lowercase characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9ead2-191">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-191">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="9ead2-192">pinSpecialCharactersUsage</span><span class="sxs-lookup"><span data-stu-id="9ead2-192">pinSpecialCharactersUsage</span></span>|[<span data-ttu-id="9ead2-193">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="9ead2-193">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="9ead2-194">ビジネスの暗証番号 (pin) を Windows こんにちはで特殊文字を使用する機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-194">Controls the ability to use special characters in the Windows Hello for Business PIN.</span></span> <span data-ttu-id="9ead2-195">可能な値は、`blocked`、`required`、`allowed` です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-195">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="9ead2-196">pinExpirationInDays</span><span class="sxs-lookup"><span data-stu-id="9ead2-196">pinExpirationInDays</span></span>|<span data-ttu-id="9ead2-197">Int32</span><span class="sxs-lookup"><span data-stu-id="9ead2-197">Int32</span></span>|<span data-ttu-id="9ead2-198">期間 (日数) を指定する整数値システムがそれを変更するユーザーを必要とする前に、暗証番号 (pin) を使用することができます。</span><span class="sxs-lookup"><span data-stu-id="9ead2-198">Integer value specifies the period (in days) that a PIN can be used before the system requires the user to change it.</span></span> <span data-ttu-id="9ead2-199">有効な値は、0 に 730 包括的です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-199">Valid values are 0 to 730 inclusive.</span></span> <span data-ttu-id="9ead2-200">有効な値は 0 から 730 までです</span><span class="sxs-lookup"><span data-stu-id="9ead2-200">Valid values 0 to 730</span></span>|
|<span data-ttu-id="9ead2-201">pinPreviousBlockCount</span><span class="sxs-lookup"><span data-stu-id="9ead2-201">pinPreviousBlockCount</span></span>|<span data-ttu-id="9ead2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="9ead2-202">Int32</span></span>|<span data-ttu-id="9ead2-203">過去のピンを使用できないようにする機能を制御します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-203">Controls the ability to prevent users from using past PINs.</span></span> <span data-ttu-id="9ead2-204">0 から 50、包括的で、これを設定する必要があり、その数にユーザーの現在の暗証番号 (pin) が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ead2-204">This must be set between 0 and 50, inclusive, and the current PIN of the user is included in that count.</span></span> <span data-ttu-id="9ead2-205">かどうかは 0 では、以前に設定ピンは格納されません。</span><span class="sxs-lookup"><span data-stu-id="9ead2-205">If set to 0, previous PINs are not stored.</span></span> <span data-ttu-id="9ead2-206">PIN を通じて暗証番号 (pin) の履歴は保持されませんをリセットします。</span><span class="sxs-lookup"><span data-stu-id="9ead2-206">PIN history is not preserved through a PIN reset.</span></span> <span data-ttu-id="9ead2-207">有効な値は 0 から 50 までです</span><span class="sxs-lookup"><span data-stu-id="9ead2-207">Valid values 0 to 50</span></span>|
|<span data-ttu-id="9ead2-208">pinRecoveryEnabled</span><span class="sxs-lookup"><span data-stu-id="9ead2-208">pinRecoveryEnabled</span></span>|<span data-ttu-id="9ead2-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ead2-209">Boolean</span></span>|<span data-ttu-id="9ead2-210">使用して、Windows こんにちはビジネス暗証番号 (pin) リカバリ ・ サービスの PIN を変更するユーザーを有効にするブール値です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-210">Boolean value that enables a user to change their PIN by using the Windows Hello for Business PIN recovery service.</span></span>|
|<span data-ttu-id="9ead2-211">securityDeviceRequired</span><span class="sxs-lookup"><span data-stu-id="9ead2-211">securityDeviceRequired</span></span>|<span data-ttu-id="9ead2-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ead2-212">Boolean</span></span>|<span data-ttu-id="9ead2-213">Windows こんにちはビジネスのための準備のトラステッド プラットフォーム モジュール (TPM) を必要とするかどうかを制御します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-213">Controls whether to require a Trusted Platform Module (TPM) for provisioning Windows Hello for Business.</span></span> <span data-ttu-id="9ead2-214">TPM は、他のデバイス上に格納されているデータは使用できませんという点で、その他セキュリティ上の利点を提供します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-214">A TPM provides an additional security benefit in that data stored on it cannot be used on other devices.</span></span> <span data-ttu-id="9ead2-215">かどうかは False に設定すると、すべてのデバイスをプロビジョニングできる Windows こんにちはビジネスに使用可能な TPM がない場合でも。</span><span class="sxs-lookup"><span data-stu-id="9ead2-215">If set to False, all devices can provision Windows Hello for Business even if there is not a usable TPM.</span></span>|
|<span data-ttu-id="9ead2-216">unlockWithBiometricsEnabled</span><span class="sxs-lookup"><span data-stu-id="9ead2-216">unlockWithBiometricsEnabled</span></span>|<span data-ttu-id="9ead2-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ead2-217">Boolean</span></span>|<span data-ttu-id="9ead2-218">代わりに、Windows こんにちはビジネス暗証番号 (pin) の顔や指紋などの生体認証のジェスチャの使用を制御します。</span><span class="sxs-lookup"><span data-stu-id="9ead2-218">Controls the use of biometric gestures, such as face and fingerprint, as an alternative to the Windows Hello for Business PIN.</span></span>  <span data-ttu-id="9ead2-219">場合は False、生体認証のジェスチャに設定することはできません。</span><span class="sxs-lookup"><span data-stu-id="9ead2-219">If set to False, biometric gestures are not allowed.</span></span> <span data-ttu-id="9ead2-220">ユーザーは、障害が発生した場合のバックアップとして、暗証番号 (pin) を構成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ead2-220">Users must still configure a PIN as a backup in case of failures.</span></span>|
|<span data-ttu-id="9ead2-221">useCertificatesForOnPremisesAuthEnabled</span><span class="sxs-lookup"><span data-stu-id="9ead2-221">useCertificatesForOnPremisesAuthEnabled</span></span>|<span data-ttu-id="9ead2-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ead2-222">Boolean</span></span>|<span data-ttu-id="9ead2-223">Windows こんにちは設置型リソースの認証に証明書を使用するビジネスを可能にするブール値です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-223">Boolean value that enables Windows Hello for Business to use certificates to authenticate on-premise resources.</span></span>|
|<span data-ttu-id="9ead2-224">windowsHelloForBusinessBlocked</span><span class="sxs-lookup"><span data-stu-id="9ead2-224">windowsHelloForBusinessBlocked</span></span>|<span data-ttu-id="9ead2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="9ead2-225">Boolean</span></span>|<span data-ttu-id="9ead2-226">Windows こんにちはの Windows へのサインイン方法としてビジネスをブロックするブール値です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-226">Boolean value that blocks Windows Hello for Business as a method for signing into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="9ead2-227">応答</span><span class="sxs-lookup"><span data-stu-id="9ead2-227">Response</span></span>
<span data-ttu-id="9ead2-228">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="9ead2-228">If successful, this method returns a `201 Created` response code and a [windowsIdentityProtectionConfiguration](../resources/intune-deviceconfig-windowsidentityprotectionconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ead2-229">例</span><span class="sxs-lookup"><span data-stu-id="9ead2-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ead2-230">要求</span><span class="sxs-lookup"><span data-stu-id="9ead2-230">Request</span></span>
<span data-ttu-id="9ead2-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9ead2-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="9ead2-232">応答</span><span class="sxs-lookup"><span data-stu-id="9ead2-232">Response</span></span>
<span data-ttu-id="9ead2-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9ead2-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




