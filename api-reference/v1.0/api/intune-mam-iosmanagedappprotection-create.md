---
title: Create iosManagedAppProtection
description: 新しい iosManagedAppProtection オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b753d1e2b41cefd5659c43c779187c8b54b50a1e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30977794"
---
# <a name="create-iosmanagedappprotection"></a><span data-ttu-id="09a52-103">Create iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="09a52-103">Create iosManagedAppProtection</span></span>

> <span data-ttu-id="09a52-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="09a52-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09a52-105">新しい [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="09a52-105">Create a new [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09a52-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="09a52-106">Prerequisites</span></span>
<span data-ttu-id="09a52-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09a52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09a52-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09a52-109">Permission type</span></span>|<span data-ttu-id="09a52-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="09a52-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09a52-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09a52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09a52-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09a52-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="09a52-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09a52-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09a52-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09a52-114">Not supported.</span></span>|
|<span data-ttu-id="09a52-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09a52-115">Application</span></span>|<span data-ttu-id="09a52-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09a52-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09a52-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09a52-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/iosManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="09a52-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09a52-118">Request headers</span></span>
|<span data-ttu-id="09a52-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09a52-119">Header</span></span>|<span data-ttu-id="09a52-120">値</span><span class="sxs-lookup"><span data-stu-id="09a52-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09a52-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09a52-121">Authorization</span></span>|<span data-ttu-id="09a52-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="09a52-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09a52-123">承諾</span><span class="sxs-lookup"><span data-stu-id="09a52-123">Accept</span></span>|<span data-ttu-id="09a52-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09a52-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09a52-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="09a52-125">Request body</span></span>
<span data-ttu-id="09a52-126">要求本文で、iosManagedAppProtection オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="09a52-126">In the request body, supply a JSON representation for the iosManagedAppProtection object.</span></span>

<span data-ttu-id="09a52-127">次の表に、iosManagedAppProtection の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-127">The following table shows the properties that are required when you create the iosManagedAppProtection.</span></span>

|<span data-ttu-id="09a52-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09a52-128">Property</span></span>|<span data-ttu-id="09a52-129">型</span><span class="sxs-lookup"><span data-stu-id="09a52-129">Type</span></span>|<span data-ttu-id="09a52-130">説明</span><span class="sxs-lookup"><span data-stu-id="09a52-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09a52-131">displayName</span><span class="sxs-lookup"><span data-stu-id="09a52-131">displayName</span></span>|<span data-ttu-id="09a52-132">String</span><span class="sxs-lookup"><span data-stu-id="09a52-132">String</span></span>|<span data-ttu-id="09a52-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="09a52-133">Policy display name.</span></span> <span data-ttu-id="09a52-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="09a52-135">description</span><span class="sxs-lookup"><span data-stu-id="09a52-135">description</span></span>|<span data-ttu-id="09a52-136">String</span><span class="sxs-lookup"><span data-stu-id="09a52-136">String</span></span>|<span data-ttu-id="09a52-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="09a52-137">The policy's description.</span></span> <span data-ttu-id="09a52-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="09a52-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="09a52-139">createdDateTime</span></span>|<span data-ttu-id="09a52-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09a52-140">DateTimeOffset</span></span>|<span data-ttu-id="09a52-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="09a52-141">The date and time the policy was created.</span></span> <span data-ttu-id="09a52-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="09a52-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="09a52-143">lastModifiedDateTime</span></span>|<span data-ttu-id="09a52-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="09a52-144">DateTimeOffset</span></span>|<span data-ttu-id="09a52-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="09a52-145">Last time the policy was modified.</span></span> <span data-ttu-id="09a52-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="09a52-147">id</span><span class="sxs-lookup"><span data-stu-id="09a52-147">id</span></span>|<span data-ttu-id="09a52-148">String</span><span class="sxs-lookup"><span data-stu-id="09a52-148">String</span></span>|<span data-ttu-id="09a52-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="09a52-149">Key of the entity.</span></span> <span data-ttu-id="09a52-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="09a52-151">version</span><span class="sxs-lookup"><span data-stu-id="09a52-151">version</span></span>|<span data-ttu-id="09a52-152">String</span><span class="sxs-lookup"><span data-stu-id="09a52-152">String</span></span>|<span data-ttu-id="09a52-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="09a52-153">Version of the entity.</span></span> <span data-ttu-id="09a52-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="09a52-155">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="09a52-155">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="09a52-156">期間</span><span class="sxs-lookup"><span data-stu-id="09a52-156">Duration</span></span>|<span data-ttu-id="09a52-157">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="09a52-157">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="09a52-158">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-158">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-159">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="09a52-159">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="09a52-160">期間</span><span class="sxs-lookup"><span data-stu-id="09a52-160">Duration</span></span>|<span data-ttu-id="09a52-161">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="09a52-161">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="09a52-162">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-162">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-163">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="09a52-163">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="09a52-164">managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="09a52-164">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="09a52-165">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="09a52-165">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="09a52-166">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="09a52-166">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="09a52-167">使用可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="09a52-167">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="09a52-168">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="09a52-168">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="09a52-169">managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="09a52-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="09a52-170">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="09a52-170">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="09a52-171">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="09a52-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="09a52-172">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="09a52-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="09a52-173">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="09a52-173">organizationalCredentialsRequired</span></span>|<span data-ttu-id="09a52-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-174">Boolean</span></span>|<span data-ttu-id="09a52-175">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-175">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="09a52-176">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-177">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="09a52-177">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="09a52-178">managedappクリップボードの sharinglevel</span><span class="sxs-lookup"><span data-stu-id="09a52-178">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="09a52-179">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="09a52-179">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="09a52-180">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="09a52-180">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="09a52-181">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="09a52-181">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="09a52-182">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="09a52-182">dataBackupBlocked</span></span>|<span data-ttu-id="09a52-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-183">Boolean</span></span>|<span data-ttu-id="09a52-184">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-184">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="09a52-185">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-186">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="09a52-186">deviceComplianceRequired</span></span>|<span data-ttu-id="09a52-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-187">Boolean</span></span>|<span data-ttu-id="09a52-188">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-188">Indicates whether device compliance is required.</span></span> <span data-ttu-id="09a52-189">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-189">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-190">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="09a52-190">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="09a52-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-191">Boolean</span></span>|<span data-ttu-id="09a52-192">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-192">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="09a52-193">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-193">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="09a52-194">saveAsBlocked</span></span>|<span data-ttu-id="09a52-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-195">Boolean</span></span>|<span data-ttu-id="09a52-196">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="09a52-197">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="09a52-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="09a52-199">期間</span><span class="sxs-lookup"><span data-stu-id="09a52-199">Duration</span></span>|<span data-ttu-id="09a52-200">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="09a52-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="09a52-201">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="09a52-202">pinRequired</span></span>|<span data-ttu-id="09a52-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-203">Boolean</span></span>|<span data-ttu-id="09a52-204">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="09a52-205">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="09a52-206">maximumPinRetries</span></span>|<span data-ttu-id="09a52-207">Int32</span><span class="sxs-lookup"><span data-stu-id="09a52-207">Int32</span></span>|<span data-ttu-id="09a52-208">管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。</span><span class="sxs-lookup"><span data-stu-id="09a52-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="09a52-209">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="09a52-210">simplePinBlocked</span></span>|<span data-ttu-id="09a52-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-211">Boolean</span></span>|<span data-ttu-id="09a52-212">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="09a52-213">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="09a52-214">minimumPinLength</span></span>|<span data-ttu-id="09a52-215">Int32</span><span class="sxs-lookup"><span data-stu-id="09a52-215">Int32</span></span>|<span data-ttu-id="09a52-216">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="09a52-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="09a52-217">pinCharacterSet</span></span>|[<span data-ttu-id="09a52-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="09a52-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="09a52-219">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="09a52-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="09a52-220">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="09a52-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="09a52-221">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="09a52-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="09a52-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="09a52-222">periodBeforePinReset</span></span>|<span data-ttu-id="09a52-223">Duration</span><span class="sxs-lookup"><span data-stu-id="09a52-223">Duration</span></span>|<span data-ttu-id="09a52-224">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="09a52-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="09a52-225">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="09a52-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="09a52-227">[managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="09a52-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="09a52-228">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="09a52-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="09a52-229">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="09a52-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="09a52-230">使用可能な値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="09a52-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="09a52-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="09a52-231">contactSyncBlocked</span></span>|<span data-ttu-id="09a52-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-232">Boolean</span></span>|<span data-ttu-id="09a52-233">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="09a52-234">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="09a52-235">printBlocked</span></span>|<span data-ttu-id="09a52-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-236">Boolean</span></span>|<span data-ttu-id="09a52-237">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="09a52-238">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="09a52-239">fingerprintBlocked</span></span>|<span data-ttu-id="09a52-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-240">Boolean</span></span>|<span data-ttu-id="09a52-241">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="09a52-242">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="09a52-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="09a52-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-244">Boolean</span></span>|<span data-ttu-id="09a52-245">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="09a52-246">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="09a52-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="09a52-248">String</span><span class="sxs-lookup"><span data-stu-id="09a52-248">String</span></span>|<span data-ttu-id="09a52-249">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="09a52-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="09a52-250">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="09a52-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="09a52-252">String</span><span class="sxs-lookup"><span data-stu-id="09a52-252">String</span></span>|<span data-ttu-id="09a52-253">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="09a52-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="09a52-254">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="09a52-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="09a52-256">String</span><span class="sxs-lookup"><span data-stu-id="09a52-256">String</span></span>|<span data-ttu-id="09a52-257">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="09a52-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="09a52-258">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="09a52-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="09a52-260">String</span><span class="sxs-lookup"><span data-stu-id="09a52-260">String</span></span>|<span data-ttu-id="09a52-261">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="09a52-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="09a52-262">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-263">isAssigned</span><span class="sxs-lookup"><span data-stu-id="09a52-263">isAssigned</span></span>|<span data-ttu-id="09a52-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-264">Boolean</span></span>|<span data-ttu-id="09a52-265">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-265">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="09a52-266">[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09a52-266">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="09a52-267">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="09a52-267">appDataEncryptionType</span></span>|[<span data-ttu-id="09a52-268">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="09a52-268">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="09a52-269">管理対象アプリのデータに使用する暗号化の種類。</span><span class="sxs-lookup"><span data-stu-id="09a52-269">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="09a52-270">可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。</span><span class="sxs-lookup"><span data-stu-id="09a52-270">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="09a52-271">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="09a52-271">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="09a52-272">String</span><span class="sxs-lookup"><span data-stu-id="09a52-272">String</span></span>|<span data-ttu-id="09a52-273">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="09a52-273">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="09a52-274">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="09a52-274">deployedAppCount</span></span>|<span data-ttu-id="09a52-275">Int32</span><span class="sxs-lookup"><span data-stu-id="09a52-275">Int32</span></span>|<span data-ttu-id="09a52-276">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="09a52-276">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="09a52-277">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="09a52-277">faceIdBlocked</span></span>|<span data-ttu-id="09a52-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="09a52-278">Boolean</span></span>|<span data-ttu-id="09a52-279">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="09a52-279">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|



## <a name="response"></a><span data-ttu-id="09a52-280">応答</span><span class="sxs-lookup"><span data-stu-id="09a52-280">Response</span></span>
<span data-ttu-id="09a52-281">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="09a52-281">If successful, this method returns a `201 Created` response code and a [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09a52-282">例</span><span class="sxs-lookup"><span data-stu-id="09a52-282">Example</span></span>

### <a name="request"></a><span data-ttu-id="09a52-283">要求</span><span class="sxs-lookup"><span data-stu-id="09a52-283">Request</span></span>
<span data-ttu-id="09a52-284">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09a52-284">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections
Content-type: application/json
Content-length: 1568

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
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
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="09a52-285">応答</span><span class="sxs-lookup"><span data-stu-id="09a52-285">Response</span></span>
<span data-ttu-id="09a52-p135">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09a52-p135">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1740

{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "5bc789cb-89cb-5bc7-cb89-c75bcb89c75b",
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
  "appDataEncryptionType": "afterDeviceRestart",
  "minimumRequiredSdkVersion": "Minimum Required Sdk Version value",
  "deployedAppCount": 0,
  "faceIdBlocked": true
}
```



