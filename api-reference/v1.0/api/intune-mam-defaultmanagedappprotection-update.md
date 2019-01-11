---
title: Update defaultManagedAppProtection
description: defaultManagedAppProtection オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: df4d6efc83c5975589707b519cdf208ceec1e8d7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864093"
---
# <a name="update-defaultmanagedappprotection"></a><span data-ttu-id="e090f-103">Update defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="e090f-103">Update defaultManagedAppProtection</span></span>

> <span data-ttu-id="e090f-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e090f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e090f-105">[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e090f-105">Update the properties of a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e090f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e090f-106">Prerequisites</span></span>
<span data-ttu-id="e090f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e090f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e090f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e090f-109">Permission type</span></span>|<span data-ttu-id="e090f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e090f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e090f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e090f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e090f-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e090f-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e090f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e090f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e090f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e090f-114">Not supported.</span></span>|
|<span data-ttu-id="e090f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e090f-115">Application</span></span>|<span data-ttu-id="e090f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e090f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e090f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e090f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="e090f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e090f-118">Request headers</span></span>
|<span data-ttu-id="e090f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e090f-119">Header</span></span>|<span data-ttu-id="e090f-120">値</span><span class="sxs-lookup"><span data-stu-id="e090f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e090f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e090f-121">Authorization</span></span>|<span data-ttu-id="e090f-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e090f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e090f-123">Accept</span><span class="sxs-lookup"><span data-stu-id="e090f-123">Accept</span></span>|<span data-ttu-id="e090f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e090f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e090f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="e090f-125">Request body</span></span>
<span data-ttu-id="e090f-126">要求本文において、[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクト用の JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="e090f-126">In the request body, supply a JSON representation for the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

<span data-ttu-id="e090f-127">次の表に、[defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-127">The following table shows the properties that are required when you create the [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md).</span></span>

|<span data-ttu-id="e090f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e090f-128">Property</span></span>|<span data-ttu-id="e090f-129">種類</span><span class="sxs-lookup"><span data-stu-id="e090f-129">Type</span></span>|<span data-ttu-id="e090f-130">説明</span><span class="sxs-lookup"><span data-stu-id="e090f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e090f-131">displayName</span><span class="sxs-lookup"><span data-stu-id="e090f-131">displayName</span></span>|<span data-ttu-id="e090f-132">String</span><span class="sxs-lookup"><span data-stu-id="e090f-132">String</span></span>|<span data-ttu-id="e090f-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="e090f-133">Policy display name.</span></span> <span data-ttu-id="e090f-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e090f-135">説明</span><span class="sxs-lookup"><span data-stu-id="e090f-135">description</span></span>|<span data-ttu-id="e090f-136">String</span><span class="sxs-lookup"><span data-stu-id="e090f-136">String</span></span>|<span data-ttu-id="e090f-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="e090f-137">The policy's description.</span></span> <span data-ttu-id="e090f-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e090f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e090f-139">createdDateTime</span></span>|<span data-ttu-id="e090f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e090f-140">DateTimeOffset</span></span>|<span data-ttu-id="e090f-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e090f-141">The date and time the policy was created.</span></span> <span data-ttu-id="e090f-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e090f-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e090f-143">lastModifiedDateTime</span></span>|<span data-ttu-id="e090f-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e090f-144">DateTimeOffset</span></span>|<span data-ttu-id="e090f-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="e090f-145">Last time the policy was modified.</span></span> <span data-ttu-id="e090f-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e090f-147">id</span><span class="sxs-lookup"><span data-stu-id="e090f-147">id</span></span>|<span data-ttu-id="e090f-148">String</span><span class="sxs-lookup"><span data-stu-id="e090f-148">String</span></span>|<span data-ttu-id="e090f-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e090f-149">Key of the entity.</span></span> <span data-ttu-id="e090f-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e090f-151">version</span><span class="sxs-lookup"><span data-stu-id="e090f-151">version</span></span>|<span data-ttu-id="e090f-152">String</span><span class="sxs-lookup"><span data-stu-id="e090f-152">String</span></span>|<span data-ttu-id="e090f-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e090f-153">Version of the entity.</span></span> <span data-ttu-id="e090f-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e090f-155">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="e090f-155">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="e090f-156">Duration</span><span class="sxs-lookup"><span data-stu-id="e090f-156">Duration</span></span>|<span data-ttu-id="e090f-157">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="e090f-157">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="e090f-158">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-158">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-159">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="e090f-159">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="e090f-160">Duration</span><span class="sxs-lookup"><span data-stu-id="e090f-160">Duration</span></span>|<span data-ttu-id="e090f-161">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="e090f-161">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="e090f-162">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-162">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-163">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="e090f-163">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="e090f-164">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="e090f-164">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="e090f-165">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="e090f-165">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="e090f-166">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-166">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="e090f-167">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="e090f-167">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="e090f-168">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="e090f-168">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="e090f-169">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="e090f-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="e090f-170">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="e090f-170">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="e090f-171">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="e090f-172">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="e090f-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="e090f-173">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="e090f-173">organizationalCredentialsRequired</span></span>|<span data-ttu-id="e090f-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-174">Boolean</span></span>|<span data-ttu-id="e090f-175">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-175">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="e090f-176">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-177">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="e090f-177">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="e090f-178">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="e090f-178">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="e090f-179">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="e090f-179">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="e090f-180">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-180">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="e090f-181">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="e090f-181">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="e090f-182">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="e090f-182">dataBackupBlocked</span></span>|<span data-ttu-id="e090f-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-183">Boolean</span></span>|<span data-ttu-id="e090f-184">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-184">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="e090f-185">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-186">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="e090f-186">deviceComplianceRequired</span></span>|<span data-ttu-id="e090f-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-187">Boolean</span></span>|<span data-ttu-id="e090f-188">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-188">Indicates whether device compliance is required.</span></span> <span data-ttu-id="e090f-189">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-189">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-190">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="e090f-190">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="e090f-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-191">Boolean</span></span>|<span data-ttu-id="e090f-192">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-192">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="e090f-193">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-193">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="e090f-194">saveAsBlocked</span></span>|<span data-ttu-id="e090f-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-195">Boolean</span></span>|<span data-ttu-id="e090f-196">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="e090f-197">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="e090f-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="e090f-199">Duration</span><span class="sxs-lookup"><span data-stu-id="e090f-199">Duration</span></span>|<span data-ttu-id="e090f-200">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="e090f-201">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="e090f-202">pinRequired</span></span>|<span data-ttu-id="e090f-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-203">Boolean</span></span>|<span data-ttu-id="e090f-204">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="e090f-205">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="e090f-206">maximumPinRetries</span></span>|<span data-ttu-id="e090f-207">Int32</span><span class="sxs-lookup"><span data-stu-id="e090f-207">Int32</span></span>|<span data-ttu-id="e090f-208">間違った暗証番号 (pin) の再試行の最大数は、マネージ アプリケーションがブロックされているかどうかが消去する前にしようとします。</span><span class="sxs-lookup"><span data-stu-id="e090f-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="e090f-209">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="e090f-210">simplePinBlocked</span></span>|<span data-ttu-id="e090f-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-211">Boolean</span></span>|<span data-ttu-id="e090f-212">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="e090f-213">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="e090f-214">minimumPinLength</span></span>|<span data-ttu-id="e090f-215">Int32</span><span class="sxs-lookup"><span data-stu-id="e090f-215">Int32</span></span>|<span data-ttu-id="e090f-216">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="e090f-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="e090f-217">pinCharacterSet</span></span>|[<span data-ttu-id="e090f-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="e090f-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="e090f-219">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="e090f-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="e090f-220">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="e090f-221">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="e090f-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="e090f-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="e090f-222">periodBeforePinReset</span></span>|<span data-ttu-id="e090f-223">Duration</span><span class="sxs-lookup"><span data-stu-id="e090f-223">Duration</span></span>|<span data-ttu-id="e090f-224">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e090f-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="e090f-225">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="e090f-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="e090f-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e090f-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="e090f-228">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="e090f-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="e090f-229">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="e090f-230">可能な値は、`oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="e090f-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="e090f-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="e090f-231">contactSyncBlocked</span></span>|<span data-ttu-id="e090f-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-232">Boolean</span></span>|<span data-ttu-id="e090f-233">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="e090f-234">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="e090f-235">printBlocked</span></span>|<span data-ttu-id="e090f-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-236">Boolean</span></span>|<span data-ttu-id="e090f-237">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="e090f-238">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="e090f-239">fingerprintBlocked</span></span>|<span data-ttu-id="e090f-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-240">Boolean</span></span>|<span data-ttu-id="e090f-241">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="e090f-242">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="e090f-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="e090f-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-244">Boolean</span></span>|<span data-ttu-id="e090f-245">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="e090f-246">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="e090f-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="e090f-248">String</span><span class="sxs-lookup"><span data-stu-id="e090f-248">String</span></span>|<span data-ttu-id="e090f-249">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="e090f-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="e090f-250">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="e090f-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="e090f-252">String</span><span class="sxs-lookup"><span data-stu-id="e090f-252">String</span></span>|<span data-ttu-id="e090f-253">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="e090f-254">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="e090f-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="e090f-256">String</span><span class="sxs-lookup"><span data-stu-id="e090f-256">String</span></span>|<span data-ttu-id="e090f-257">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="e090f-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="e090f-258">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="e090f-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="e090f-260">String</span><span class="sxs-lookup"><span data-stu-id="e090f-260">String</span></span>|<span data-ttu-id="e090f-261">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="e090f-262">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e090f-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="e090f-263">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="e090f-263">appDataEncryptionType</span></span>|[<span data-ttu-id="e090f-264">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="e090f-264">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="e090f-265">管理対象アプリのデータに使用する暗号化の種類。</span><span class="sxs-lookup"><span data-stu-id="e090f-265">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="e090f-266">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="e090f-266">(iOS Only).</span></span> <span data-ttu-id="e090f-267">可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。</span><span class="sxs-lookup"><span data-stu-id="e090f-267">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="e090f-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e090f-268">screenCaptureBlocked</span></span>|<span data-ttu-id="e090f-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-269">Boolean</span></span>|<span data-ttu-id="e090f-270">画面キャプチャがブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-270">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="e090f-271">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="e090f-271">(Android only)</span></span>|
|<span data-ttu-id="e090f-272">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="e090f-272">encryptAppData</span></span>|<span data-ttu-id="e090f-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-273">Boolean</span></span>|<span data-ttu-id="e090f-274">管理対象アプリのデータを暗号化するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-274">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="e090f-275">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="e090f-275">(Android only)</span></span>|
|<span data-ttu-id="e090f-276">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="e090f-276">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="e090f-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-277">Boolean</span></span>|<span data-ttu-id="e090f-278">この設定を有効にすると、デバイス レベルの暗号化が有効になっている場合、アプリケーション レベルの暗号化が無効です。</span><span class="sxs-lookup"><span data-stu-id="e090f-278">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="e090f-279">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="e090f-279">(Android only)</span></span>|
|<span data-ttu-id="e090f-280">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="e090f-280">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="e090f-281">String</span><span class="sxs-lookup"><span data-stu-id="e090f-281">String</span></span>|<span data-ttu-id="e090f-282">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="e090f-282">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="e090f-283">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="e090f-283">(iOS Only)</span></span>|
|<span data-ttu-id="e090f-284">customSettings</span><span class="sxs-lookup"><span data-stu-id="e090f-284">customSettings</span></span>|<span data-ttu-id="e090f-285">[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e090f-285">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e090f-286">このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="e090f-286">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="e090f-287">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="e090f-287">deployedAppCount</span></span>|<span data-ttu-id="e090f-288">Int32</span><span class="sxs-lookup"><span data-stu-id="e090f-288">Int32</span></span>|<span data-ttu-id="e090f-289">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="e090f-289">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="e090f-290">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="e090f-290">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="e090f-291">String</span><span class="sxs-lookup"><span data-stu-id="e090f-291">String</span></span>|<span data-ttu-id="e090f-292">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="e090f-292">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="e090f-293">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="e090f-293">(Android only)</span></span>|
|<span data-ttu-id="e090f-294">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="e090f-294">minimumWarningPatchVersion</span></span>|<span data-ttu-id="e090f-295">String</span><span class="sxs-lookup"><span data-stu-id="e090f-295">String</span></span>|<span data-ttu-id="e090f-296">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="e090f-296">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="e090f-297">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="e090f-297">(Android only)</span></span>|
|<span data-ttu-id="e090f-298">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="e090f-298">faceIdBlocked</span></span>|<span data-ttu-id="e090f-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="e090f-299">Boolean</span></span>|<span data-ttu-id="e090f-300">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e090f-300">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="e090f-301">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="e090f-301">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="e090f-302">応答</span><span class="sxs-lookup"><span data-stu-id="e090f-302">Response</span></span>
<span data-ttu-id="e090f-303">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e090f-303">If successful, this method returns a `200 OK` response code and an updated [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e090f-304">例</span><span class="sxs-lookup"><span data-stu-id="e090f-304">Example</span></span>
### <a name="request"></a><span data-ttu-id="e090f-305">要求</span><span class="sxs-lookup"><span data-stu-id="e090f-305">Request</span></span>
<span data-ttu-id="e090f-306">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e090f-306">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}
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

### <a name="response"></a><span data-ttu-id="e090f-307">応答</span><span class="sxs-lookup"><span data-stu-id="e090f-307">Response</span></span>
<span data-ttu-id="e090f-p141">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e090f-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



