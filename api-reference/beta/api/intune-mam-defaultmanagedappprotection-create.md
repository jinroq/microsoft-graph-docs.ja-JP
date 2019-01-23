---
title: Create defaultManagedAppProtection
description: 新しい defaultManagedAppProtection オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aebce79a25fa7ca166e563c51db706a62cc23a8f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403323"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="4c2a1-103">Create defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="4c2a1-103">Create defaultManagedAppProtection</span></span>

> <span data-ttu-id="4c2a1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4c2a1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c2a1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c2a1-107">新しい [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-107">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c2a1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c2a1-108">Prerequisites</span></span>
<span data-ttu-id="4c2a1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4c2a1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c2a1-111">Permission type</span></span>|<span data-ttu-id="4c2a1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c2a1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c2a1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c2a1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c2a1-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c2a1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-116">Not supported.</span></span>|
|<span data-ttu-id="4c2a1-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c2a1-117">Application</span></span>|<span data-ttu-id="4c2a1-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c2a1-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c2a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="4c2a1-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c2a1-120">Request headers</span></span>
|<span data-ttu-id="4c2a1-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c2a1-121">Header</span></span>|<span data-ttu-id="4c2a1-122">値</span><span class="sxs-lookup"><span data-stu-id="4c2a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c2a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c2a1-123">Authorization</span></span>|<span data-ttu-id="4c2a1-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c2a1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4c2a1-125">Accept</span></span>|<span data-ttu-id="4c2a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c2a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c2a1-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c2a1-127">Request body</span></span>
<span data-ttu-id="4c2a1-128">要求本文において、defaultManagedAppProtection オブジェクト用の JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-128">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="4c2a1-129">次の表に、defaultManagedAppProtection 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-129">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="4c2a1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c2a1-130">Property</span></span>|<span data-ttu-id="4c2a1-131">型</span><span class="sxs-lookup"><span data-stu-id="4c2a1-131">Type</span></span>|<span data-ttu-id="4c2a1-132">説明</span><span class="sxs-lookup"><span data-stu-id="4c2a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c2a1-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4c2a1-133">displayName</span></span>|<span data-ttu-id="4c2a1-134">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-134">String</span></span>|<span data-ttu-id="4c2a1-135">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-135">Policy display name.</span></span> <span data-ttu-id="4c2a1-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c2a1-137">説明</span><span class="sxs-lookup"><span data-stu-id="4c2a1-137">description</span></span>|<span data-ttu-id="4c2a1-138">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-138">String</span></span>|<span data-ttu-id="4c2a1-139">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-139">The policy's description.</span></span> <span data-ttu-id="4c2a1-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c2a1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c2a1-141">createdDateTime</span></span>|<span data-ttu-id="4c2a1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c2a1-142">DateTimeOffset</span></span>|<span data-ttu-id="4c2a1-143">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-143">The date and time the policy was created.</span></span> <span data-ttu-id="4c2a1-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c2a1-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c2a1-145">lastModifiedDateTime</span></span>|<span data-ttu-id="4c2a1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c2a1-146">DateTimeOffset</span></span>|<span data-ttu-id="4c2a1-147">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-147">Last time the policy was modified.</span></span> <span data-ttu-id="4c2a1-148">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-148">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c2a1-149">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4c2a1-149">roleScopeTagIds</span></span>|<span data-ttu-id="4c2a1-150">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4c2a1-150">String collection</span></span>|<span data-ttu-id="4c2a1-151">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-151">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4c2a1-152">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-152">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c2a1-153">id</span><span class="sxs-lookup"><span data-stu-id="4c2a1-153">id</span></span>|<span data-ttu-id="4c2a1-154">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-154">String</span></span>|<span data-ttu-id="4c2a1-155">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-155">Key of the entity.</span></span> <span data-ttu-id="4c2a1-156">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-156">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c2a1-157">version</span><span class="sxs-lookup"><span data-stu-id="4c2a1-157">version</span></span>|<span data-ttu-id="4c2a1-158">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-158">String</span></span>|<span data-ttu-id="4c2a1-159">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-159">Version of the entity.</span></span> <span data-ttu-id="4c2a1-160">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-160">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="4c2a1-161">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="4c2a1-161">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="4c2a1-162">Duration</span><span class="sxs-lookup"><span data-stu-id="4c2a1-162">Duration</span></span>|<span data-ttu-id="4c2a1-163">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-163">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="4c2a1-164">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-164">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-165">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="4c2a1-165">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="4c2a1-166">Duration</span><span class="sxs-lookup"><span data-stu-id="4c2a1-166">Duration</span></span>|<span data-ttu-id="4c2a1-167">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-167">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="4c2a1-168">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-168">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-169">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="4c2a1-169">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="4c2a1-170">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="4c2a1-170">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="4c2a1-171">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-171">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="4c2a1-172">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-172">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="4c2a1-173">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-173">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="4c2a1-174">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="4c2a1-174">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="4c2a1-175">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="4c2a1-175">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="4c2a1-176">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-176">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="4c2a1-177">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-177">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="4c2a1-178">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-178">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="4c2a1-179">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="4c2a1-179">organizationalCredentialsRequired</span></span>|<span data-ttu-id="4c2a1-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-180">Boolean</span></span>|<span data-ttu-id="4c2a1-181">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-181">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="4c2a1-182">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-182">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-183">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="4c2a1-183">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="4c2a1-184">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="4c2a1-184">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="4c2a1-185">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-185">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="4c2a1-186">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-186">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="4c2a1-187">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-187">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="4c2a1-188">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-188">dataBackupBlocked</span></span>|<span data-ttu-id="4c2a1-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-189">Boolean</span></span>|<span data-ttu-id="4c2a1-190">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-190">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="4c2a1-191">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-191">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-192">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="4c2a1-192">deviceComplianceRequired</span></span>|<span data-ttu-id="4c2a1-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-193">Boolean</span></span>|<span data-ttu-id="4c2a1-194">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-194">Indicates whether device compliance is required.</span></span> <span data-ttu-id="4c2a1-195">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-195">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-196">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="4c2a1-196">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="4c2a1-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-197">Boolean</span></span>|<span data-ttu-id="4c2a1-198">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-198">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="4c2a1-199">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-199">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-200">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-200">saveAsBlocked</span></span>|<span data-ttu-id="4c2a1-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-201">Boolean</span></span>|<span data-ttu-id="4c2a1-202">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-202">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="4c2a1-203">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-203">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-204">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="4c2a1-204">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="4c2a1-205">Duration</span><span class="sxs-lookup"><span data-stu-id="4c2a1-205">Duration</span></span>|<span data-ttu-id="4c2a1-206">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-206">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="4c2a1-207">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-207">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-208">pinRequired</span><span class="sxs-lookup"><span data-stu-id="4c2a1-208">pinRequired</span></span>|<span data-ttu-id="4c2a1-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-209">Boolean</span></span>|<span data-ttu-id="4c2a1-210">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-210">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="4c2a1-211">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-211">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-212">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="4c2a1-212">maximumPinRetries</span></span>|<span data-ttu-id="4c2a1-213">Int32</span><span class="sxs-lookup"><span data-stu-id="4c2a1-213">Int32</span></span>|<span data-ttu-id="4c2a1-214">間違った暗証番号 (pin) の再試行の最大数は、マネージ アプリケーションがブロックされているかどうかが消去する前にしようとします。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-214">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="4c2a1-215">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-215">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-216">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-216">simplePinBlocked</span></span>|<span data-ttu-id="4c2a1-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-217">Boolean</span></span>|<span data-ttu-id="4c2a1-218">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-218">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="4c2a1-219">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-219">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-220">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="4c2a1-220">minimumPinLength</span></span>|<span data-ttu-id="4c2a1-221">Int32</span><span class="sxs-lookup"><span data-stu-id="4c2a1-221">Int32</span></span>|<span data-ttu-id="4c2a1-222">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-222">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-223">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="4c2a1-223">pinCharacterSet</span></span>|[<span data-ttu-id="4c2a1-224">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="4c2a1-224">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="4c2a1-225">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-225">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="4c2a1-226">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-226">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="4c2a1-227">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-227">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="4c2a1-228">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="4c2a1-228">periodBeforePinReset</span></span>|<span data-ttu-id="4c2a1-229">Duration</span><span class="sxs-lookup"><span data-stu-id="4c2a1-229">Duration</span></span>|<span data-ttu-id="4c2a1-230">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-230">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="4c2a1-231">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-231">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-232">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="4c2a1-232">allowedDataStorageLocations</span></span>|<span data-ttu-id="4c2a1-233">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c2a1-233">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="4c2a1-234">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-234">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="4c2a1-235">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-235">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="4c2a1-236">可能な値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-236">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="4c2a1-237">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-237">contactSyncBlocked</span></span>|<span data-ttu-id="4c2a1-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-238">Boolean</span></span>|<span data-ttu-id="4c2a1-239">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-239">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="4c2a1-240">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-240">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-241">printBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-241">printBlocked</span></span>|<span data-ttu-id="4c2a1-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-242">Boolean</span></span>|<span data-ttu-id="4c2a1-243">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-243">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="4c2a1-244">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-244">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-245">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-245">fingerprintBlocked</span></span>|<span data-ttu-id="4c2a1-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-246">Boolean</span></span>|<span data-ttu-id="4c2a1-247">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-247">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="4c2a1-248">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-248">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-249">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="4c2a1-249">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="4c2a1-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-250">Boolean</span></span>|<span data-ttu-id="4c2a1-251">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-251">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="4c2a1-252">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-252">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-253">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-253">minimumRequiredOsVersion</span></span>|<span data-ttu-id="4c2a1-254">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-254">String</span></span>|<span data-ttu-id="4c2a1-255">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-255">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="4c2a1-256">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-256">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-257">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-257">minimumWarningOsVersion</span></span>|<span data-ttu-id="4c2a1-258">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-258">String</span></span>|<span data-ttu-id="4c2a1-259">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-259">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="4c2a1-260">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-260">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-261">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-261">minimumRequiredAppVersion</span></span>|<span data-ttu-id="4c2a1-262">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-262">String</span></span>|<span data-ttu-id="4c2a1-263">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-263">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="4c2a1-264">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-264">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-265">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-265">minimumWarningAppVersion</span></span>|<span data-ttu-id="4c2a1-266">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-266">String</span></span>|<span data-ttu-id="4c2a1-267">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-267">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="4c2a1-268">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-268">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-269">minimumWipeOsVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-269">minimumWipeOsVersion</span></span>|<span data-ttu-id="4c2a1-270">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-270">String</span></span>|<span data-ttu-id="4c2a1-271">マネージ アプリケーションと関連付けられている会社のデータを消去は指定されたバージョン以下のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-271">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="4c2a1-272">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-272">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-273">minimumWipeAppVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-273">minimumWipeAppVersion</span></span>|<span data-ttu-id="4c2a1-274">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-274">String</span></span>|<span data-ttu-id="4c2a1-275">マネージ アプリケーションと関連付けられている会社のデータを消去は指定されたバージョン以下のバージョンです。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-275">Versions less than or equal to the specified version will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="4c2a1-276">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4c2a1-276">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-277">appActionIfDeviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="4c2a1-277">appActionIfDeviceComplianceRequired</span></span>|[<span data-ttu-id="4c2a1-278">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="4c2a1-278">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="4c2a1-279">、マネージ アプリケーションの動作を定義するブロックまたはワイプ、デバイスのルートとなるか、とか、jailbroken、DeviceComplianceRequired が設定されている場合 true に設定します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-279">Defines a managed app behavior, either block or wipe, when the device is either rooted or jailbroken, if DeviceComplianceRequired is set to true.</span></span> <span data-ttu-id="4c2a1-280">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-280">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="4c2a1-281">使用可能な値は、`block`、`wipe` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-281">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="4c2a1-282">appActionIfMaximumPinRetriesExceeded</span><span class="sxs-lookup"><span data-stu-id="4c2a1-282">appActionIfMaximumPinRetriesExceeded</span></span>|[<span data-ttu-id="4c2a1-283">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="4c2a1-283">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="4c2a1-284">マネージ アプリケーションの動作では、いずれかのブロックを定義またはワイプ、不正な pin の再試行回数の最大数に基づいています。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-284">Defines a managed app behavior, either block or wipe, based on maximum number of incorrect pin retry attempts.</span></span> <span data-ttu-id="4c2a1-285">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-285">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="4c2a1-286">使用可能な値は、`block`、`wipe` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-286">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="4c2a1-287">pinRequiredInsteadOfBiometricTimeout</span><span class="sxs-lookup"><span data-stu-id="4c2a1-287">pinRequiredInsteadOfBiometricTimeout</span></span>|<span data-ttu-id="4c2a1-288">Duration</span><span class="sxs-lookup"><span data-stu-id="4c2a1-288">Duration</span></span>|<span data-ttu-id="4c2a1-289">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から非生体認証パスコード継承ではなく、アプリのピンを分単位でタイムアウト</span><span class="sxs-lookup"><span data-stu-id="4c2a1-289">Timeout in minutes for an app pin instead of non biometrics passcode Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="4c2a1-290">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="4c2a1-290">appDataEncryptionType</span></span>|[<span data-ttu-id="4c2a1-291">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="4c2a1-291">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="4c2a1-292">管理対象アプリのデータに使用する暗号化の種類。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-292">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="4c2a1-293">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-293">(iOS Only).</span></span> <span data-ttu-id="4c2a1-294">可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-294">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="4c2a1-295">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-295">screenCaptureBlocked</span></span>|<span data-ttu-id="4c2a1-296">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-296">Boolean</span></span>|<span data-ttu-id="4c2a1-297">画面キャプチャがブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-297">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="4c2a1-298">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-298">(Android only)</span></span>|
|<span data-ttu-id="4c2a1-299">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="4c2a1-299">encryptAppData</span></span>|<span data-ttu-id="4c2a1-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-300">Boolean</span></span>|<span data-ttu-id="4c2a1-301">管理対象アプリのデータを暗号化するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-301">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="4c2a1-302">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-302">(Android only)</span></span>|
|<span data-ttu-id="4c2a1-303">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="4c2a1-303">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="4c2a1-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-304">Boolean</span></span>|<span data-ttu-id="4c2a1-305">この設定を有効にすると、デバイス レベルの暗号化が有効になっている場合、アプリケーション レベルの暗号化が無効です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-305">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="4c2a1-306">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-306">(Android only)</span></span>|
|<span data-ttu-id="4c2a1-307">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-307">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="4c2a1-308">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-308">String</span></span>|<span data-ttu-id="4c2a1-309">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-309">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="4c2a1-310">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-310">(iOS Only)</span></span>|
|<span data-ttu-id="4c2a1-311">customSettings</span><span class="sxs-lookup"><span data-stu-id="4c2a1-311">customSettings</span></span>|<span data-ttu-id="4c2a1-312">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c2a1-312">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4c2a1-313">このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="4c2a1-313">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="4c2a1-314">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="4c2a1-314">deployedAppCount</span></span>|<span data-ttu-id="4c2a1-315">Int32</span><span class="sxs-lookup"><span data-stu-id="4c2a1-315">Int32</span></span>|<span data-ttu-id="4c2a1-316">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-316">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="4c2a1-317">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-317">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="4c2a1-318">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-318">String</span></span>|<span data-ttu-id="4c2a1-319">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-319">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="4c2a1-320">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-320">(Android only)</span></span>|
|<span data-ttu-id="4c2a1-321">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-321">minimumWarningPatchVersion</span></span>|<span data-ttu-id="4c2a1-322">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-322">String</span></span>|<span data-ttu-id="4c2a1-323">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-323">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="4c2a1-324">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-324">(Android only)</span></span>|
|<span data-ttu-id="4c2a1-325">exemptedAppProtocols</span><span class="sxs-lookup"><span data-stu-id="4c2a1-325">exemptedAppProtocols</span></span>|<span data-ttu-id="4c2a1-326">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c2a1-326">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4c2a1-327">iOS アプリをこのリストには、ポリシーの対象外になります、マネージ アプリケーションからデータを受信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-327">iOS Apps in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="4c2a1-328">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-328">(iOS Only)</span></span>|
|<span data-ttu-id="4c2a1-329">exemptedAppPackages</span><span class="sxs-lookup"><span data-stu-id="4c2a1-329">exemptedAppPackages</span></span>|<span data-ttu-id="4c2a1-330">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4c2a1-330">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="4c2a1-331">このリスト内の android のアプリケーション パッケージは、ポリシーの対象外になり、マネージ アプリケーションからデータを受信できるようになります。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-331">Android App packages in this list will be exempt from the policy and will be able to receive data from managed apps.</span></span> <span data-ttu-id="4c2a1-332">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-332">(Android only)</span></span>|
|<span data-ttu-id="4c2a1-333">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-333">faceIdBlocked</span></span>|<span data-ttu-id="4c2a1-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-334">Boolean</span></span>|<span data-ttu-id="4c2a1-335">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-335">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="4c2a1-336">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-336">(iOS Only)</span></span>|
|<span data-ttu-id="4c2a1-337">minimumWipeSdkVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-337">minimumWipeSdkVersion</span></span>|<span data-ttu-id="4c2a1-338">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-338">String</span></span>|<span data-ttu-id="4c2a1-339">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-339">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="4c2a1-340">minimumWipePatchVersion</span><span class="sxs-lookup"><span data-stu-id="4c2a1-340">minimumWipePatchVersion</span></span>|<span data-ttu-id="4c2a1-341">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-341">String</span></span>|<span data-ttu-id="4c2a1-342">Android のセキュリティ修正プログラムのレベル以下または指定した値に等しいは、マネージ アプリケーションと関連付けられている会社のデータに拭きます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-342">Android security patch level  less than or equal to the specified value will wipe the managed app and the associated company data.</span></span> <span data-ttu-id="4c2a1-343">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-343">(Android only)</span></span>|
|<span data-ttu-id="4c2a1-344">allowedIosDeviceModels</span><span class="sxs-lookup"><span data-stu-id="4c2a1-344">allowedIosDeviceModels</span></span>|<span data-ttu-id="4c2a1-345">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-345">String</span></span>|<span data-ttu-id="4c2a1-346">デバイス モデルのセミコロン区切りのリストは、動作するマネージ アプリケーションの文字列として使用できます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-346">Semicolon seperated list of device models allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="4c2a1-347">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-347">(iOS Only)</span></span>|
|<span data-ttu-id="4c2a1-348">appActionIfIosDeviceModelNotAllowed</span><span class="sxs-lookup"><span data-stu-id="4c2a1-348">appActionIfIosDeviceModelNotAllowed</span></span>|[<span data-ttu-id="4c2a1-349">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="4c2a1-349">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="4c2a1-350">、マネージ アプリケーションの動作を定義するブロック] または [指定したデバイスのモデルが許可されていない場合、クリーン インストールします。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-350">Defines a managed app behavior, either block or wipe, if the specified device model is not allowed.</span></span> <span data-ttu-id="4c2a1-351">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-351">(iOS Only).</span></span> <span data-ttu-id="4c2a1-352">使用可能な値は、`block`、`wipe` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-352">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="4c2a1-353">allowedAndroidDeviceManufacturers</span><span class="sxs-lookup"><span data-stu-id="4c2a1-353">allowedAndroidDeviceManufacturers</span></span>|<span data-ttu-id="4c2a1-354">String</span><span class="sxs-lookup"><span data-stu-id="4c2a1-354">String</span></span>|<span data-ttu-id="4c2a1-355">デバイスの製造元のセミコロン区切りのリストは、動作するマネージ アプリケーションの文字列として使用できます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-355">Semicolon seperated list of device manufacturers allowed, as a string, for the managed app to work.</span></span> <span data-ttu-id="4c2a1-356">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-356">(Android only)</span></span>|
|<span data-ttu-id="4c2a1-357">appActionIfAndroidDeviceManufacturerNotAllowed</span><span class="sxs-lookup"><span data-stu-id="4c2a1-357">appActionIfAndroidDeviceManufacturerNotAllowed</span></span>|[<span data-ttu-id="4c2a1-358">managedAppRemediationAction</span><span class="sxs-lookup"><span data-stu-id="4c2a1-358">managedAppRemediationAction</span></span>](../resources/intune-mam-managedappremediationaction.md)|<span data-ttu-id="4c2a1-359">、マネージ アプリケーションの動作を定義するブロックまたは指定されたデバイスの製造元が許可されていない場合、クリーン インストールのいずれかです。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-359">Defines a managed app behavior, either block or wipe, if the specified device manufacturer is not allowed.</span></span> <span data-ttu-id="4c2a1-360">(アプリのみ)。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-360">(Android only).</span></span> <span data-ttu-id="4c2a1-361">使用可能な値は、`block`、`wipe` です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-361">Possible values are: `block`, `wipe`.</span></span>|
|<span data-ttu-id="4c2a1-362">thirdPartyKeyboardsBlocked</span><span class="sxs-lookup"><span data-stu-id="4c2a1-362">thirdPartyKeyboardsBlocked</span></span>|<span data-ttu-id="4c2a1-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-363">Boolean</span></span>|<span data-ttu-id="4c2a1-364">サードパーティ製キーボードが管理されているアプリケーションへのアクセス中に許可されている場合を定義します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-364">Defines if third party keyboards are allowed while accessing a managed app.</span></span> <span data-ttu-id="4c2a1-365">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-365">(iOS Only)</span></span>|
|<span data-ttu-id="4c2a1-366">filterOpenInToOnlyManagedApps</span><span class="sxs-lookup"><span data-stu-id="4c2a1-366">filterOpenInToOnlyManagedApps</span></span>|<span data-ttu-id="4c2a1-367">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-367">Boolean</span></span>|<span data-ttu-id="4c2a1-368">選択されているファイル共有の場所に、マネージ アプリケーションから開くの操作がサポートされている場合を定義します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-368">Defines if open-in operation is supported from the managed app to the filesharing locations selected.</span></span> <span data-ttu-id="4c2a1-369">この設定は、AllowedOutboundDataTransferDestinations を ManagedApps に設定し、DisableProtectionOfManagedOutboundOpenInData が False に設定されて場合にのみ適用されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-369">This setting only applies when AllowedOutboundDataTransferDestinations is set to ManagedApps and DisableProtectionOfManagedOutboundOpenInData is set to False.</span></span> <span data-ttu-id="4c2a1-370">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-370">(iOS Only)</span></span>|
|<span data-ttu-id="4c2a1-371">disableProtectionOfManagedOutboundOpenInData</span><span class="sxs-lookup"><span data-stu-id="4c2a1-371">disableProtectionOfManagedOutboundOpenInData</span></span>|<span data-ttu-id="4c2a1-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-372">Boolean</span></span>|<span data-ttu-id="4c2a1-373">IOS OpenIn オプションを使用して他のアプリケーションに転送されるデータの保護を無効にします。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-373">Disable protection of data transferred to other apps through IOS OpenIn option.</span></span> <span data-ttu-id="4c2a1-374">この設定はのみできる AllowedOutboundDataTransferDestinations が ManagedApps に設定されている場合に true を設定します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-374">This setting is only allowed to be True when AllowedOutboundDataTransferDestinations is set to ManagedApps.</span></span> <span data-ttu-id="4c2a1-375">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-375">(iOS Only)</span></span>|
|<span data-ttu-id="4c2a1-376">protectInboundDataFromUnknownSources</span><span class="sxs-lookup"><span data-stu-id="4c2a1-376">protectInboundDataFromUnknownSources</span></span>|<span data-ttu-id="4c2a1-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c2a1-377">Boolean</span></span>|<span data-ttu-id="4c2a1-378">不明なソースから受信したデータを保護します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-378">Protect incoming data from unknown source.</span></span> <span data-ttu-id="4c2a1-379">この設定はのみできる AllowedInboundDataTransferSources が AllApps に設定されている場合に true を設定します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-379">This setting is only allowed to be True when AllowedInboundDataTransferSources is set to AllApps.</span></span> <span data-ttu-id="4c2a1-380">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="4c2a1-380">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="4c2a1-381">応答</span><span class="sxs-lookup"><span data-stu-id="4c2a1-381">Response</span></span>
<span data-ttu-id="4c2a1-382">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-382">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c2a1-383">例</span><span class="sxs-lookup"><span data-stu-id="4c2a1-383">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c2a1-384">要求</span><span class="sxs-lookup"><span data-stu-id="4c2a1-384">Request</span></span>
<span data-ttu-id="4c2a1-385">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-385">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4c2a1-386">応答</span><span class="sxs-lookup"><span data-stu-id="4c2a1-386">Response</span></span>
<span data-ttu-id="4c2a1-p158">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c2a1-p158">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




