---
title: Create androidManagedAppProtection
description: 新しい androidManagedAppProtection オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f2e1f6bba4401c89b1094697fd334fd2cdb842e5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36018493"
---
# <a name="create-androidmanagedappprotection"></a><span data-ttu-id="ce0e2-103">Create androidManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="ce0e2-103">Create androidManagedAppProtection</span></span>

> <span data-ttu-id="ce0e2-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce0e2-105">新しい [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-105">Create a new [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ce0e2-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ce0e2-106">Prerequisites</span></span>
<span data-ttu-id="ce0e2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ce0e2-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ce0e2-109">Permission type</span></span>|<span data-ttu-id="ce0e2-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ce0e2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ce0e2-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ce0e2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ce0e2-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ce0e2-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ce0e2-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ce0e2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ce0e2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-114">Not supported.</span></span>|
|<span data-ttu-id="ce0e2-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ce0e2-115">Application</span></span>|<span data-ttu-id="ce0e2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ce0e2-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ce0e2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/androidManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="ce0e2-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce0e2-118">Request headers</span></span>
|<span data-ttu-id="ce0e2-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ce0e2-119">Header</span></span>|<span data-ttu-id="ce0e2-120">値</span><span class="sxs-lookup"><span data-stu-id="ce0e2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ce0e2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ce0e2-121">Authorization</span></span>|<span data-ttu-id="ce0e2-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ce0e2-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ce0e2-123">Accept</span></span>|<span data-ttu-id="ce0e2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ce0e2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ce0e2-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ce0e2-125">Request body</span></span>
<span data-ttu-id="ce0e2-126">要求本文で、androidManagedAppProtection オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-126">In the request body, supply a JSON representation for the androidManagedAppProtection object.</span></span>

<span data-ttu-id="ce0e2-127">次の表に、androidManagedAppProtection の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-127">The following table shows the properties that are required when you create the androidManagedAppProtection.</span></span>

|<span data-ttu-id="ce0e2-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce0e2-128">Property</span></span>|<span data-ttu-id="ce0e2-129">型</span><span class="sxs-lookup"><span data-stu-id="ce0e2-129">Type</span></span>|<span data-ttu-id="ce0e2-130">説明</span><span class="sxs-lookup"><span data-stu-id="ce0e2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce0e2-131">displayName</span><span class="sxs-lookup"><span data-stu-id="ce0e2-131">displayName</span></span>|<span data-ttu-id="ce0e2-132">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-132">String</span></span>|<span data-ttu-id="ce0e2-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-133">Policy display name.</span></span> <span data-ttu-id="ce0e2-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ce0e2-135">description</span><span class="sxs-lookup"><span data-stu-id="ce0e2-135">description</span></span>|<span data-ttu-id="ce0e2-136">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-136">String</span></span>|<span data-ttu-id="ce0e2-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-137">The policy's description.</span></span> <span data-ttu-id="ce0e2-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ce0e2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ce0e2-139">createdDateTime</span></span>|<span data-ttu-id="ce0e2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce0e2-140">DateTimeOffset</span></span>|<span data-ttu-id="ce0e2-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-141">The date and time the policy was created.</span></span> <span data-ttu-id="ce0e2-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ce0e2-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ce0e2-143">lastModifiedDateTime</span></span>|<span data-ttu-id="ce0e2-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce0e2-144">DateTimeOffset</span></span>|<span data-ttu-id="ce0e2-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-145">Last time the policy was modified.</span></span> <span data-ttu-id="ce0e2-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ce0e2-147">id</span><span class="sxs-lookup"><span data-stu-id="ce0e2-147">id</span></span>|<span data-ttu-id="ce0e2-148">文字列</span><span class="sxs-lookup"><span data-stu-id="ce0e2-148">String</span></span>|<span data-ttu-id="ce0e2-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-149">Key of the entity.</span></span> <span data-ttu-id="ce0e2-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ce0e2-151">version</span><span class="sxs-lookup"><span data-stu-id="ce0e2-151">version</span></span>|<span data-ttu-id="ce0e2-152">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-152">String</span></span>|<span data-ttu-id="ce0e2-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-153">Version of the entity.</span></span> <span data-ttu-id="ce0e2-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="ce0e2-155">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="ce0e2-155">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="ce0e2-156">期間</span><span class="sxs-lookup"><span data-stu-id="ce0e2-156">Duration</span></span>|<span data-ttu-id="ce0e2-157">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-157">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="ce0e2-158">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-158">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-159">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="ce0e2-159">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="ce0e2-160">期間</span><span class="sxs-lookup"><span data-stu-id="ce0e2-160">Duration</span></span>|<span data-ttu-id="ce0e2-161">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-161">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="ce0e2-162">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-162">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-163">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="ce0e2-163">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="ce0e2-164">Managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="ce0e2-164">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="ce0e2-165">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-165">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="ce0e2-166">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-166">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="ce0e2-167">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-167">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="ce0e2-168">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="ce0e2-168">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="ce0e2-169">Managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="ce0e2-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="ce0e2-170">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-170">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="ce0e2-171">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="ce0e2-172">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="ce0e2-173">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="ce0e2-173">organizationalCredentialsRequired</span></span>|<span data-ttu-id="ce0e2-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-174">Boolean</span></span>|<span data-ttu-id="ce0e2-175">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-175">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="ce0e2-176">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-177">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="ce0e2-177">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="ce0e2-178">Managedappクリップボードの Sharinglevel</span><span class="sxs-lookup"><span data-stu-id="ce0e2-178">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="ce0e2-179">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-179">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="ce0e2-180">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-180">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="ce0e2-181">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-181">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="ce0e2-182">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="ce0e2-182">dataBackupBlocked</span></span>|<span data-ttu-id="ce0e2-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-183">Boolean</span></span>|<span data-ttu-id="ce0e2-184">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-184">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="ce0e2-185">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-186">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="ce0e2-186">deviceComplianceRequired</span></span>|<span data-ttu-id="ce0e2-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-187">Boolean</span></span>|<span data-ttu-id="ce0e2-188">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-188">Indicates whether device compliance is required.</span></span> <span data-ttu-id="ce0e2-189">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-189">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-190">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="ce0e2-190">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="ce0e2-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-191">Boolean</span></span>|<span data-ttu-id="ce0e2-192">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-192">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="ce0e2-193">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-193">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="ce0e2-194">saveAsBlocked</span></span>|<span data-ttu-id="ce0e2-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-195">Boolean</span></span>|<span data-ttu-id="ce0e2-196">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="ce0e2-197">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="ce0e2-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="ce0e2-199">期間</span><span class="sxs-lookup"><span data-stu-id="ce0e2-199">Duration</span></span>|<span data-ttu-id="ce0e2-200">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="ce0e2-201">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="ce0e2-202">pinRequired</span></span>|<span data-ttu-id="ce0e2-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-203">Boolean</span></span>|<span data-ttu-id="ce0e2-204">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="ce0e2-205">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="ce0e2-206">maximumPinRetries</span></span>|<span data-ttu-id="ce0e2-207">Int32</span><span class="sxs-lookup"><span data-stu-id="ce0e2-207">Int32</span></span>|<span data-ttu-id="ce0e2-208">管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="ce0e2-209">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="ce0e2-210">simplePinBlocked</span></span>|<span data-ttu-id="ce0e2-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-211">Boolean</span></span>|<span data-ttu-id="ce0e2-212">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="ce0e2-213">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="ce0e2-214">minimumPinLength</span></span>|<span data-ttu-id="ce0e2-215">Int32</span><span class="sxs-lookup"><span data-stu-id="ce0e2-215">Int32</span></span>|<span data-ttu-id="ce0e2-216">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ce0e2-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="ce0e2-217">pinCharacterSet</span></span>|[<span data-ttu-id="ce0e2-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="ce0e2-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="ce0e2-219">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="ce0e2-220">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="ce0e2-221">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="ce0e2-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="ce0e2-222">periodBeforePinReset</span></span>|<span data-ttu-id="ce0e2-223">Duration</span><span class="sxs-lookup"><span data-stu-id="ce0e2-223">Duration</span></span>|<span data-ttu-id="ce0e2-224">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="ce0e2-225">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="ce0e2-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="ce0e2-227">[Managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ce0e2-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="ce0e2-228">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="ce0e2-229">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="ce0e2-230">可能な値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="ce0e2-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="ce0e2-231">contactSyncBlocked</span></span>|<span data-ttu-id="ce0e2-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-232">Boolean</span></span>|<span data-ttu-id="ce0e2-233">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="ce0e2-234">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="ce0e2-235">printBlocked</span></span>|<span data-ttu-id="ce0e2-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-236">Boolean</span></span>|<span data-ttu-id="ce0e2-237">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="ce0e2-238">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="ce0e2-239">fingerprintBlocked</span></span>|<span data-ttu-id="ce0e2-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-240">Boolean</span></span>|<span data-ttu-id="ce0e2-241">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="ce0e2-242">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="ce0e2-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="ce0e2-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-244">Boolean</span></span>|<span data-ttu-id="ce0e2-245">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="ce0e2-246">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce0e2-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="ce0e2-248">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-248">String</span></span>|<span data-ttu-id="ce0e2-249">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="ce0e2-250">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="ce0e2-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="ce0e2-252">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-252">String</span></span>|<span data-ttu-id="ce0e2-253">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="ce0e2-254">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="ce0e2-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="ce0e2-256">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-256">String</span></span>|<span data-ttu-id="ce0e2-257">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="ce0e2-258">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="ce0e2-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="ce0e2-260">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-260">String</span></span>|<span data-ttu-id="ce0e2-261">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="ce0e2-262">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-263">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ce0e2-263">isAssigned</span></span>|<span data-ttu-id="ce0e2-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-264">Boolean</span></span>|<span data-ttu-id="ce0e2-265">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-265">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="ce0e2-266">[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-266">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="ce0e2-267">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="ce0e2-267">screenCaptureBlocked</span></span>|<span data-ttu-id="ce0e2-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-268">Boolean</span></span>|<span data-ttu-id="ce0e2-269">管理対象ユーザーによる管理対象アプリのスクリーン キャプチャが可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-269">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="ce0e2-270">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="ce0e2-270">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="ce0e2-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-271">Boolean</span></span>|<span data-ttu-id="ce0e2-272">この設定が有効で、デバイス レベルの暗号化が有効な場合、アプリ レベルの暗号化は無効になります</span><span class="sxs-lookup"><span data-stu-id="ce0e2-272">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="ce0e2-273">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="ce0e2-273">encryptAppData</span></span>|<span data-ttu-id="ce0e2-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce0e2-274">Boolean</span></span>|<span data-ttu-id="ce0e2-275">管理対象アプリのアプリケーション データを暗号化する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="ce0e2-275">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="ce0e2-276">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="ce0e2-276">deployedAppCount</span></span>|<span data-ttu-id="ce0e2-277">Int32</span><span class="sxs-lookup"><span data-stu-id="ce0e2-277">Int32</span></span>|<span data-ttu-id="ce0e2-278">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-278">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="ce0e2-279">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="ce0e2-279">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="ce0e2-280">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-280">String</span></span>|<span data-ttu-id="ce0e2-281">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-281">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="ce0e2-282">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="ce0e2-282">minimumWarningPatchVersion</span></span>|<span data-ttu-id="ce0e2-283">String</span><span class="sxs-lookup"><span data-stu-id="ce0e2-283">String</span></span>|<span data-ttu-id="ce0e2-284">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-284">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|



## <a name="response"></a><span data-ttu-id="ce0e2-285">応答</span><span class="sxs-lookup"><span data-stu-id="ce0e2-285">Response</span></span>
<span data-ttu-id="ce0e2-286">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-286">If successful, this method returns a `201 Created` response code and a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ce0e2-287">例</span><span class="sxs-lookup"><span data-stu-id="ce0e2-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="ce0e2-288">要求</span><span class="sxs-lookup"><span data-stu-id="ce0e2-288">Request</span></span>
<span data-ttu-id="ce0e2-289">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-289">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections
Content-type: application/json
Content-length: 1692

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
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
  "isAssigned": true,
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
}
```

### <a name="response"></a><span data-ttu-id="ce0e2-290">応答</span><span class="sxs-lookup"><span data-stu-id="ce0e2-290">Response</span></span>
<span data-ttu-id="ce0e2-p134">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ce0e2-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1864

{
  "@odata.type": "#microsoft.graph.androidManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "cf517ced-7ced-cf51-ed7c-51cfed7c51cf",
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
  "isAssigned": true,
  "screenCaptureBlocked": true,
  "disableAppEncryptionIfDeviceEncryptionIsEnabled": true,
  "encryptAppData": true,
  "deployedAppCount": 0,
  "minimumRequiredPatchVersion": "Minimum Required Patch Version value",
  "minimumWarningPatchVersion": "Minimum Warning Patch Version value"
}
```



