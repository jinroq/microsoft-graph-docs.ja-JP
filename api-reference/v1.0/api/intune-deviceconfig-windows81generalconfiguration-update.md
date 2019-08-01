---
title: Update windows81GeneralConfiguration
description: windows81GeneralConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac5115ec2dae19fc111fb0dfea8a8092fbbb031c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019983"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="c9d13-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="c9d13-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="c9d13-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9d13-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9d13-105">[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-105">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9d13-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="c9d13-106">Prerequisites</span></span>
<span data-ttu-id="c9d13-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9d13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9d13-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9d13-109">Permission type</span></span>|<span data-ttu-id="c9d13-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9d13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9d13-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9d13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c9d13-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9d13-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c9d13-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9d13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9d13-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9d13-114">Not supported.</span></span>|
|<span data-ttu-id="c9d13-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9d13-115">Application</span></span>|<span data-ttu-id="c9d13-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9d13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9d13-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9d13-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c9d13-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9d13-118">Request headers</span></span>
|<span data-ttu-id="c9d13-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9d13-119">Header</span></span>|<span data-ttu-id="c9d13-120">値</span><span class="sxs-lookup"><span data-stu-id="c9d13-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9d13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9d13-121">Authorization</span></span>|<span data-ttu-id="c9d13-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9d13-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9d13-123">承諾</span><span class="sxs-lookup"><span data-stu-id="c9d13-123">Accept</span></span>|<span data-ttu-id="c9d13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c9d13-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9d13-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9d13-125">Request body</span></span>
<span data-ttu-id="c9d13-126">要求本文で、[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-126">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="c9d13-127">次の表に、[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-127">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="c9d13-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c9d13-128">Property</span></span>|<span data-ttu-id="c9d13-129">型</span><span class="sxs-lookup"><span data-stu-id="c9d13-129">Type</span></span>|<span data-ttu-id="c9d13-130">説明</span><span class="sxs-lookup"><span data-stu-id="c9d13-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9d13-131">id</span><span class="sxs-lookup"><span data-stu-id="c9d13-131">id</span></span>|<span data-ttu-id="c9d13-132">文字列</span><span class="sxs-lookup"><span data-stu-id="c9d13-132">String</span></span>|<span data-ttu-id="c9d13-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c9d13-133">Key of the entity.</span></span> <span data-ttu-id="c9d13-134">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9d13-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9d13-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c9d13-135">lastModifiedDateTime</span></span>|<span data-ttu-id="c9d13-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9d13-136">DateTimeOffset</span></span>|<span data-ttu-id="c9d13-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="c9d13-137">DateTime the object was last modified.</span></span> <span data-ttu-id="c9d13-138">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9d13-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9d13-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c9d13-139">createdDateTime</span></span>|<span data-ttu-id="c9d13-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9d13-140">DateTimeOffset</span></span>|<span data-ttu-id="c9d13-141">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="c9d13-141">DateTime the object was created.</span></span> <span data-ttu-id="c9d13-142">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9d13-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9d13-143">description</span><span class="sxs-lookup"><span data-stu-id="c9d13-143">description</span></span>|<span data-ttu-id="c9d13-144">String</span><span class="sxs-lookup"><span data-stu-id="c9d13-144">String</span></span>|<span data-ttu-id="c9d13-145">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="c9d13-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c9d13-146">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9d13-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9d13-147">displayName</span><span class="sxs-lookup"><span data-stu-id="c9d13-147">displayName</span></span>|<span data-ttu-id="c9d13-148">String</span><span class="sxs-lookup"><span data-stu-id="c9d13-148">String</span></span>|<span data-ttu-id="c9d13-149">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="c9d13-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c9d13-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9d13-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9d13-151">version</span><span class="sxs-lookup"><span data-stu-id="c9d13-151">version</span></span>|<span data-ttu-id="c9d13-152">Int32</span><span class="sxs-lookup"><span data-stu-id="c9d13-152">Int32</span></span>|<span data-ttu-id="c9d13-153">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="c9d13-153">Version of the device configuration.</span></span> <span data-ttu-id="c9d13-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c9d13-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c9d13-155">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="c9d13-155">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="c9d13-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-156">Boolean</span></span>|<span data-ttu-id="c9d13-157">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-157">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="c9d13-158">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="c9d13-158">applyOnlyToWindows81</span></span>|<span data-ttu-id="c9d13-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-159">Boolean</span></span>|<span data-ttu-id="c9d13-160">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="c9d13-160">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="c9d13-161">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c9d13-161">This property is read-only.</span></span>|
|<span data-ttu-id="c9d13-162">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="c9d13-162">browserBlockAutofill</span></span>|<span data-ttu-id="c9d13-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-163">Boolean</span></span>|<span data-ttu-id="c9d13-164">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-164">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="c9d13-165">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="c9d13-165">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="c9d13-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-166">Boolean</span></span>|<span data-ttu-id="c9d13-167">イントラネット サイトの自動検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-167">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="c9d13-168">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="c9d13-168">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="c9d13-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-169">Boolean</span></span>|<span data-ttu-id="c9d13-170">エンタープライズ モードのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-170">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="c9d13-171">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="c9d13-171">browserBlockJavaScript</span></span>|<span data-ttu-id="c9d13-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-172">Boolean</span></span>|<span data-ttu-id="c9d13-173">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-173">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="c9d13-174">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="c9d13-174">browserBlockPlugins</span></span>|<span data-ttu-id="c9d13-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-175">Boolean</span></span>|<span data-ttu-id="c9d13-176">プラグインを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-176">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="c9d13-177">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="c9d13-177">browserBlockPopups</span></span>|<span data-ttu-id="c9d13-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-178">Boolean</span></span>|<span data-ttu-id="c9d13-179">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-179">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="c9d13-180">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="c9d13-180">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="c9d13-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-181">Boolean</span></span>|<span data-ttu-id="c9d13-182">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-182">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="c9d13-183">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="c9d13-183">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="c9d13-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-184">Boolean</span></span>|<span data-ttu-id="c9d13-185">イントラネット サイトでの 1 単語のエントリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-185">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="c9d13-186">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="c9d13-186">browserRequireSmartScreen</span></span>|<span data-ttu-id="c9d13-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-187">Boolean</span></span>|<span data-ttu-id="c9d13-188">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-188">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="c9d13-189">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="c9d13-189">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="c9d13-190">String</span><span class="sxs-lookup"><span data-stu-id="c9d13-190">String</span></span>|<span data-ttu-id="c9d13-191">エンタープライズ モードのサイト リストの場所。</span><span class="sxs-lookup"><span data-stu-id="c9d13-191">The enterprise mode site list location.</span></span> <span data-ttu-id="c9d13-192">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-192">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="c9d13-193">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c9d13-193">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="c9d13-194">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c9d13-194">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="c9d13-195">インターネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="c9d13-195">The internet security level.</span></span> <span data-ttu-id="c9d13-196">可能な値は、`userDefined`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="c9d13-196">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="c9d13-197">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c9d13-197">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="c9d13-198">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c9d13-198">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="c9d13-199">イントラネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="c9d13-199">The Intranet security level.</span></span> <span data-ttu-id="c9d13-200">使用可能な値: `userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high`。</span><span class="sxs-lookup"><span data-stu-id="c9d13-200">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="c9d13-201">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="c9d13-201">browserLoggingReportLocation</span></span>|<span data-ttu-id="c9d13-202">String</span><span class="sxs-lookup"><span data-stu-id="c9d13-202">String</span></span>|<span data-ttu-id="c9d13-203">ログ レポートの場所。</span><span class="sxs-lookup"><span data-stu-id="c9d13-203">The logging report location.</span></span>|
|<span data-ttu-id="c9d13-204">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="c9d13-204">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="c9d13-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-205">Boolean</span></span>|<span data-ttu-id="c9d13-206">制限付きサイトに対する高度なセキュリティを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-206">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="c9d13-207">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="c9d13-207">browserRequireFirewall</span></span>|<span data-ttu-id="c9d13-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-208">Boolean</span></span>|<span data-ttu-id="c9d13-209">ファイアウォールが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-209">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="c9d13-210">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="c9d13-210">browserRequireFraudWarning</span></span>|<span data-ttu-id="c9d13-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-211">Boolean</span></span>|<span data-ttu-id="c9d13-212">不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-212">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="c9d13-213">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c9d13-213">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="c9d13-214">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="c9d13-214">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="c9d13-215">信頼済みサイトのセキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="c9d13-215">The trusted sites security level.</span></span> <span data-ttu-id="c9d13-216">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="c9d13-216">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="c9d13-217">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="c9d13-217">cellularBlockDataRoaming</span></span>|<span data-ttu-id="c9d13-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-218">Boolean</span></span>|<span data-ttu-id="c9d13-219">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-219">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="c9d13-220">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="c9d13-220">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="c9d13-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-221">Boolean</span></span>|<span data-ttu-id="c9d13-222">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-222">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="c9d13-223">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="c9d13-223">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="c9d13-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-224">Boolean</span></span>|<span data-ttu-id="c9d13-225">ユーザーがピクチャ パスワードおよび暗証番号 (PIN) を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-225">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="c9d13-226">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c9d13-226">passwordExpirationDays</span></span>|<span data-ttu-id="c9d13-227">Int32</span><span class="sxs-lookup"><span data-stu-id="c9d13-227">Int32</span></span>|<span data-ttu-id="c9d13-228">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="c9d13-228">Password expiration in days.</span></span>|
|<span data-ttu-id="c9d13-229">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c9d13-229">passwordMinimumLength</span></span>|<span data-ttu-id="c9d13-230">Int32</span><span class="sxs-lookup"><span data-stu-id="c9d13-230">Int32</span></span>|<span data-ttu-id="c9d13-231">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="c9d13-231">The minimum password length.</span></span>|
|<span data-ttu-id="c9d13-232">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c9d13-232">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c9d13-233">Int32</span><span class="sxs-lookup"><span data-stu-id="c9d13-233">Int32</span></span>|<span data-ttu-id="c9d13-234">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="c9d13-234">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c9d13-235">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="c9d13-235">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="c9d13-236">Int32</span><span class="sxs-lookup"><span data-stu-id="c9d13-236">Int32</span></span>|<span data-ttu-id="c9d13-237">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="c9d13-237">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="c9d13-238">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c9d13-238">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c9d13-239">Int32</span><span class="sxs-lookup"><span data-stu-id="c9d13-239">Int32</span></span>|<span data-ttu-id="c9d13-240">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="c9d13-240">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="c9d13-241">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="c9d13-241">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c9d13-242">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c9d13-242">passwordRequiredType</span></span>|[<span data-ttu-id="c9d13-243">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c9d13-243">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="c9d13-244">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="c9d13-244">The required password type.</span></span> <span data-ttu-id="c9d13-245">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="c9d13-245">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="c9d13-246">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c9d13-246">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c9d13-247">Int32</span><span class="sxs-lookup"><span data-stu-id="c9d13-247">Int32</span></span>|<span data-ttu-id="c9d13-248">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="c9d13-248">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="c9d13-249">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="c9d13-249">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="c9d13-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-250">Boolean</span></span>|<span data-ttu-id="c9d13-251">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-251">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="c9d13-252">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="c9d13-252">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="c9d13-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d13-253">Boolean</span></span>|<span data-ttu-id="c9d13-254">自動更新が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-254">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="c9d13-255">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="c9d13-255">userAccountControlSettings</span></span>|[<span data-ttu-id="c9d13-256">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="c9d13-256">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="c9d13-257">ユーザー アカウント制御の設定。</span><span class="sxs-lookup"><span data-stu-id="c9d13-257">The user account control settings.</span></span> <span data-ttu-id="c9d13-258">可能な値は、`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify` です。</span><span class="sxs-lookup"><span data-stu-id="c9d13-258">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="c9d13-259">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="c9d13-259">workFoldersUrl</span></span>|<span data-ttu-id="c9d13-260">String</span><span class="sxs-lookup"><span data-stu-id="c9d13-260">String</span></span>|<span data-ttu-id="c9d13-261">作業フォルダーの URL。</span><span class="sxs-lookup"><span data-stu-id="c9d13-261">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="c9d13-262">応答</span><span class="sxs-lookup"><span data-stu-id="c9d13-262">Response</span></span>
<span data-ttu-id="c9d13-263">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="c9d13-263">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9d13-264">例</span><span class="sxs-lookup"><span data-stu-id="c9d13-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9d13-265">要求</span><span class="sxs-lookup"><span data-stu-id="c9d13-265">Request</span></span>
<span data-ttu-id="c9d13-266">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c9d13-266">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1693

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="c9d13-267">応答</span><span class="sxs-lookup"><span data-stu-id="c9d13-267">Response</span></span>
<span data-ttu-id="c9d13-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c9d13-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1865

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "applyOnlyToWindows81": true,
  "browserBlockAutofill": true,
  "browserBlockAutomaticDetectionOfIntranetSites": true,
  "browserBlockEnterpriseModeAccess": true,
  "browserBlockJavaScript": true,
  "browserBlockPlugins": true,
  "browserBlockPopups": true,
  "browserBlockSendingDoNotTrackHeader": true,
  "browserBlockSingleWordEntryOnIntranetSites": true,
  "browserRequireSmartScreen": true,
  "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
  "browserInternetSecurityLevel": "medium",
  "browserIntranetSecurityLevel": "low",
  "browserLoggingReportLocation": "Browser Logging Report Location value",
  "browserRequireHighSecurityForRestrictedSites": true,
  "browserRequireFirewall": true,
  "browserRequireFraudWarning": true,
  "browserTrustedSitesSecurityLevel": "low",
  "cellularBlockDataRoaming": true,
  "diagnosticsBlockDataSubmission": true,
  "passwordBlockPicturePasswordAndPin": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "storageRequireDeviceEncryption": true,
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```



