---
title: Create defaultManagedAppProtection
description: 新しい defaultManagedAppProtection オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f0da26a10f0925e3b347d971f303f58aef035b8c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146208"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="0477a-103">Create defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="0477a-103">Create defaultManagedAppProtection</span></span>

> <span data-ttu-id="0477a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0477a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0477a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0477a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0477a-106">新しい [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0477a-106">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0477a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0477a-107">Prerequisites</span></span>
<span data-ttu-id="0477a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0477a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0477a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0477a-110">Permission type</span></span>|<span data-ttu-id="0477a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0477a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0477a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0477a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0477a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0477a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0477a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0477a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0477a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0477a-115">Not supported.</span></span>|
|<span data-ttu-id="0477a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0477a-116">Application</span></span>|<span data-ttu-id="0477a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0477a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0477a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0477a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="0477a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0477a-119">Request headers</span></span>
|<span data-ttu-id="0477a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0477a-120">Header</span></span>|<span data-ttu-id="0477a-121">値</span><span class="sxs-lookup"><span data-stu-id="0477a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0477a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0477a-122">Authorization</span></span>|<span data-ttu-id="0477a-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0477a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0477a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0477a-124">Accept</span></span>|<span data-ttu-id="0477a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0477a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0477a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0477a-126">Request body</span></span>
<span data-ttu-id="0477a-127">要求本文において、defaultManagedAppProtection オブジェクト用の JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="0477a-127">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="0477a-128">次の表に、defaultManagedAppProtection 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-128">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="0477a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0477a-129">Property</span></span>|<span data-ttu-id="0477a-130">型</span><span class="sxs-lookup"><span data-stu-id="0477a-130">Type</span></span>|<span data-ttu-id="0477a-131">説明</span><span class="sxs-lookup"><span data-stu-id="0477a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0477a-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0477a-132">displayName</span></span>|<span data-ttu-id="0477a-133">String</span><span class="sxs-lookup"><span data-stu-id="0477a-133">String</span></span>|<span data-ttu-id="0477a-134">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="0477a-134">Policy display name.</span></span> <span data-ttu-id="0477a-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0477a-136">説明</span><span class="sxs-lookup"><span data-stu-id="0477a-136">description</span></span>|<span data-ttu-id="0477a-137">String</span><span class="sxs-lookup"><span data-stu-id="0477a-137">String</span></span>|<span data-ttu-id="0477a-138">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="0477a-138">The policy's description.</span></span> <span data-ttu-id="0477a-139">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0477a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0477a-140">createdDateTime</span></span>|<span data-ttu-id="0477a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0477a-141">DateTimeOffset</span></span>|<span data-ttu-id="0477a-142">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0477a-142">The date and time the policy was created.</span></span> <span data-ttu-id="0477a-143">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0477a-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0477a-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0477a-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0477a-145">DateTimeOffset</span></span>|<span data-ttu-id="0477a-146">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="0477a-146">Last time the policy was modified.</span></span> <span data-ttu-id="0477a-147">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0477a-148">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0477a-148">roleScopeTagIds</span></span>|<span data-ttu-id="0477a-149">String collection</span><span class="sxs-lookup"><span data-stu-id="0477a-149">String collection</span></span>|<span data-ttu-id="0477a-150">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="0477a-150">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0477a-151">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-151">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0477a-152">id</span><span class="sxs-lookup"><span data-stu-id="0477a-152">id</span></span>|<span data-ttu-id="0477a-153">文字列</span><span class="sxs-lookup"><span data-stu-id="0477a-153">String</span></span>|<span data-ttu-id="0477a-154">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0477a-154">Key of the entity.</span></span> <span data-ttu-id="0477a-155">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-155">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0477a-156">version</span><span class="sxs-lookup"><span data-stu-id="0477a-156">version</span></span>|<span data-ttu-id="0477a-157">String</span><span class="sxs-lookup"><span data-stu-id="0477a-157">String</span></span>|<span data-ttu-id="0477a-158">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="0477a-158">Version of the entity.</span></span> <span data-ttu-id="0477a-159">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-159">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="0477a-160">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="0477a-160">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="0477a-161">Duration</span><span class="sxs-lookup"><span data-stu-id="0477a-161">Duration</span></span>|<span data-ttu-id="0477a-162">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="0477a-162">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="0477a-163">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-163">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-164">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="0477a-164">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="0477a-165">Duration</span><span class="sxs-lookup"><span data-stu-id="0477a-165">Duration</span></span>|<span data-ttu-id="0477a-166">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="0477a-166">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="0477a-167">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-167">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-168">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="0477a-168">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="0477a-169">managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="0477a-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="0477a-170">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="0477a-170">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="0477a-171">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0477a-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="0477a-172">可能な値は `allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="0477a-173">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="0477a-173">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="0477a-174">managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="0477a-174">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="0477a-175">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="0477a-175">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="0477a-176">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0477a-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="0477a-177">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-177">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="0477a-178">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="0477a-178">organizationalCredentialsRequired</span></span>|<span data-ttu-id="0477a-179">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-179">Boolean</span></span>|<span data-ttu-id="0477a-180">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-180">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="0477a-181">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-181">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-182">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="0477a-182">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="0477a-183">managedappクリップボードの sharinglevel</span><span class="sxs-lookup"><span data-stu-id="0477a-183">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="0477a-184">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="0477a-184">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="0477a-185">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0477a-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="0477a-186">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-186">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="0477a-187">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-187">dataBackupBlocked</span></span>|<span data-ttu-id="0477a-188">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-188">Boolean</span></span>|<span data-ttu-id="0477a-189">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-189">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="0477a-190">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-190">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-191">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="0477a-191">deviceComplianceRequired</span></span>|<span data-ttu-id="0477a-192">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-192">Boolean</span></span>|<span data-ttu-id="0477a-193">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-193">Indicates whether device compliance is required.</span></span> <span data-ttu-id="0477a-194">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-194">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-195">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="0477a-195">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="0477a-196">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-196">Boolean</span></span>|<span data-ttu-id="0477a-197">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-197">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="0477a-198">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-198">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-199">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-199">saveAsBlocked</span></span>|<span data-ttu-id="0477a-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="0477a-200">Boolean</span></span>|<span data-ttu-id="0477a-201">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-201">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="0477a-202">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-202">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-203">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="0477a-203">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="0477a-204">Duration</span><span class="sxs-lookup"><span data-stu-id="0477a-204">Duration</span></span>|<span data-ttu-id="0477a-205">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="0477a-205">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="0477a-206">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-206">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-207">pinRequired</span><span class="sxs-lookup"><span data-stu-id="0477a-207">pinRequired</span></span>|<span data-ttu-id="0477a-208">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-208">Boolean</span></span>|<span data-ttu-id="0477a-209">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-209">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="0477a-210">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-210">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-211">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="0477a-211">maximumPinRetries</span></span>|<span data-ttu-id="0477a-212">Int32</span><span class="sxs-lookup"><span data-stu-id="0477a-212">Int32</span></span>|<span data-ttu-id="0477a-213">管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。</span><span class="sxs-lookup"><span data-stu-id="0477a-213">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="0477a-214">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-214">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-215">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-215">simplePinBlocked</span></span>|<span data-ttu-id="0477a-216">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-216">Boolean</span></span>|<span data-ttu-id="0477a-217">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-217">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="0477a-218">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-218">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-219">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="0477a-219">minimumPinLength</span></span>|<span data-ttu-id="0477a-220">Int32</span><span class="sxs-lookup"><span data-stu-id="0477a-220">Int32</span></span>|<span data-ttu-id="0477a-221">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="0477a-221">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-222">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="0477a-222">pinCharacterSet</span></span>|[<span data-ttu-id="0477a-223">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="0477a-223">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="0477a-224">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="0477a-224">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="0477a-225">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0477a-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="0477a-226">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-226">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="0477a-227">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="0477a-227">periodBeforePinReset</span></span>|<span data-ttu-id="0477a-228">Duration</span><span class="sxs-lookup"><span data-stu-id="0477a-228">Duration</span></span>|<span data-ttu-id="0477a-229">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0477a-229">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="0477a-230">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-230">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-231">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="0477a-231">allowedDataStorageLocations</span></span>|<span data-ttu-id="0477a-232">[managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="0477a-232">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="0477a-233">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="0477a-233">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="0477a-234">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0477a-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="0477a-235">可能な値は `oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-235">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="0477a-236">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-236">contactSyncBlocked</span></span>|<span data-ttu-id="0477a-237">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-237">Boolean</span></span>|<span data-ttu-id="0477a-238">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-238">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="0477a-239">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-239">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-240">printBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-240">printBlocked</span></span>|<span data-ttu-id="0477a-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="0477a-241">Boolean</span></span>|<span data-ttu-id="0477a-242">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-242">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="0477a-243">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-243">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-244">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-244">fingerprintBlocked</span></span>|<span data-ttu-id="0477a-245">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-245">Boolean</span></span>|<span data-ttu-id="0477a-246">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-246">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="0477a-247">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-247">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-248">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="0477a-248">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="0477a-249">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-249">Boolean</span></span>|<span data-ttu-id="0477a-250">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-250">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="0477a-251">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-251">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-252">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-252">minimumRequiredOsVersion</span></span>|<span data-ttu-id="0477a-253">String</span><span class="sxs-lookup"><span data-stu-id="0477a-253">String</span></span>|<span data-ttu-id="0477a-254">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="0477a-254">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="0477a-255">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-255">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-256">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-256">minimumWarningOsVersion</span></span>|<span data-ttu-id="0477a-257">String</span><span class="sxs-lookup"><span data-stu-id="0477a-257">String</span></span>|<span data-ttu-id="0477a-258">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0477a-258">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="0477a-259">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-259">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-260">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-260">minimumRequiredAppVersion</span></span>|<span data-ttu-id="0477a-261">String</span><span class="sxs-lookup"><span data-stu-id="0477a-261">String</span></span>|<span data-ttu-id="0477a-262">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="0477a-262">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="0477a-263">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-263">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-264">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-264">minimumWarningAppVersion</span></span>|<span data-ttu-id="0477a-265">String</span><span class="sxs-lookup"><span data-stu-id="0477a-265">String</span></span>|<span data-ttu-id="0477a-266">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="0477a-266">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="0477a-267">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-267">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-268">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-268">minimumWipeOsVersion</span></span>|<span data-ttu-id="0477a-269">String</span><span class="sxs-lookup"><span data-stu-id="0477a-269">String</span></span>|<span data-ttu-id="0477a-270">指定したバージョン以下のバージョンでは、管理対象アプリと関連付けられている会社データがワイプされます。</span><span class="sxs-lookup"><span data-stu-id="0477a-270">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="0477a-271">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-271">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-272">minimumwipeappversion</span><span class="sxs-lookup"><span data-stu-id="0477a-272">minimumWipeAppVersion</span></span>|<span data-ttu-id="0477a-273">String</span><span class="sxs-lookup"><span data-stu-id="0477a-273">String</span></span>|<span data-ttu-id="0477a-274">指定したバージョン以下のバージョンでは、管理対象アプリと関連付けられている会社データがワイプされます。</span><span class="sxs-lookup"><span data-stu-id="0477a-274">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="0477a-275">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0477a-275">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-276">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="0477a-276">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="0477a-277">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="0477a-277">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="0477a-278">DeviceComplianceRequired が true に設定されている場合、デバイスがルートまたは脱獄のどちらかの場合に、管理対象アプリの動作 (ブロックまたはワイプ) を定義します。</span><span class="sxs-lookup"><span data-stu-id="0477a-278">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="0477a-279">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0477a-279">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="0477a-280">可能な値は `block`、`wipe`、`warn` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-280">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="0477a-281">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="0477a-281">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="0477a-282">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="0477a-282">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="0477a-283">正しくない pin の再試行回数の最大数に基づいて、管理対象アプリの動作 (ブロックまたはワイプ) を定義します。</span><span class="sxs-lookup"><span data-stu-id="0477a-283">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="0477a-284">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="0477a-284">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="0477a-285">可能な値は `block`、`wipe`、`warn` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-285">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="0477a-286">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="0477a-286">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="0477a-287">Duration</span><span class="sxs-lookup"><span data-stu-id="0477a-287">Duration</span></span>|<span data-ttu-id="0477a-288">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承された非バイオメトリクスパスコードではなく、アプリ pin のタイムアウト (分単位)</span><span class="sxs-lookup"><span data-stu-id="0477a-288">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="0477a-289">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="0477a-289">appDataEncryptionType</span></span>|[<span data-ttu-id="0477a-290">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="0477a-290">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="0477a-291">管理対象アプリのデータに使用する暗号化の種類。</span><span class="sxs-lookup"><span data-stu-id="0477a-291">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="0477a-292">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="0477a-292">(iOS Only).</span></span> <span data-ttu-id="0477a-293">使用可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-293">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="0477a-294">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-294">screenCaptureBlocked</span></span>|<span data-ttu-id="0477a-295">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-295">Boolean</span></span>|<span data-ttu-id="0477a-296">画面キャプチャがブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-296">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="0477a-297">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-297">(Android only)</span></span>|
|<span data-ttu-id="0477a-298">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="0477a-298">encryptAppData</span></span>|<span data-ttu-id="0477a-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="0477a-299">Boolean</span></span>|<span data-ttu-id="0477a-300">管理対象アプリのデータを暗号化するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-300">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="0477a-301">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-301">(Android only)</span></span>|
|<span data-ttu-id="0477a-302">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="0477a-302">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="0477a-303">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-303">Boolean</span></span>|<span data-ttu-id="0477a-304">この設定を有効にすると、デバイスレベルの暗号化が有効になっている場合、アプリレベルの暗号化が無効になります。</span><span class="sxs-lookup"><span data-stu-id="0477a-304">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="0477a-305">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-305">(Android only)</span></span>|
|<span data-ttu-id="0477a-306">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-306">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="0477a-307">String</span><span class="sxs-lookup"><span data-stu-id="0477a-307">String</span></span>|<span data-ttu-id="0477a-308">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="0477a-308">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="0477a-309">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-309">(iOS Only)</span></span>|
|<span data-ttu-id="0477a-310">customSettings</span><span class="sxs-lookup"><span data-stu-id="0477a-310">customSettings</span></span>|<span data-ttu-id="0477a-311">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0477a-311">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0477a-312">このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="0477a-312">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="0477a-313">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="0477a-313">deployedAppCount</span></span>|<span data-ttu-id="0477a-314">Int32</span><span class="sxs-lookup"><span data-stu-id="0477a-314">Int32</span></span>|<span data-ttu-id="0477a-315">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="0477a-315">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="0477a-316">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-316">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="0477a-317">String</span><span class="sxs-lookup"><span data-stu-id="0477a-317">String</span></span>|<span data-ttu-id="0477a-318">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="0477a-318">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="0477a-319">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-319">(Android only)</span></span>|
|<span data-ttu-id="0477a-320">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-320">minimumWarningPatchVersion</span></span>|<span data-ttu-id="0477a-321">String</span><span class="sxs-lookup"><span data-stu-id="0477a-321">String</span></span>|<span data-ttu-id="0477a-322">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="0477a-322">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="0477a-323">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-323">(Android only)</span></span>|
|<span data-ttu-id="0477a-324">exemptedAppProtocols</span><span class="sxs-lookup"><span data-stu-id="0477a-324">exemptedAppProtocols</span></span>|<span data-ttu-id="0477a-325">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0477a-325">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0477a-326">このリストに含まれる iOS アプリはポリシーから除外され、管理対象アプリからデータを受信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="0477a-326">iOS Apps in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="0477a-327">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-327">(iOS Only)</span></span>|
|<span data-ttu-id="0477a-328">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="0477a-328">exemptedAppPackages</span></span>|<span data-ttu-id="0477a-329">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0477a-329">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="0477a-330">このリストの Android アプリパッケージは、ポリシーから除外され、管理対象アプリからデータを受信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="0477a-330">Android App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="0477a-331">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-331">(Android only)</span></span>|
|<span data-ttu-id="0477a-332">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-332">faceIdBlocked</span></span>|<span data-ttu-id="0477a-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="0477a-333">Boolean</span></span>|<span data-ttu-id="0477a-334">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0477a-334">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="0477a-335">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-335">(iOS Only)</span></span>|
|<span data-ttu-id="0477a-336">minimumWipeSdkVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-336">minimumWipeSdkVersion</span></span>|<span data-ttu-id="0477a-337">String</span><span class="sxs-lookup"><span data-stu-id="0477a-337">String</span></span>|<span data-ttu-id="0477a-338">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="0477a-338">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="0477a-339">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="0477a-339">minimumWipePatchVersion</span></span>|<span data-ttu-id="0477a-340">String</span><span class="sxs-lookup"><span data-stu-id="0477a-340">String</span></span>|<span data-ttu-id="0477a-341">指定された値以下の Android セキュリティパッチレベルでは、管理対象アプリと関連会社のデータが消去されます。</span><span class="sxs-lookup"><span data-stu-id="0477a-341">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="0477a-342">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-342">(Android only)</span></span>|
|<span data-ttu-id="0477a-343">allowedIosDeviceModels</span><span class="sxs-lookup"><span data-stu-id="0477a-343">allowedIosDeviceModels</span></span>|<span data-ttu-id="0477a-344">String</span><span class="sxs-lookup"><span data-stu-id="0477a-344">String</span></span>|<span data-ttu-id="0477a-345">管理対象アプリが動作するために、文字列として許可されるデバイスモデルのセミコロンで区切られたリスト。</span><span class="sxs-lookup"><span data-stu-id="0477a-345">Semicolon seperated list of device models allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="0477a-346">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-346">(iOS Only)</span></span>|
|<span data-ttu-id="0477a-347">appActionIfIosDeviceModelNotAllowed</span><span class="sxs-lookup"><span data-stu-id="0477a-347">appActionIfIosDeviceModelNotAllowed</span></span>|[<span data-ttu-id="0477a-348">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="0477a-348">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="0477a-349">指定されたデバイスモデルが許可されていない場合は、ブロックまたはワイプのいずれかの管理対象アプリの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="0477a-349">Defines a managed app behavior, either block or wipe, if the specified device model is not allowed.</span></span> <span data-ttu-id="0477a-350">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="0477a-350">(iOS Only).</span></span> <span data-ttu-id="0477a-351">可能な値は `block`、`wipe`、`warn` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-351">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="0477a-352">allowedandroiddevicemanufacturers、</span><span class="sxs-lookup"><span data-stu-id="0477a-352">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="0477a-353">String</span><span class="sxs-lookup"><span data-stu-id="0477a-353">String</span></span>|<span data-ttu-id="0477a-354">管理対象アプリが動作するために文字列として許可されるデバイスメーカーのセミコロンで区切られたリスト。</span><span class="sxs-lookup"><span data-stu-id="0477a-354">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="0477a-355">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-355">(Android only)</span></span>|
|<span data-ttu-id="0477a-356">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="0477a-356">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="0477a-357">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="0477a-357">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="0477a-358">指定されたデバイスの製造元が許可されていない場合は、ブロックまたはワイプのいずれかの管理対象アプリの動作を定義します。</span><span class="sxs-lookup"><span data-stu-id="0477a-358">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="0477a-359">(Android のみ)。</span><span class="sxs-lookup"><span data-stu-id="0477a-359">(Android only).</span></span> <span data-ttu-id="0477a-360">可能な値は `block`、`wipe`、`warn` です。</span><span class="sxs-lookup"><span data-stu-id="0477a-360">Possible values are: `block`, `wipe`, `warn`.</span></span>|
|<span data-ttu-id="0477a-361">thirdPartyKeyboardsBlocked</span><span class="sxs-lookup"><span data-stu-id="0477a-361">thirdPartyKeyboardsBlocked</span></span>|<span data-ttu-id="0477a-362">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-362">Boolean</span></span>|<span data-ttu-id="0477a-363">管理対象アプリへのアクセス時にサードパーティ製のキーボードを許可するかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="0477a-363">Defines if third party keyboards are allowed while accessing a managed app.</span></span> <span data-ttu-id="0477a-364">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-364">(iOS Only)</span></span>|
|<span data-ttu-id="0477a-365">filterOpenInToOnlyManagedApps</span><span class="sxs-lookup"><span data-stu-id="0477a-365">filterOpenInToOnlyManagedApps</span></span>|<span data-ttu-id="0477a-366">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-366">Boolean</span></span>|<span data-ttu-id="0477a-367">管理対象アプリから、選択された共有ファイルの場所に対してオープンイン操作がサポートされているかどうかを定義します。</span><span class="sxs-lookup"><span data-stu-id="0477a-367">Defines if open-in operation is supported from the managed app to the filesharing locations selected.</span></span> <span data-ttu-id="0477a-368">この設定は、allowedoutbounddatatrans小 DisableProtectionOfManagedOutboundOpenInData が managedapps に設定されていて、が False に設定されている場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="0477a-368">This setting only applies when AllowedOutboundDataTransferDestinations is set to ManagedApps and DisableProtectionOfManagedOutboundOpenInData is set to False.</span></span> <span data-ttu-id="0477a-369">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-369">(iOS Only)</span></span>|
|<span data-ttu-id="0477a-370">disableProtectionOfManagedOutboundOpenInData</span><span class="sxs-lookup"><span data-stu-id="0477a-370">disableProtectionOfManagedOutboundOpenInData</span></span>|<span data-ttu-id="0477a-371">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-371">Boolean</span></span>|<span data-ttu-id="0477a-372">[IOS openin] オプションを使用して、他のアプリに転送されるデータの保護を無効にします。</span><span class="sxs-lookup"><span data-stu-id="0477a-372">Disable protection of data transferred to other apps through IOS OpenIn option.</span></span> <span data-ttu-id="0477a-373">この設定は、allowedoutbounddatatransferdestinations が managedapps に設定されている場合にのみ、True になることができます。</span><span class="sxs-lookup"><span data-stu-id="0477a-373">This setting is only allowed to be True when AllowedOutboundDataTransferDestinations is set to ManagedApps.</span></span> <span data-ttu-id="0477a-374">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-374">(iOS Only)</span></span>|
|<span data-ttu-id="0477a-375">protectInboundDataFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="0477a-375">protectInboundDataFromUnknownSources</span></span>|<span data-ttu-id="0477a-376">ブール値</span><span class="sxs-lookup"><span data-stu-id="0477a-376">Boolean</span></span>|<span data-ttu-id="0477a-377">不明なソースからの受信データを保護します。</span><span class="sxs-lookup"><span data-stu-id="0477a-377">Protect incoming data from unknown source.</span></span> <span data-ttu-id="0477a-378">AllowedInboundDataTransferSources が allapps に設定されている場合にのみ、この設定は True になります。</span><span class="sxs-lookup"><span data-stu-id="0477a-378">This setting is only allowed to be True when AllowedInboundDataTransferSources is set to AllApps.</span></span> <span data-ttu-id="0477a-379">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="0477a-379">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="0477a-380">応答</span><span class="sxs-lookup"><span data-stu-id="0477a-380">Response</span></span>
<span data-ttu-id="0477a-381">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0477a-381">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0477a-382">例</span><span class="sxs-lookup"><span data-stu-id="0477a-382">Example</span></span>

### <a name="request"></a><span data-ttu-id="0477a-383">要求</span><span class="sxs-lookup"><span data-stu-id="0477a-383">Request</span></span>
<span data-ttu-id="0477a-384">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0477a-384">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 3217

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```

### <a name="response"></a><span data-ttu-id="0477a-385">応答</span><span class="sxs-lookup"><span data-stu-id="0477a-385">Response</span></span>
<span data-ttu-id="0477a-p157">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0477a-p157">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 3389

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "id": "77064c51-4c51-7706-514c-0677514c0677",
  "version": "Version value",
  "periodOfflineBeforeAccessCheck": "-PT17.1357909S",
  "periodOnlineBeforeAccessCheck": "PT35.0018757S",
  "allowedInboundDataTransferSources": "managedApps",
  "allowedOutboundDataTransferDestinations": "managedApps",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "managedAppsWithPasteIn",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "-PT3M22.1587532S",
  "pinRequired": true,
  "maximumPinRetries": 1,
  "simplePinBlocked": true,
  "minimumPinLength": 0,
  "pinCharacterSet": "alphanumericAndSymbol",
  "periodBeforePinReset": "PT3M29.6631862S",
  "allowedDataStorageLocations": [
    "sharePoint"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "Minimum Required Os Version value",
  "minimumWarningOsVersion": "Minimum Warning Os Version value",
  "minimumRequiredAppVersion": "Minimum Required App Version value",
  "minimumWarningAppVersion": "Minimum Warning App Version value",
  "minimumWipeOsVersion": "Minimum Wipe Os Version value",
  "minimumWipeAppVersion": "Minimum Wipe App Version value",
  "appActionIfDeviceComplianceRequired": "wipe",
  "appActionIfMaximumPinRetriesExceeded": "wipe",
  "pinRequiredInsteadOfBiometricTimeout": "-PT3M9.8396734S",
  "appDataEncryptionType": "afterDeviceRestart",
  "screenCaptureBlocked": true,
  "encryptAppData": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value",
  "exemptedAppProtocols": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "exemptedAppPackages": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "faceIdBlocked": true,
  "minimumWipeSdkVersion": "Minimum Wipe Sdk Version value",
  "minimumWipePatchVersion": "Minimum Wipe Patch Version value",
  "allowedIosDeviceModels": "Allowed Ios Device Models value",
  "appActionIfIosDeviceModelNotAllowed": "wipe",
  "allowedAndroidDeviceManufacturers": "Allowed Android Device Manufacturers value",
  "appActionIfAndroidDeviceManufacturerNotAllowed": "wipe",
  "thirdPartyKeyboardsBlocked": true,
  "filterOpenInToOnlyManagedApps": true,
  "disableProtectionOfManagedOutboundOpenInData": true,
  "protectInboundDataFromUnknownSources": true
}
```




