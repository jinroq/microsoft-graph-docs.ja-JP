---
title: Create windows81GeneralConfiguration
description: 新しい windows81GeneralConfiguration オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: c06b6f4a955d904b1da65b11e99ef4af307004cb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319748"
---
# <a name="create-windows81generalconfiguration"></a><span data-ttu-id="8d2b9-103">Create windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="8d2b9-103">Create windows81GeneralConfiguration</span></span>

> <span data-ttu-id="8d2b9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d2b9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d2b9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d2b9-107">新しい [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-107">Create a new [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8d2b9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8d2b9-108">Prerequisites</span></span>
<span data-ttu-id="8d2b9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8d2b9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8d2b9-111">Permission type</span></span>|<span data-ttu-id="8d2b9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8d2b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8d2b9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8d2b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8d2b9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8d2b9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8d2b9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8d2b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8d2b9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-116">Not supported.</span></span>|
|<span data-ttu-id="8d2b9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8d2b9-117">Application</span></span>|<span data-ttu-id="8d2b9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8d2b9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8d2b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8d2b9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d2b9-120">Request headers</span></span>
|<span data-ttu-id="8d2b9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8d2b9-121">Header</span></span>|<span data-ttu-id="8d2b9-122">値</span><span class="sxs-lookup"><span data-stu-id="8d2b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8d2b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8d2b9-123">Authorization</span></span>|<span data-ttu-id="8d2b9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8d2b9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8d2b9-125">Accept</span></span>|<span data-ttu-id="8d2b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8d2b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8d2b9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8d2b9-127">Request body</span></span>
<span data-ttu-id="8d2b9-128">要求本文で、windows81GeneralConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-128">In the request body, supply a JSON representation for the windows81GeneralConfiguration object.</span></span>

<span data-ttu-id="8d2b9-129">次の表に、windows81GeneralConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-129">The following table shows the properties that are required when you create the windows81GeneralConfiguration.</span></span>

|<span data-ttu-id="8d2b9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d2b9-130">Property</span></span>|<span data-ttu-id="8d2b9-131">種類</span><span class="sxs-lookup"><span data-stu-id="8d2b9-131">Type</span></span>|<span data-ttu-id="8d2b9-132">説明</span><span class="sxs-lookup"><span data-stu-id="8d2b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d2b9-133">ID</span><span class="sxs-lookup"><span data-stu-id="8d2b9-133">id</span></span>|<span data-ttu-id="8d2b9-134">String</span><span class="sxs-lookup"><span data-stu-id="8d2b9-134">String</span></span>|<span data-ttu-id="8d2b9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-135">Key of the entity.</span></span> <span data-ttu-id="8d2b9-136">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d2b9-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d2b9-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8d2b9-137">lastModifiedDateTime</span></span>|<span data-ttu-id="8d2b9-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d2b9-138">DateTimeOffset</span></span>|<span data-ttu-id="8d2b9-139">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-139">DateTime the object was last modified.</span></span> <span data-ttu-id="8d2b9-140">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d2b9-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d2b9-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8d2b9-141">roleScopeTagIds</span></span>|<span data-ttu-id="8d2b9-142">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8d2b9-142">String collection</span></span>|<span data-ttu-id="8d2b9-143">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8d2b9-144">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d2b9-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d2b9-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8d2b9-145">supportsScopeTags</span></span>|<span data-ttu-id="8d2b9-146">ブール型</span><span class="sxs-lookup"><span data-stu-id="8d2b9-146">Boolean</span></span>|<span data-ttu-id="8d2b9-147">デバイスの構成を基になるスコープのタグの割り当てをサポートしているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8d2b9-148">この値が false であり、エンティティをスコープ指定されたユーザーには表示されませんがある場合、ScopeTags プロパティに割り当てることは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8d2b9-149">これは、Silverlight で作成されたレガシ ポリシーに対して発生し、削除して、Azure ポータル内のポリシーを再作成することで解決できます。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8d2b9-150">このプロパティは読み取りのみ可能です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-150">This property is read-only.</span></span> <span data-ttu-id="8d2b9-151">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d2b9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d2b9-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8d2b9-152">createdDateTime</span></span>|<span data-ttu-id="8d2b9-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d2b9-153">DateTimeOffset</span></span>|<span data-ttu-id="8d2b9-154">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-154">DateTime the object was created.</span></span> <span data-ttu-id="8d2b9-155">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d2b9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d2b9-156">説明</span><span class="sxs-lookup"><span data-stu-id="8d2b9-156">description</span></span>|<span data-ttu-id="8d2b9-157">String</span><span class="sxs-lookup"><span data-stu-id="8d2b9-157">String</span></span>|<span data-ttu-id="8d2b9-158">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8d2b9-159">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d2b9-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d2b9-160">displayName</span><span class="sxs-lookup"><span data-stu-id="8d2b9-160">displayName</span></span>|<span data-ttu-id="8d2b9-161">String</span><span class="sxs-lookup"><span data-stu-id="8d2b9-161">String</span></span>|<span data-ttu-id="8d2b9-162">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8d2b9-163">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d2b9-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d2b9-164">version</span><span class="sxs-lookup"><span data-stu-id="8d2b9-164">version</span></span>|<span data-ttu-id="8d2b9-165">Int32</span><span class="sxs-lookup"><span data-stu-id="8d2b9-165">Int32</span></span>|<span data-ttu-id="8d2b9-166">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-166">Version of the device configuration.</span></span> <span data-ttu-id="8d2b9-167">[deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8d2b9-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8d2b9-168">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="8d2b9-168">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="8d2b9-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-169">Boolean</span></span>|<span data-ttu-id="8d2b9-170">Microsoft アカウントに関連付けられていない電子メール アカウントをユーザーがデバイスに追加できないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-170">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="8d2b9-171">applyOnlyToWindows81</span><span class="sxs-lookup"><span data-stu-id="8d2b9-171">applyOnlyToWindows81</span></span>|<span data-ttu-id="8d2b9-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-172">Boolean</span></span>|<span data-ttu-id="8d2b9-173">このポリシーを Windows 8.1 にのみ適用するかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-173">Value indicating whether this policy only applies to Windows 8.1.</span></span> <span data-ttu-id="8d2b9-174">このプロパティは読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-174">This property is read-only.</span></span>|
|<span data-ttu-id="8d2b9-175">browserBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="8d2b9-175">browserBlockAutofill</span></span>|<span data-ttu-id="8d2b9-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-176">Boolean</span></span>|<span data-ttu-id="8d2b9-177">自動入力を禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-177">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="8d2b9-178">browserBlockAutomaticDetectionOfIntranetSites</span><span class="sxs-lookup"><span data-stu-id="8d2b9-178">browserBlockAutomaticDetectionOfIntranetSites</span></span>|<span data-ttu-id="8d2b9-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-179">Boolean</span></span>|<span data-ttu-id="8d2b9-180">イントラネット サイトの自動検出をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-180">Indicates whether or not to block automatic detection of Intranet sites.</span></span>|
|<span data-ttu-id="8d2b9-181">browserBlockEnterpriseModeAccess</span><span class="sxs-lookup"><span data-stu-id="8d2b9-181">browserBlockEnterpriseModeAccess</span></span>|<span data-ttu-id="8d2b9-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-182">Boolean</span></span>|<span data-ttu-id="8d2b9-183">エンタープライズ モードのアクセスを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-183">Indicates whether or not to block enterprise mode access.</span></span>|
|<span data-ttu-id="8d2b9-184">browserBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="8d2b9-184">browserBlockJavaScript</span></span>|<span data-ttu-id="8d2b9-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-185">Boolean</span></span>|<span data-ttu-id="8d2b9-186">ユーザーが JavaScript を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-186">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="8d2b9-187">browserBlockPlugins</span><span class="sxs-lookup"><span data-stu-id="8d2b9-187">browserBlockPlugins</span></span>|<span data-ttu-id="8d2b9-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-188">Boolean</span></span>|<span data-ttu-id="8d2b9-189">プラグインを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-189">Indicates whether or not to block plug-ins.</span></span>|
|<span data-ttu-id="8d2b9-190">browserBlockPopups</span><span class="sxs-lookup"><span data-stu-id="8d2b9-190">browserBlockPopups</span></span>|<span data-ttu-id="8d2b9-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-191">Boolean</span></span>|<span data-ttu-id="8d2b9-192">ポップアップをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-192">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="8d2b9-193">browserBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="8d2b9-193">browserBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="8d2b9-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-194">Boolean</span></span>|<span data-ttu-id="8d2b9-195">ユーザーがトラッキング拒否ヘッダーを送信することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-195">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="8d2b9-196">browserBlockSingleWordEntryOnIntranetSites</span><span class="sxs-lookup"><span data-stu-id="8d2b9-196">browserBlockSingleWordEntryOnIntranetSites</span></span>|<span data-ttu-id="8d2b9-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-197">Boolean</span></span>|<span data-ttu-id="8d2b9-198">イントラネット サイトでの 1 単語のエントリを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-198">Indicates whether or not to block a single word entry on Intranet sites.</span></span>|
|<span data-ttu-id="8d2b9-199">browserRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="8d2b9-199">browserRequireSmartScreen</span></span>|<span data-ttu-id="8d2b9-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-200">Boolean</span></span>|<span data-ttu-id="8d2b9-201">スマート スクリーン フィルターの使用をユーザーに要求するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-201">Indicates whether or not to require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="8d2b9-202">browserEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="8d2b9-202">browserEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="8d2b9-203">String</span><span class="sxs-lookup"><span data-stu-id="8d2b9-203">String</span></span>|<span data-ttu-id="8d2b9-204">エンタープライズ モードのサイト リストの場所。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-204">The enterprise mode site list location.</span></span> <span data-ttu-id="8d2b9-205">ローカル ファイル、ローカル ネットワーク、http の場所が該当します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-205">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="8d2b9-206">browserInternetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d2b9-206">browserInternetSecurityLevel</span></span>|[<span data-ttu-id="8d2b9-207">internetSiteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d2b9-207">internetSiteSecurityLevel</span></span>](../resources/intune-deviceconfig-internetsitesecuritylevel.md)|<span data-ttu-id="8d2b9-208">インターネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-208">The internet security level.</span></span> <span data-ttu-id="8d2b9-209">可能な値は、`userDefined`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-209">Possible values are: `userDefined`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8d2b9-210">browserIntranetSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d2b9-210">browserIntranetSecurityLevel</span></span>|[<span data-ttu-id="8d2b9-211">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d2b9-211">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="8d2b9-212">イントラネット セキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-212">The Intranet security level.</span></span> <span data-ttu-id="8d2b9-213">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-213">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8d2b9-214">browserLoggingReportLocation</span><span class="sxs-lookup"><span data-stu-id="8d2b9-214">browserLoggingReportLocation</span></span>|<span data-ttu-id="8d2b9-215">String</span><span class="sxs-lookup"><span data-stu-id="8d2b9-215">String</span></span>|<span data-ttu-id="8d2b9-216">ログ レポートの場所。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-216">The logging report location.</span></span>|
|<span data-ttu-id="8d2b9-217">browserRequireHighSecurityForRestrictedSites</span><span class="sxs-lookup"><span data-stu-id="8d2b9-217">browserRequireHighSecurityForRestrictedSites</span></span>|<span data-ttu-id="8d2b9-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-218">Boolean</span></span>|<span data-ttu-id="8d2b9-219">制限付きサイトに対する高度なセキュリティを必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-219">Indicates whether or not to require high security for restricted sites.</span></span>|
|<span data-ttu-id="8d2b9-220">browserRequireFirewall</span><span class="sxs-lookup"><span data-stu-id="8d2b9-220">browserRequireFirewall</span></span>|<span data-ttu-id="8d2b9-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-221">Boolean</span></span>|<span data-ttu-id="8d2b9-222">ファイアウォールが必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-222">Indicates whether or not to require a firewall.</span></span>|
|<span data-ttu-id="8d2b9-223">browserRequireFraudWarning</span><span class="sxs-lookup"><span data-stu-id="8d2b9-223">browserRequireFraudWarning</span></span>|<span data-ttu-id="8d2b9-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-224">Boolean</span></span>|<span data-ttu-id="8d2b9-225">不正行為の警告を必要とするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-225">Indicates whether or not to require fraud warning.</span></span>|
|<span data-ttu-id="8d2b9-226">browserTrustedSitesSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d2b9-226">browserTrustedSitesSecurityLevel</span></span>|[<span data-ttu-id="8d2b9-227">siteSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="8d2b9-227">siteSecurityLevel</span></span>](../resources/intune-deviceconfig-sitesecuritylevel.md)|<span data-ttu-id="8d2b9-228">信頼済みサイトのセキュリティ レベル。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-228">The trusted sites security level.</span></span> <span data-ttu-id="8d2b9-229">可能な値は、`userDefined`、`low`、`mediumLow`、`medium`、`mediumHigh`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-229">Possible values are: `userDefined`, `low`, `mediumLow`, `medium`, `mediumHigh`, `high`.</span></span>|
|<span data-ttu-id="8d2b9-230">cellularBlockDataRoaming</span><span class="sxs-lookup"><span data-stu-id="8d2b9-230">cellularBlockDataRoaming</span></span>|<span data-ttu-id="8d2b9-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-231">Boolean</span></span>|<span data-ttu-id="8d2b9-232">データ ローミングをブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-232">Indicates whether or not to block data roaming.</span></span>|
|<span data-ttu-id="8d2b9-233">diagnosticsBlockDataSubmission</span><span class="sxs-lookup"><span data-stu-id="8d2b9-233">diagnosticsBlockDataSubmission</span></span>|<span data-ttu-id="8d2b9-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-234">Boolean</span></span>|<span data-ttu-id="8d2b9-235">診断データの送信をブロックするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-235">Indicates whether or not to block diagnostic data submission.</span></span>|
|<span data-ttu-id="8d2b9-236">passwordBlockPicturePasswordAndPin</span><span class="sxs-lookup"><span data-stu-id="8d2b9-236">passwordBlockPicturePasswordAndPin</span></span>|<span data-ttu-id="8d2b9-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-237">Boolean</span></span>|<span data-ttu-id="8d2b9-238">ユーザーがピクチャ パスワードおよび暗証番号 (PIN) を使用することを禁止するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-238">Indicates whether or not to Block the user from using a pictures password and pin.</span></span>|
|<span data-ttu-id="8d2b9-239">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="8d2b9-239">passwordExpirationDays</span></span>|<span data-ttu-id="8d2b9-240">Int32</span><span class="sxs-lookup"><span data-stu-id="8d2b9-240">Int32</span></span>|<span data-ttu-id="8d2b9-241">パスワードの有効期限 (日数)。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-241">Password expiration in days.</span></span>|
|<span data-ttu-id="8d2b9-242">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="8d2b9-242">passwordMinimumLength</span></span>|<span data-ttu-id="8d2b9-243">Int32</span><span class="sxs-lookup"><span data-stu-id="8d2b9-243">Int32</span></span>|<span data-ttu-id="8d2b9-244">パスワードの最小文字数。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-244">The minimum password length.</span></span>|
|<span data-ttu-id="8d2b9-245">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="8d2b9-245">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="8d2b9-246">Int32</span><span class="sxs-lookup"><span data-stu-id="8d2b9-246">Int32</span></span>|<span data-ttu-id="8d2b9-247">画面がタイムアウトになるまでの非アクティブ時間 (分)。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-247">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="8d2b9-248">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="8d2b9-248">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="8d2b9-249">Int32</span><span class="sxs-lookup"><span data-stu-id="8d2b9-249">Int32</span></span>|<span data-ttu-id="8d2b9-250">パスワードに必要な文字セットの数。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-250">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="8d2b9-251">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="8d2b9-251">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="8d2b9-252">Int32</span><span class="sxs-lookup"><span data-stu-id="8d2b9-252">Int32</span></span>|<span data-ttu-id="8d2b9-253">再使用を禁止する、以前のパスワードの数。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-253">The number of previous passwords to prevent re-use of.</span></span> <span data-ttu-id="8d2b9-254">有効な値は 0 から 24 までです</span><span class="sxs-lookup"><span data-stu-id="8d2b9-254">Valid values 0 to 24</span></span>|
|<span data-ttu-id="8d2b9-255">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="8d2b9-255">passwordRequiredType</span></span>|[<span data-ttu-id="8d2b9-256">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="8d2b9-256">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="8d2b9-257">必要なパスワードの種類。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-257">The required password type.</span></span> <span data-ttu-id="8d2b9-258">可能な値は、`deviceDefault`、`alphanumeric`、`numeric` です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-258">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="8d2b9-259">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="8d2b9-259">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="8d2b9-260">Int32</span><span class="sxs-lookup"><span data-stu-id="8d2b9-260">Int32</span></span>|<span data-ttu-id="8d2b9-261">出荷時の設定にリセットされるサインインの失敗回数。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-261">The number of sign in failures before factory reset.</span></span>|
|<span data-ttu-id="8d2b9-262">storageRequireDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="8d2b9-262">storageRequireDeviceEncryption</span></span>|<span data-ttu-id="8d2b9-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-263">Boolean</span></span>|<span data-ttu-id="8d2b9-264">モバイル デバイスでの暗号化が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-264">Indicates whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="8d2b9-265">minimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="8d2b9-265">minimumAutoInstallClassification</span></span>|[<span data-ttu-id="8d2b9-266">updateClassification</span><span class="sxs-lookup"><span data-stu-id="8d2b9-266">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="8d2b9-267">最小値は、自動的にインストールするのにはクラス分けを更新します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-267">The minimum update classification to install automatically.</span></span> <span data-ttu-id="8d2b9-268">可能な値は、`userDefined`、`recommendedAndImportant`、`important`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-268">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="8d2b9-269">updatesMinimumAutoInstallClassification</span><span class="sxs-lookup"><span data-stu-id="8d2b9-269">updatesMinimumAutoInstallClassification</span></span>|[<span data-ttu-id="8d2b9-270">updateClassification</span><span class="sxs-lookup"><span data-stu-id="8d2b9-270">updateClassification</span></span>](../resources/intune-deviceconfig-updateclassification.md)|<span data-ttu-id="8d2b9-271">最小値は、自動的にインストールするのにはクラス分けを更新します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-271">The minimum update classification to install automatically.</span></span> <span data-ttu-id="8d2b9-272">可能な値は、`userDefined`、`recommendedAndImportant`、`important`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-272">Possible values are: `userDefined`, `recommendedAndImportant`, `important`, `none`.</span></span>|
|<span data-ttu-id="8d2b9-273">updatesRequireAutomaticUpdates</span><span class="sxs-lookup"><span data-stu-id="8d2b9-273">updatesRequireAutomaticUpdates</span></span>|<span data-ttu-id="8d2b9-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="8d2b9-274">Boolean</span></span>|<span data-ttu-id="8d2b9-275">自動更新が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-275">Indicates whether or not to require automatic updates.</span></span>|
|<span data-ttu-id="8d2b9-276">userAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8d2b9-276">userAccountControlSettings</span></span>|[<span data-ttu-id="8d2b9-277">windowsUserAccountControlSettings</span><span class="sxs-lookup"><span data-stu-id="8d2b9-277">windowsUserAccountControlSettings</span></span>](../resources/intune-deviceconfig-windowsuseraccountcontrolsettings.md)|<span data-ttu-id="8d2b9-278">ユーザー アカウント制御の設定。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-278">The user account control settings.</span></span> <span data-ttu-id="8d2b9-279">可能な値は、`userDefined`、`alwaysNotify`、`notifyOnAppChanges`、`notifyOnAppChangesWithoutDimming`、`neverNotify` です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-279">Possible values are: `userDefined`, `alwaysNotify`, `notifyOnAppChanges`, `notifyOnAppChangesWithoutDimming`, `neverNotify`.</span></span>|
|<span data-ttu-id="8d2b9-280">workFoldersUrl</span><span class="sxs-lookup"><span data-stu-id="8d2b9-280">workFoldersUrl</span></span>|<span data-ttu-id="8d2b9-281">String</span><span class="sxs-lookup"><span data-stu-id="8d2b9-281">String</span></span>|<span data-ttu-id="8d2b9-282">作業フォルダーの URL。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-282">The work folders url.</span></span>|



## <a name="response"></a><span data-ttu-id="8d2b9-283">応答</span><span class="sxs-lookup"><span data-stu-id="8d2b9-283">Response</span></span>
<span data-ttu-id="8d2b9-284">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-284">If successful, this method returns a `201 Created` response code and a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8d2b9-285">例</span><span class="sxs-lookup"><span data-stu-id="8d2b9-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="8d2b9-286">要求</span><span class="sxs-lookup"><span data-stu-id="8d2b9-286">Request</span></span>
<span data-ttu-id="8d2b9-287">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="8d2b9-288">応答</span><span class="sxs-lookup"><span data-stu-id="8d2b9-288">Response</span></span>
<span data-ttu-id="8d2b9-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8d2b9-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





