---
title: Create defaultManagedAppProtection
description: 新しい defaultManagedAppProtection オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 26189aeabe2e89926a0c0f1057c34f7cf30d2d7d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020711"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="02f7e-103">Create defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="02f7e-103">Create defaultManagedAppProtection</span></span>

> <span data-ttu-id="02f7e-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02f7e-105">新しい [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-105">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02f7e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="02f7e-106">Prerequisites</span></span>
<span data-ttu-id="02f7e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02f7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02f7e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02f7e-109">Permission type</span></span>|<span data-ttu-id="02f7e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="02f7e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02f7e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02f7e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="02f7e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="02f7e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="02f7e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02f7e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02f7e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f7e-114">Not supported.</span></span>|
|<span data-ttu-id="02f7e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02f7e-115">Application</span></span>|<span data-ttu-id="02f7e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f7e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02f7e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02f7e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="02f7e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02f7e-118">Request headers</span></span>
|<span data-ttu-id="02f7e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02f7e-119">Header</span></span>|<span data-ttu-id="02f7e-120">値</span><span class="sxs-lookup"><span data-stu-id="02f7e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02f7e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="02f7e-121">Authorization</span></span>|<span data-ttu-id="02f7e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02f7e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="02f7e-123">Accept</span></span>|<span data-ttu-id="02f7e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="02f7e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02f7e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="02f7e-125">Request body</span></span>
<span data-ttu-id="02f7e-126">要求本文において、defaultManagedAppProtection オブジェクト用の JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-126">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="02f7e-127">次の表に、defaultManagedAppProtection 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-127">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="02f7e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02f7e-128">Property</span></span>|<span data-ttu-id="02f7e-129">型</span><span class="sxs-lookup"><span data-stu-id="02f7e-129">Type</span></span>|<span data-ttu-id="02f7e-130">説明</span><span class="sxs-lookup"><span data-stu-id="02f7e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02f7e-131">displayName</span><span class="sxs-lookup"><span data-stu-id="02f7e-131">displayName</span></span>|<span data-ttu-id="02f7e-132">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-132">String</span></span>|<span data-ttu-id="02f7e-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="02f7e-133">Policy display name.</span></span> <span data-ttu-id="02f7e-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="02f7e-135">description</span><span class="sxs-lookup"><span data-stu-id="02f7e-135">description</span></span>|<span data-ttu-id="02f7e-136">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-136">String</span></span>|<span data-ttu-id="02f7e-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="02f7e-137">The policy's description.</span></span> <span data-ttu-id="02f7e-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="02f7e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="02f7e-139">createdDateTime</span></span>|<span data-ttu-id="02f7e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02f7e-140">DateTimeOffset</span></span>|<span data-ttu-id="02f7e-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="02f7e-141">The date and time the policy was created.</span></span> <span data-ttu-id="02f7e-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="02f7e-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="02f7e-143">lastModifiedDateTime</span></span>|<span data-ttu-id="02f7e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="02f7e-144">DateTimeOffset</span></span>|<span data-ttu-id="02f7e-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="02f7e-145">Last time the policy was modified.</span></span> <span data-ttu-id="02f7e-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="02f7e-147">id</span><span class="sxs-lookup"><span data-stu-id="02f7e-147">id</span></span>|<span data-ttu-id="02f7e-148">文字列</span><span class="sxs-lookup"><span data-stu-id="02f7e-148">String</span></span>|<span data-ttu-id="02f7e-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="02f7e-149">Key of the entity.</span></span> <span data-ttu-id="02f7e-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="02f7e-151">version</span><span class="sxs-lookup"><span data-stu-id="02f7e-151">version</span></span>|<span data-ttu-id="02f7e-152">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-152">String</span></span>|<span data-ttu-id="02f7e-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="02f7e-153">Version of the entity.</span></span> <span data-ttu-id="02f7e-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="02f7e-155">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="02f7e-155">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="02f7e-156">期間</span><span class="sxs-lookup"><span data-stu-id="02f7e-156">Duration</span></span>|<span data-ttu-id="02f7e-157">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="02f7e-157">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="02f7e-158">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-158">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-159">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="02f7e-159">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="02f7e-160">期間</span><span class="sxs-lookup"><span data-stu-id="02f7e-160">Duration</span></span>|<span data-ttu-id="02f7e-161">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="02f7e-161">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="02f7e-162">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-162">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-163">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="02f7e-163">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="02f7e-164">Managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="02f7e-164">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="02f7e-165">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="02f7e-165">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="02f7e-166">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-166">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="02f7e-167">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-167">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="02f7e-168">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="02f7e-168">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="02f7e-169">Managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="02f7e-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="02f7e-170">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="02f7e-170">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="02f7e-171">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="02f7e-172">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="02f7e-173">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="02f7e-173">organizationalCredentialsRequired</span></span>|<span data-ttu-id="02f7e-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-174">Boolean</span></span>|<span data-ttu-id="02f7e-175">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-175">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="02f7e-176">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-177">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="02f7e-177">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="02f7e-178">Managedappクリップボードの Sharinglevel</span><span class="sxs-lookup"><span data-stu-id="02f7e-178">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="02f7e-179">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="02f7e-179">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="02f7e-180">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-180">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="02f7e-181">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-181">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="02f7e-182">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="02f7e-182">dataBackupBlocked</span></span>|<span data-ttu-id="02f7e-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-183">Boolean</span></span>|<span data-ttu-id="02f7e-184">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-184">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="02f7e-185">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-186">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="02f7e-186">deviceComplianceRequired</span></span>|<span data-ttu-id="02f7e-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-187">Boolean</span></span>|<span data-ttu-id="02f7e-188">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-188">Indicates whether device compliance is required.</span></span> <span data-ttu-id="02f7e-189">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-189">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-190">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="02f7e-190">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="02f7e-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-191">Boolean</span></span>|<span data-ttu-id="02f7e-192">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-192">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="02f7e-193">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-193">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="02f7e-194">saveAsBlocked</span></span>|<span data-ttu-id="02f7e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-195">Boolean</span></span>|<span data-ttu-id="02f7e-196">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="02f7e-197">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="02f7e-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="02f7e-199">期間</span><span class="sxs-lookup"><span data-stu-id="02f7e-199">Duration</span></span>|<span data-ttu-id="02f7e-200">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="02f7e-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="02f7e-201">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="02f7e-202">pinRequired</span></span>|<span data-ttu-id="02f7e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-203">Boolean</span></span>|<span data-ttu-id="02f7e-204">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="02f7e-205">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="02f7e-206">maximumPinRetries</span></span>|<span data-ttu-id="02f7e-207">Int32</span><span class="sxs-lookup"><span data-stu-id="02f7e-207">Int32</span></span>|<span data-ttu-id="02f7e-208">管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。</span><span class="sxs-lookup"><span data-stu-id="02f7e-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="02f7e-209">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="02f7e-210">simplePinBlocked</span></span>|<span data-ttu-id="02f7e-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-211">Boolean</span></span>|<span data-ttu-id="02f7e-212">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="02f7e-213">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="02f7e-214">minimumPinLength</span></span>|<span data-ttu-id="02f7e-215">Int32</span><span class="sxs-lookup"><span data-stu-id="02f7e-215">Int32</span></span>|<span data-ttu-id="02f7e-216">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="02f7e-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="02f7e-217">pinCharacterSet</span></span>|[<span data-ttu-id="02f7e-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="02f7e-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="02f7e-219">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="02f7e-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="02f7e-220">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="02f7e-221">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="02f7e-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="02f7e-222">periodBeforePinReset</span></span>|<span data-ttu-id="02f7e-223">Duration</span><span class="sxs-lookup"><span data-stu-id="02f7e-223">Duration</span></span>|<span data-ttu-id="02f7e-224">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="02f7e-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="02f7e-225">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="02f7e-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="02f7e-227">[Managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="02f7e-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="02f7e-228">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="02f7e-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="02f7e-229">[Managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="02f7e-230">可能な値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="02f7e-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="02f7e-231">contactSyncBlocked</span></span>|<span data-ttu-id="02f7e-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-232">Boolean</span></span>|<span data-ttu-id="02f7e-233">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="02f7e-234">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="02f7e-235">printBlocked</span></span>|<span data-ttu-id="02f7e-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-236">Boolean</span></span>|<span data-ttu-id="02f7e-237">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="02f7e-238">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="02f7e-239">fingerprintBlocked</span></span>|<span data-ttu-id="02f7e-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-240">Boolean</span></span>|<span data-ttu-id="02f7e-241">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="02f7e-242">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="02f7e-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="02f7e-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-244">Boolean</span></span>|<span data-ttu-id="02f7e-245">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="02f7e-246">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="02f7e-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="02f7e-248">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-248">String</span></span>|<span data-ttu-id="02f7e-249">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="02f7e-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="02f7e-250">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="02f7e-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="02f7e-252">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-252">String</span></span>|<span data-ttu-id="02f7e-253">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="02f7e-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="02f7e-254">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="02f7e-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="02f7e-256">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-256">String</span></span>|<span data-ttu-id="02f7e-257">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="02f7e-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="02f7e-258">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="02f7e-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="02f7e-260">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-260">String</span></span>|<span data-ttu-id="02f7e-261">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="02f7e-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="02f7e-262">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="02f7e-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="02f7e-263">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="02f7e-263">appDataEncryptionType</span></span>|[<span data-ttu-id="02f7e-264">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="02f7e-264">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="02f7e-265">管理対象アプリのデータに使用する暗号化の種類。</span><span class="sxs-lookup"><span data-stu-id="02f7e-265">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="02f7e-266">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="02f7e-266">(iOS Only).</span></span> <span data-ttu-id="02f7e-267">使用可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-267">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="02f7e-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="02f7e-268">screenCaptureBlocked</span></span>|<span data-ttu-id="02f7e-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-269">Boolean</span></span>|<span data-ttu-id="02f7e-270">画面キャプチャがブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-270">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="02f7e-271">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="02f7e-271">(Android only)</span></span>|
|<span data-ttu-id="02f7e-272">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="02f7e-272">encryptAppData</span></span>|<span data-ttu-id="02f7e-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-273">Boolean</span></span>|<span data-ttu-id="02f7e-274">管理対象アプリのデータを暗号化するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-274">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="02f7e-275">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="02f7e-275">(Android only)</span></span>|
|<span data-ttu-id="02f7e-276">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="02f7e-276">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="02f7e-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-277">Boolean</span></span>|<span data-ttu-id="02f7e-278">この設定を有効にすると、デバイスレベルの暗号化が有効になっている場合、アプリレベルの暗号化が無効になります。</span><span class="sxs-lookup"><span data-stu-id="02f7e-278">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="02f7e-279">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="02f7e-279">(Android only)</span></span>|
|<span data-ttu-id="02f7e-280">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="02f7e-280">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="02f7e-281">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-281">String</span></span>|<span data-ttu-id="02f7e-282">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="02f7e-282">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="02f7e-283">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="02f7e-283">(iOS Only)</span></span>|
|<span data-ttu-id="02f7e-284">customSettings</span><span class="sxs-lookup"><span data-stu-id="02f7e-284">customSettings</span></span>|<span data-ttu-id="02f7e-285">[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="02f7e-285">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="02f7e-286">このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="02f7e-286">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="02f7e-287">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="02f7e-287">deployedAppCount</span></span>|<span data-ttu-id="02f7e-288">Int32</span><span class="sxs-lookup"><span data-stu-id="02f7e-288">Int32</span></span>|<span data-ttu-id="02f7e-289">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="02f7e-289">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="02f7e-290">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="02f7e-290">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="02f7e-291">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-291">String</span></span>|<span data-ttu-id="02f7e-292">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-292">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="02f7e-293">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="02f7e-293">(Android only)</span></span>|
|<span data-ttu-id="02f7e-294">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="02f7e-294">minimumWarningPatchVersion</span></span>|<span data-ttu-id="02f7e-295">String</span><span class="sxs-lookup"><span data-stu-id="02f7e-295">String</span></span>|<span data-ttu-id="02f7e-296">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-296">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="02f7e-297">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="02f7e-297">(Android only)</span></span>|
|<span data-ttu-id="02f7e-298">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="02f7e-298">faceIdBlocked</span></span>|<span data-ttu-id="02f7e-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="02f7e-299">Boolean</span></span>|<span data-ttu-id="02f7e-300">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-300">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="02f7e-301">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="02f7e-301">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="02f7e-302">応答</span><span class="sxs-lookup"><span data-stu-id="02f7e-302">Response</span></span>
<span data-ttu-id="02f7e-303">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="02f7e-303">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02f7e-304">例</span><span class="sxs-lookup"><span data-stu-id="02f7e-304">Example</span></span>

### <a name="request"></a><span data-ttu-id="02f7e-305">要求</span><span class="sxs-lookup"><span data-stu-id="02f7e-305">Request</span></span>
<span data-ttu-id="02f7e-306">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02f7e-306">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections
Content-type: application/json
Content-length: 1971

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
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
  "faceIdBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="02f7e-307">応答</span><span class="sxs-lookup"><span data-stu-id="02f7e-307">Response</span></span>
<span data-ttu-id="02f7e-p141">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02f7e-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2143

{
  "@odata.type": "#microsoft.graph.defaultManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "faceIdBlocked": true
}
```



