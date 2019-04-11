---
title: Update windows81GeneralConfiguration
description: windows81GeneralConfiguration オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7ae714c6fc270866da8dc1e153db5765d810e9f7
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31786680"
---
# <a name="update-windows81generalconfiguration"></a><span data-ttu-id="9c3aa-103">Update windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="9c3aa-103">Update windows81GeneralConfiguration</span></span>

> <span data-ttu-id="9c3aa-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c3aa-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c3aa-106">[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-106">Update the properties of a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c3aa-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="9c3aa-107">Prerequisites</span></span>
<span data-ttu-id="9c3aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c3aa-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9c3aa-110">Permission type</span></span>|<span data-ttu-id="9c3aa-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9c3aa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c3aa-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9c3aa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c3aa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c3aa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c3aa-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9c3aa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c3aa-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-115">Not supported.</span></span>|
|<span data-ttu-id="9c3aa-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9c3aa-116">Application</span></span>|<span data-ttu-id="9c3aa-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c3aa-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9c3aa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9c3aa-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c3aa-119">Request headers</span></span>
|<span data-ttu-id="9c3aa-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9c3aa-120">Header</span></span>|<span data-ttu-id="9c3aa-121">値</span><span class="sxs-lookup"><span data-stu-id="9c3aa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c3aa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9c3aa-122">Authorization</span></span>|<span data-ttu-id="9c3aa-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c3aa-124">承諾</span><span class="sxs-lookup"><span data-stu-id="9c3aa-124">Accept</span></span>|<span data-ttu-id="9c3aa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c3aa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c3aa-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="9c3aa-126">Request body</span></span>
<span data-ttu-id="9c3aa-127">要求本文で、[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-127">In the request body, supply a JSON representation for the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>

<span data-ttu-id="9c3aa-128">次の表に、[windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-128">The following table shows the properties that are required when you create the [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

|<span data-ttu-id="9c3aa-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9c3aa-129">Property</span></span>|<span data-ttu-id="9c3aa-130">型</span><span class="sxs-lookup"><span data-stu-id="9c3aa-130">Type</span></span>|<span data-ttu-id="9c3aa-131">説明</span><span class="sxs-lookup"><span data-stu-id="9c3aa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c3aa-132">id</span><span class="sxs-lookup"><span data-stu-id="9c3aa-132">id</span></span>|<span data-ttu-id="9c3aa-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9c3aa-133">String</span></span>|<span data-ttu-id="9c3aa-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-134">Key of the entity.</span></span> <span data-ttu-id="9c3aa-135">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9c3aa-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c3aa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9c3aa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9c3aa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c3aa-137">DateTimeOffset</span></span>|<span data-ttu-id="9c3aa-138">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9c3aa-139">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9c3aa-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c3aa-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9c3aa-140">roleScopeTagIds</span></span>|<span data-ttu-id="9c3aa-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9c3aa-141">String collection</span></span>|<span data-ttu-id="9c3aa-142">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9c3aa-143">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9c3aa-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c3aa-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9c3aa-144">supportsScopeTags</span></span>|<span data-ttu-id="9c3aa-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-145">Boolean</span></span>|<span data-ttu-id="9c3aa-146">基になるデバイス構成がスコープタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9c3aa-147">この値が false である場合、ScopeTags プロパティへの割り当ては許可されません。エンティティは、スコープを持つユーザーには表示されません。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9c3aa-148">これは Silverlight で作成された従来のポリシーに対して実行され、Azure ポータルでポリシーを削除して再作成することによって解決できます。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9c3aa-149">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-149">This property is read-only.</span></span> <span data-ttu-id="9c3aa-150">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9c3aa-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c3aa-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9c3aa-151">createdDateTime</span></span>|<span data-ttu-id="9c3aa-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9c3aa-152">DateTimeOffset</span></span>|<span data-ttu-id="9c3aa-153">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-153">DateTime the object was created.</span></span> <span data-ttu-id="9c3aa-154">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9c3aa-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c3aa-155">説明</span><span class="sxs-lookup"><span data-stu-id="9c3aa-155">description</span></span>|<span data-ttu-id="9c3aa-156">String</span><span class="sxs-lookup"><span data-stu-id="9c3aa-156">String</span></span>|<span data-ttu-id="9c3aa-157">管理者が指定した、デバイス構成についての説明。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9c3aa-158">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9c3aa-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c3aa-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9c3aa-159">displayName</span></span>|<span data-ttu-id="9c3aa-160">String</span><span class="sxs-lookup"><span data-stu-id="9c3aa-160">String</span></span>|<span data-ttu-id="9c3aa-161">管理者が指定した、デバイス構成の名前。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9c3aa-162">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9c3aa-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c3aa-163">version</span><span class="sxs-lookup"><span data-stu-id="9c3aa-163">version</span></span>|<span data-ttu-id="9c3aa-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3aa-164">Int32</span></span>|<span data-ttu-id="9c3aa-165">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-165">Version of the device configuration.</span></span> <span data-ttu-id="9c3aa-166">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="9c3aa-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9c3aa-167">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="9c3aa-167">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="9c3aa-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-168">Boolean</span></span>|<span data-ttu-id="9c3aa-169">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-169">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="9c3aa-170">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="9c3aa-170">applyOnlyToWindows81</span></span>|<span data-ttu-id="9c3aa-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-171">Boolean</span></span>|<span data-ttu-id="9c3aa-172">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-172">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="9c3aa-173">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-173">This property is read-only.</span></span>|
|<span data-ttu-id="9c3aa-174">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="9c3aa-174">browserBlockAutofill</span></span>|<span data-ttu-id="9c3aa-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-175">Boolean</span></span>|<span data-ttu-id="9c3aa-176">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-176">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="9c3aa-177">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="9c3aa-177">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="9c3aa-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-178">Boolean</span></span>|<span data-ttu-id="9c3aa-179">イントラネット サイトの自動検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-179">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="9c3aa-180">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="9c3aa-180">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="9c3aa-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-181">Boolean</span></span>|<span data-ttu-id="9c3aa-182">エンタープライズ モードのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-182">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="9c3aa-183">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="9c3aa-183">browserBlockJavaScript</span></span>|<span data-ttu-id="9c3aa-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-184">Boolean</span></span>|<span data-ttu-id="9c3aa-185">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-185">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="9c3aa-186">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="9c3aa-186">browserBlockPlugins</span></span>|<span data-ttu-id="9c3aa-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-187">Boolean</span></span>|<span data-ttu-id="9c3aa-188">プラグインを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-188">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="9c3aa-189">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="9c3aa-189">browserBlockPopups</span></span>|<span data-ttu-id="9c3aa-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-190">Boolean</span></span>|<span data-ttu-id="9c3aa-191">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-191">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="9c3aa-192">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="9c3aa-192">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="9c3aa-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-193">Boolean</span></span>|<span data-ttu-id="9c3aa-194">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-194">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="9c3aa-195">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="9c3aa-195">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="9c3aa-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-196">Boolean</span></span>|<span data-ttu-id="9c3aa-197">イントラネット サイトでの 1 単語のエントリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-197">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="9c3aa-198">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="9c3aa-198">browserRequireSmartScreen</span></span>|<span data-ttu-id="9c3aa-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-199">Boolean</span></span>|<span data-ttu-id="9c3aa-200">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-200">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="9c3aa-201">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="9c3aa-201">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="9c3aa-202">文字列</span><span class="sxs-lookup"><span data-stu-id="9c3aa-202">String</span></span>|<span data-ttu-id="9c3aa-203">エンタープライズ モードのサイト リストの場所。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-203">The enterprise mode site list location.</span></span> <span data-ttu-id="9c3aa-204">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-204">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="9c3aa-205">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9c3aa-205">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="9c3aa-206">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9c3aa-206">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="9c3aa-207">インターネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-207">The internet security level.</span></span> <span data-ttu-id="9c3aa-208">可能な値は、`userDefined`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-208">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="9c3aa-209">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9c3aa-209">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="9c3aa-210">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9c3aa-210">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="9c3aa-211">イントラネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-211">The Intranet security level.</span></span> <span data-ttu-id="9c3aa-212">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-212">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="9c3aa-213">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="9c3aa-213">browserLoggingReportLocation</span></span>|<span data-ttu-id="9c3aa-214">String</span><span class="sxs-lookup"><span data-stu-id="9c3aa-214">String</span></span>|<span data-ttu-id="9c3aa-215">ログ レポートの場所。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-215">The logging report location.</span></span>|
|<span data-ttu-id="9c3aa-216">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="9c3aa-216">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="9c3aa-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-217">Boolean</span></span>|<span data-ttu-id="9c3aa-218">制限付きサイトに対する高度なセキュリティを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-218">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="9c3aa-219">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="9c3aa-219">browserRequireFirewall</span></span>|<span data-ttu-id="9c3aa-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-220">Boolean</span></span>|<span data-ttu-id="9c3aa-221">ファイアウォールが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-221">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="9c3aa-222">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="9c3aa-222">browserRequireFraudWarning</span></span>|<span data-ttu-id="9c3aa-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-223">Boolean</span></span>|<span data-ttu-id="9c3aa-224">不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-224">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="9c3aa-225">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9c3aa-225">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="9c3aa-226">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="9c3aa-226">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="9c3aa-227">信頼済みサイトのセキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-227">The trusted sites security level.</span></span> <span data-ttu-id="9c3aa-228">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-228">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="9c3aa-229">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="9c3aa-229">cellularBlockDataRoaming</span></span>|<span data-ttu-id="9c3aa-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-230">Boolean</span></span>|<span data-ttu-id="9c3aa-231">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-231">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="9c3aa-232">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="9c3aa-232">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="9c3aa-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-233">Boolean</span></span>|<span data-ttu-id="9c3aa-234">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-234">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="9c3aa-235">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="9c3aa-235">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="9c3aa-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-236">Boolean</span></span>|<span data-ttu-id="9c3aa-237">ユーザーがピクチャ パスワードおよび暗証番号 (PIN) を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-237">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="9c3aa-238">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="9c3aa-238">passwordExpirationDays</span></span>|<span data-ttu-id="9c3aa-239">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3aa-239">Int32</span></span>|<span data-ttu-id="9c3aa-240">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-240">Password expiration in days.</span></span>|
|<span data-ttu-id="9c3aa-241">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="9c3aa-241">passwordMinimumLength</span></span>|<span data-ttu-id="9c3aa-242">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3aa-242">Int32</span></span>|<span data-ttu-id="9c3aa-243">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-243">The minimum password length.</span></span>|
|<span data-ttu-id="9c3aa-244">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="9c3aa-244">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="9c3aa-245">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3aa-245">Int32</span></span>|<span data-ttu-id="9c3aa-246">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-246">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="9c3aa-247">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="9c3aa-247">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="9c3aa-248">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3aa-248">Int32</span></span>|<span data-ttu-id="9c3aa-249">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-249">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="9c3aa-250">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="9c3aa-250">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="9c3aa-251">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3aa-251">Int32</span></span>|<span data-ttu-id="9c3aa-252">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-252">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="9c3aa-253">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="9c3aa-253">Valid values 0 to 24</span></span>|
|<span data-ttu-id="9c3aa-254">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="9c3aa-254">passwordRequiredType</span></span>|[<span data-ttu-id="9c3aa-255">requiredpasswordtype</span><span class="sxs-lookup"><span data-stu-id="9c3aa-255">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="9c3aa-256">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-256">The required password type.</span></span> <span data-ttu-id="9c3aa-257">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-257">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="9c3aa-258">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="9c3aa-258">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="9c3aa-259">Int32</span><span class="sxs-lookup"><span data-stu-id="9c3aa-259">Int32</span></span>|<span data-ttu-id="9c3aa-260">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-260">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="9c3aa-261">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="9c3aa-261">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="9c3aa-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-262">Boolean</span></span>|<span data-ttu-id="9c3aa-263">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-263">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="9c3aa-264">minimumautoinstallclassification</span><span class="sxs-lookup"><span data-stu-id="9c3aa-264">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="9c3aa-265">updateClassification</span><span class="sxs-lookup"><span data-stu-id="9c3aa-265">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="9c3aa-266">自動的にインストールする最小更新プログラムの分類。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-266">The minimum update classification to install automatically.</span></span> <span data-ttu-id="9c3aa-267">可能な値は、`userDefined`、`recommendedAndImportant`、`important`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-267">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="9c3aa-268">minimumautoinstall分類の更新</span><span class="sxs-lookup"><span data-stu-id="9c3aa-268">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="9c3aa-269">updateClassification</span><span class="sxs-lookup"><span data-stu-id="9c3aa-269">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="9c3aa-270">自動的にインストールする最小更新プログラムの分類。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-270">The minimum update classification to install automatically.</span></span> <span data-ttu-id="9c3aa-271">可能な値は、`userDefined`、`recommendedAndImportant`、`important`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-271">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="9c3aa-272">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="9c3aa-272">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="9c3aa-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="9c3aa-273">Boolean</span></span>|<span data-ttu-id="9c3aa-274">自動更新が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-274">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="9c3aa-275">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="9c3aa-275">userAccountControlSettings</span></span>|[<span data-ttu-id="9c3aa-276">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="9c3aa-276">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="9c3aa-277">ユーザー アカウント制御の設定。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-277">The user account control settings.</span></span> <span data-ttu-id="9c3aa-278">可能な値は、`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify` です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-278">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="9c3aa-279">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="9c3aa-279">workFoldersUrl</span></span>|<span data-ttu-id="9c3aa-280">String</span><span class="sxs-lookup"><span data-stu-id="9c3aa-280">String</span></span>|<span data-ttu-id="9c3aa-281">作業フォルダーの URL。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-281">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="9c3aa-282">応答</span><span class="sxs-lookup"><span data-stu-id="9c3aa-282">Response</span></span>
<span data-ttu-id="9c3aa-283">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-283">If successful, this method returns a `200 OK` response code and an updated [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9c3aa-284">例</span><span class="sxs-lookup"><span data-stu-id="9c3aa-284">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c3aa-285">要求</span><span class="sxs-lookup"><span data-stu-id="9c3aa-285">Request</span></span>
<span data-ttu-id="9c3aa-286">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-286">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1924

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```

### <a name="response"></a><span data-ttu-id="9c3aa-287">応答</span><span class="sxs-lookup"><span data-stu-id="9c3aa-287">Response</span></span>
<span data-ttu-id="9c3aa-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9c3aa-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2096

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "minimumAutoInstallClassification": "recommendedAndImportant",
  "updatesMinimumAutoInstallClassification": "recommendedAndImportant",
  "updatesRequireAutomaticUpdates": true,
  "userAccountControlSettings": "alwaysNotify",
  "workFoldersUrl": "https://example.com/workFoldersUrl/"
}
```





