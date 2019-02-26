---
title: >
  androidManagedAppProtection の更新
description: androidManagedAppProtection オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 640b96e7e8f47b8c569dc360a18a4c6ba7dfa202
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254962"
---
# <a name="update-androidmanagedappprotection"></a><span data-ttu-id="975eb-103">androidManagedAppProtection の更新
</span><span class="sxs-lookup"><span data-stu-id="975eb-103">Update androidManagedAppProtection</span></span>

> <span data-ttu-id="975eb-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="975eb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="975eb-105">[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="975eb-105">Update the properties of a [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="975eb-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="975eb-106">Prerequisites</span></span>
<span data-ttu-id="975eb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="975eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="975eb-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="975eb-109">Permission type</span></span>|<span data-ttu-id="975eb-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="975eb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="975eb-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="975eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="975eb-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="975eb-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="975eb-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="975eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="975eb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="975eb-114">Not supported.</span></span>|
|<span data-ttu-id="975eb-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="975eb-115">Application</span></span>|<span data-ttu-id="975eb-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="975eb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="975eb-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="975eb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
```

## <a name="request-headers"></a><span data-ttu-id="975eb-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="975eb-118">Request headers</span></span>
|<span data-ttu-id="975eb-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="975eb-119">Header</span></span>|<span data-ttu-id="975eb-120">値</span><span class="sxs-lookup"><span data-stu-id="975eb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="975eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="975eb-121">Authorization</span></span>|<span data-ttu-id="975eb-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="975eb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="975eb-123">承諾</span><span class="sxs-lookup"><span data-stu-id="975eb-123">Accept</span></span>|<span data-ttu-id="975eb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="975eb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="975eb-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="975eb-125">Request body</span></span>
<span data-ttu-id="975eb-126">要求本文で、[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="975eb-126">In the request body, supply a JSON representation for the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object.</span></span>

<span data-ttu-id="975eb-127">次の表に、[androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-127">The following table shows the properties that are required when you create the [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md).</span></span>

|<span data-ttu-id="975eb-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="975eb-128">Property</span></span>|<span data-ttu-id="975eb-129">型</span><span class="sxs-lookup"><span data-stu-id="975eb-129">Type</span></span>|<span data-ttu-id="975eb-130">説明</span><span class="sxs-lookup"><span data-stu-id="975eb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="975eb-131">displayName</span><span class="sxs-lookup"><span data-stu-id="975eb-131">displayName</span></span>|<span data-ttu-id="975eb-132">String</span><span class="sxs-lookup"><span data-stu-id="975eb-132">String</span></span>|<span data-ttu-id="975eb-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="975eb-133">Policy display name.</span></span> <span data-ttu-id="975eb-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="975eb-135">説明</span><span class="sxs-lookup"><span data-stu-id="975eb-135">description</span></span>|<span data-ttu-id="975eb-136">String</span><span class="sxs-lookup"><span data-stu-id="975eb-136">String</span></span>|<span data-ttu-id="975eb-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="975eb-137">The policy's description.</span></span> <span data-ttu-id="975eb-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="975eb-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="975eb-139">createdDateTime</span></span>|<span data-ttu-id="975eb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="975eb-140">DateTimeOffset</span></span>|<span data-ttu-id="975eb-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="975eb-141">The date and time the policy was created.</span></span> <span data-ttu-id="975eb-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="975eb-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="975eb-143">lastModifiedDateTime</span></span>|<span data-ttu-id="975eb-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="975eb-144">DateTimeOffset</span></span>|<span data-ttu-id="975eb-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="975eb-145">Last time the policy was modified.</span></span> <span data-ttu-id="975eb-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="975eb-147">id</span><span class="sxs-lookup"><span data-stu-id="975eb-147">id</span></span>|<span data-ttu-id="975eb-148">文字列</span><span class="sxs-lookup"><span data-stu-id="975eb-148">String</span></span>|<span data-ttu-id="975eb-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="975eb-149">Key of the entity.</span></span> <span data-ttu-id="975eb-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="975eb-151">version</span><span class="sxs-lookup"><span data-stu-id="975eb-151">version</span></span>|<span data-ttu-id="975eb-152">String</span><span class="sxs-lookup"><span data-stu-id="975eb-152">String</span></span>|<span data-ttu-id="975eb-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="975eb-153">Version of the entity.</span></span> <span data-ttu-id="975eb-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="975eb-155">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="975eb-155">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="975eb-156">Duration</span><span class="sxs-lookup"><span data-stu-id="975eb-156">Duration</span></span>|<span data-ttu-id="975eb-157">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="975eb-157">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="975eb-158">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-158">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-159">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="975eb-159">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="975eb-160">Duration</span><span class="sxs-lookup"><span data-stu-id="975eb-160">Duration</span></span>|<span data-ttu-id="975eb-161">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="975eb-161">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="975eb-162">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-162">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-163">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="975eb-163">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="975eb-164">managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="975eb-164">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="975eb-165">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="975eb-165">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="975eb-166">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="975eb-166">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="975eb-167">可能な値は `allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="975eb-167">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="975eb-168">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="975eb-168">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="975eb-169">managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="975eb-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="975eb-170">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="975eb-170">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="975eb-171">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="975eb-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="975eb-172">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="975eb-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="975eb-173">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="975eb-173">organizationalCredentialsRequired</span></span>|<span data-ttu-id="975eb-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-174">Boolean</span></span>|<span data-ttu-id="975eb-175">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-175">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="975eb-176">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-177">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="975eb-177">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="975eb-178">managedappクリップボードの sharinglevel</span><span class="sxs-lookup"><span data-stu-id="975eb-178">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="975eb-179">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="975eb-179">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="975eb-180">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="975eb-180">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="975eb-181">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="975eb-181">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="975eb-182">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="975eb-182">dataBackupBlocked</span></span>|<span data-ttu-id="975eb-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-183">Boolean</span></span>|<span data-ttu-id="975eb-184">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-184">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="975eb-185">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-186">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="975eb-186">deviceComplianceRequired</span></span>|<span data-ttu-id="975eb-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-187">Boolean</span></span>|<span data-ttu-id="975eb-188">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-188">Indicates whether device compliance is required.</span></span> <span data-ttu-id="975eb-189">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-189">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-190">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="975eb-190">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="975eb-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-191">Boolean</span></span>|<span data-ttu-id="975eb-192">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-192">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="975eb-193">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-193">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="975eb-194">saveAsBlocked</span></span>|<span data-ttu-id="975eb-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-195">Boolean</span></span>|<span data-ttu-id="975eb-196">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="975eb-197">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="975eb-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="975eb-199">Duration</span><span class="sxs-lookup"><span data-stu-id="975eb-199">Duration</span></span>|<span data-ttu-id="975eb-200">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="975eb-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="975eb-201">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="975eb-202">pinRequired</span></span>|<span data-ttu-id="975eb-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-203">Boolean</span></span>|<span data-ttu-id="975eb-204">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="975eb-205">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="975eb-206">maximumPinRetries</span></span>|<span data-ttu-id="975eb-207">Int32</span><span class="sxs-lookup"><span data-stu-id="975eb-207">Int32</span></span>|<span data-ttu-id="975eb-208">管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。</span><span class="sxs-lookup"><span data-stu-id="975eb-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="975eb-209">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="975eb-210">simplePinBlocked</span></span>|<span data-ttu-id="975eb-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-211">Boolean</span></span>|<span data-ttu-id="975eb-212">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="975eb-213">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="975eb-214">minimumPinLength</span></span>|<span data-ttu-id="975eb-215">Int32</span><span class="sxs-lookup"><span data-stu-id="975eb-215">Int32</span></span>|<span data-ttu-id="975eb-216">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="975eb-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="975eb-217">pinCharacterSet</span></span>|[<span data-ttu-id="975eb-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="975eb-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="975eb-219">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="975eb-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="975eb-220">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="975eb-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="975eb-221">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="975eb-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="975eb-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="975eb-222">periodBeforePinReset</span></span>|<span data-ttu-id="975eb-223">Duration</span><span class="sxs-lookup"><span data-stu-id="975eb-223">Duration</span></span>|<span data-ttu-id="975eb-224">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="975eb-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="975eb-225">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="975eb-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="975eb-227">[managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="975eb-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="975eb-228">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="975eb-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="975eb-229">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="975eb-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="975eb-230">可能な値は `oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="975eb-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="975eb-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="975eb-231">contactSyncBlocked</span></span>|<span data-ttu-id="975eb-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-232">Boolean</span></span>|<span data-ttu-id="975eb-233">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="975eb-234">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="975eb-235">printBlocked</span></span>|<span data-ttu-id="975eb-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-236">Boolean</span></span>|<span data-ttu-id="975eb-237">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="975eb-238">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="975eb-239">fingerprintBlocked</span></span>|<span data-ttu-id="975eb-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-240">Boolean</span></span>|<span data-ttu-id="975eb-241">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="975eb-242">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="975eb-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="975eb-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-244">Boolean</span></span>|<span data-ttu-id="975eb-245">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="975eb-246">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="975eb-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="975eb-248">String</span><span class="sxs-lookup"><span data-stu-id="975eb-248">String</span></span>|<span data-ttu-id="975eb-249">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="975eb-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="975eb-250">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="975eb-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="975eb-252">String</span><span class="sxs-lookup"><span data-stu-id="975eb-252">String</span></span>|<span data-ttu-id="975eb-253">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="975eb-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="975eb-254">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="975eb-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="975eb-256">String</span><span class="sxs-lookup"><span data-stu-id="975eb-256">String</span></span>|<span data-ttu-id="975eb-257">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="975eb-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="975eb-258">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="975eb-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="975eb-260">String</span><span class="sxs-lookup"><span data-stu-id="975eb-260">String</span></span>|<span data-ttu-id="975eb-261">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="975eb-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="975eb-262">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-263">isAssigned</span><span class="sxs-lookup"><span data-stu-id="975eb-263">isAssigned</span></span>|<span data-ttu-id="975eb-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-264">Boolean</span></span>|<span data-ttu-id="975eb-265">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-265">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="975eb-266">[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="975eb-266">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="975eb-267">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="975eb-267">screenCaptureBlocked</span></span>|<span data-ttu-id="975eb-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-268">Boolean</span></span>|<span data-ttu-id="975eb-269">管理対象ユーザーによる管理対象アプリのスクリーン キャプチャが可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="975eb-269">Indicates whether a managed user can take screen captures of managed apps</span></span>|
|<span data-ttu-id="975eb-270">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="975eb-270">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="975eb-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-271">Boolean</span></span>|<span data-ttu-id="975eb-272">この設定が有効で、デバイス レベルの暗号化が有効な場合、アプリ レベルの暗号化は無効になります</span><span class="sxs-lookup"><span data-stu-id="975eb-272">When this setting is enabled, app level encryption is disabled if device level encryption is enabled</span></span>|
|<span data-ttu-id="975eb-273">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="975eb-273">encryptAppData</span></span>|<span data-ttu-id="975eb-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="975eb-274">Boolean</span></span>|<span data-ttu-id="975eb-275">管理対象アプリのアプリケーション データを暗号化する必要があるかどうかを示します</span><span class="sxs-lookup"><span data-stu-id="975eb-275">Indicates whether application data for managed apps should be encrypted</span></span>|
|<span data-ttu-id="975eb-276">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="975eb-276">deployedAppCount</span></span>|<span data-ttu-id="975eb-277">Int32</span><span class="sxs-lookup"><span data-stu-id="975eb-277">Int32</span></span>|<span data-ttu-id="975eb-278">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="975eb-278">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="975eb-279">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="975eb-279">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="975eb-280">String</span><span class="sxs-lookup"><span data-stu-id="975eb-280">String</span></span>|<span data-ttu-id="975eb-281">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="975eb-281">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span>|
|<span data-ttu-id="975eb-282">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="975eb-282">minimumWarningPatchVersion</span></span>|<span data-ttu-id="975eb-283">String</span><span class="sxs-lookup"><span data-stu-id="975eb-283">String</span></span>|<span data-ttu-id="975eb-284">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="975eb-284">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span>|



## <a name="response"></a><span data-ttu-id="975eb-285">応答</span><span class="sxs-lookup"><span data-stu-id="975eb-285">Response</span></span>
<span data-ttu-id="975eb-286">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="975eb-286">If successful, this method returns a `200 OK` response code and an updated [androidManagedAppProtection](../resources/intune-mam-androidmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="975eb-287">例</span><span class="sxs-lookup"><span data-stu-id="975eb-287">Example</span></span>

### <a name="request"></a><span data-ttu-id="975eb-288">要求</span><span class="sxs-lookup"><span data-stu-id="975eb-288">Request</span></span>
<span data-ttu-id="975eb-289">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="975eb-289">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}
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

### <a name="response"></a><span data-ttu-id="975eb-290">応答</span><span class="sxs-lookup"><span data-stu-id="975eb-290">Response</span></span>
<span data-ttu-id="975eb-p134">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="975eb-p134">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



