---
title: Create defaultManagedAppProtection
description: 新しい defaultManagedAppProtection オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af3387a59b8890fa75b385e2dcaf8c73d823cf6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580838"
---
# <a name="create-defaultmanagedappprotection"></a><span data-ttu-id="6134b-103">Create defaultManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="6134b-103">Create defaultManagedAppProtection</span></span>

> <span data-ttu-id="6134b-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6134b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6134b-105">新しい [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="6134b-105">Create a new [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6134b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6134b-106">Prerequisites</span></span>
<span data-ttu-id="6134b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6134b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6134b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6134b-109">Permission type</span></span>|<span data-ttu-id="6134b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6134b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6134b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6134b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6134b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6134b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6134b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6134b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6134b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6134b-114">Not supported.</span></span>|
|<span data-ttu-id="6134b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6134b-115">Application</span></span>|<span data-ttu-id="6134b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6134b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6134b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6134b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/defaultManagedAppProtections
```

## <a name="request-headers"></a><span data-ttu-id="6134b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6134b-118">Request headers</span></span>
|<span data-ttu-id="6134b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6134b-119">Header</span></span>|<span data-ttu-id="6134b-120">値</span><span class="sxs-lookup"><span data-stu-id="6134b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6134b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6134b-121">Authorization</span></span>|<span data-ttu-id="6134b-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6134b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6134b-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6134b-123">Accept</span></span>|<span data-ttu-id="6134b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6134b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6134b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6134b-125">Request body</span></span>
<span data-ttu-id="6134b-126">要求本文において、defaultManagedAppProtection オブジェクト用の JSON 表現を提供します。</span><span class="sxs-lookup"><span data-stu-id="6134b-126">In the request body, supply a JSON representation for the defaultManagedAppProtection object.</span></span>

<span data-ttu-id="6134b-127">次の表に、defaultManagedAppProtection 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-127">The following table shows the properties that are required when you create the defaultManagedAppProtection.</span></span>

|<span data-ttu-id="6134b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6134b-128">Property</span></span>|<span data-ttu-id="6134b-129">型</span><span class="sxs-lookup"><span data-stu-id="6134b-129">Type</span></span>|<span data-ttu-id="6134b-130">説明</span><span class="sxs-lookup"><span data-stu-id="6134b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6134b-131">displayName</span><span class="sxs-lookup"><span data-stu-id="6134b-131">displayName</span></span>|<span data-ttu-id="6134b-132">String</span><span class="sxs-lookup"><span data-stu-id="6134b-132">String</span></span>|<span data-ttu-id="6134b-133">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="6134b-133">Policy display name.</span></span> <span data-ttu-id="6134b-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6134b-135">説明</span><span class="sxs-lookup"><span data-stu-id="6134b-135">description</span></span>|<span data-ttu-id="6134b-136">String</span><span class="sxs-lookup"><span data-stu-id="6134b-136">String</span></span>|<span data-ttu-id="6134b-137">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="6134b-137">The policy's description.</span></span> <span data-ttu-id="6134b-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6134b-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6134b-139">createdDateTime</span></span>|<span data-ttu-id="6134b-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6134b-140">DateTimeOffset</span></span>|<span data-ttu-id="6134b-141">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="6134b-141">The date and time the policy was created.</span></span> <span data-ttu-id="6134b-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6134b-143">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6134b-143">lastModifiedDateTime</span></span>|<span data-ttu-id="6134b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6134b-144">DateTimeOffset</span></span>|<span data-ttu-id="6134b-145">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="6134b-145">Last time the policy was modified.</span></span> <span data-ttu-id="6134b-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6134b-147">id</span><span class="sxs-lookup"><span data-stu-id="6134b-147">id</span></span>|<span data-ttu-id="6134b-148">String</span><span class="sxs-lookup"><span data-stu-id="6134b-148">String</span></span>|<span data-ttu-id="6134b-149">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6134b-149">Key of the entity.</span></span> <span data-ttu-id="6134b-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6134b-151">version</span><span class="sxs-lookup"><span data-stu-id="6134b-151">version</span></span>|<span data-ttu-id="6134b-152">String</span><span class="sxs-lookup"><span data-stu-id="6134b-152">String</span></span>|<span data-ttu-id="6134b-153">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6134b-153">Version of the entity.</span></span> <span data-ttu-id="6134b-154">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-154">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6134b-155">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="6134b-155">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="6134b-156">期間</span><span class="sxs-lookup"><span data-stu-id="6134b-156">Duration</span></span>|<span data-ttu-id="6134b-157">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="6134b-157">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="6134b-158">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-158">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-159">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="6134b-159">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="6134b-160">期間</span><span class="sxs-lookup"><span data-stu-id="6134b-160">Duration</span></span>|<span data-ttu-id="6134b-161">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="6134b-161">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="6134b-162">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-162">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-163">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="6134b-163">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="6134b-164">managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="6134b-164">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="6134b-165">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="6134b-165">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="6134b-166">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6134b-166">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6134b-167">可能な値は `allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="6134b-167">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="6134b-168">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="6134b-168">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="6134b-169">managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="6134b-169">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="6134b-170">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="6134b-170">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="6134b-171">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6134b-171">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6134b-172">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="6134b-172">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="6134b-173">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="6134b-173">organizationalCredentialsRequired</span></span>|<span data-ttu-id="6134b-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-174">Boolean</span></span>|<span data-ttu-id="6134b-175">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-175">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="6134b-176">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-176">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-177">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="6134b-177">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="6134b-178">managedappクリップボードの sharinglevel</span><span class="sxs-lookup"><span data-stu-id="6134b-178">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="6134b-179">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="6134b-179">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="6134b-180">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6134b-180">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6134b-181">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="6134b-181">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="6134b-182">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="6134b-182">dataBackupBlocked</span></span>|<span data-ttu-id="6134b-183">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-183">Boolean</span></span>|<span data-ttu-id="6134b-184">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-184">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="6134b-185">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-185">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-186">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="6134b-186">deviceComplianceRequired</span></span>|<span data-ttu-id="6134b-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-187">Boolean</span></span>|<span data-ttu-id="6134b-188">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-188">Indicates whether device compliance is required.</span></span> <span data-ttu-id="6134b-189">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-189">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-190">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="6134b-190">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="6134b-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-191">Boolean</span></span>|<span data-ttu-id="6134b-192">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-192">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="6134b-193">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-193">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-194">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="6134b-194">saveAsBlocked</span></span>|<span data-ttu-id="6134b-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-195">Boolean</span></span>|<span data-ttu-id="6134b-196">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-196">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="6134b-197">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-197">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-198">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="6134b-198">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="6134b-199">期間</span><span class="sxs-lookup"><span data-stu-id="6134b-199">Duration</span></span>|<span data-ttu-id="6134b-200">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="6134b-200">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="6134b-201">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-201">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-202">pinRequired</span><span class="sxs-lookup"><span data-stu-id="6134b-202">pinRequired</span></span>|<span data-ttu-id="6134b-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-203">Boolean</span></span>|<span data-ttu-id="6134b-204">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-204">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="6134b-205">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-205">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-206">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="6134b-206">maximumPinRetries</span></span>|<span data-ttu-id="6134b-207">Int32</span><span class="sxs-lookup"><span data-stu-id="6134b-207">Int32</span></span>|<span data-ttu-id="6134b-208">管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。</span><span class="sxs-lookup"><span data-stu-id="6134b-208">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="6134b-209">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-209">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-210">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="6134b-210">simplePinBlocked</span></span>|<span data-ttu-id="6134b-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-211">Boolean</span></span>|<span data-ttu-id="6134b-212">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-212">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="6134b-213">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-213">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-214">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="6134b-214">minimumPinLength</span></span>|<span data-ttu-id="6134b-215">Int32</span><span class="sxs-lookup"><span data-stu-id="6134b-215">Int32</span></span>|<span data-ttu-id="6134b-216">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="6134b-216">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-217">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="6134b-217">pinCharacterSet</span></span>|[<span data-ttu-id="6134b-218">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="6134b-218">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="6134b-219">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="6134b-219">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="6134b-220">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6134b-220">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6134b-221">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="6134b-221">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="6134b-222">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="6134b-222">periodBeforePinReset</span></span>|<span data-ttu-id="6134b-223">Duration</span><span class="sxs-lookup"><span data-stu-id="6134b-223">Duration</span></span>|<span data-ttu-id="6134b-224">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6134b-224">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="6134b-225">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-225">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-226">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="6134b-226">allowedDataStorageLocations</span></span>|<span data-ttu-id="6134b-227">[managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="6134b-227">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="6134b-228">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="6134b-228">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="6134b-229">[managedappprotection](../resources/intune-mam-managedappprotection.md)から継承します。</span><span class="sxs-lookup"><span data-stu-id="6134b-229">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="6134b-230">可能な値は `oneDriveForBusiness`、`sharePoint`、`localStorage` です。</span><span class="sxs-lookup"><span data-stu-id="6134b-230">Possible values are: `oneDriveForBusiness`, `sharePoint`, `localStorage`.</span></span>|
|<span data-ttu-id="6134b-231">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="6134b-231">contactSyncBlocked</span></span>|<span data-ttu-id="6134b-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-232">Boolean</span></span>|<span data-ttu-id="6134b-233">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-233">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="6134b-234">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-234">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-235">printBlocked</span><span class="sxs-lookup"><span data-stu-id="6134b-235">printBlocked</span></span>|<span data-ttu-id="6134b-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-236">Boolean</span></span>|<span data-ttu-id="6134b-237">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-237">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="6134b-238">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-238">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-239">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="6134b-239">fingerprintBlocked</span></span>|<span data-ttu-id="6134b-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-240">Boolean</span></span>|<span data-ttu-id="6134b-241">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-241">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="6134b-242">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-242">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-243">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="6134b-243">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="6134b-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-244">Boolean</span></span>|<span data-ttu-id="6134b-245">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-245">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="6134b-246">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-246">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-247">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="6134b-247">minimumRequiredOsVersion</span></span>|<span data-ttu-id="6134b-248">String</span><span class="sxs-lookup"><span data-stu-id="6134b-248">String</span></span>|<span data-ttu-id="6134b-249">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="6134b-249">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="6134b-250">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-250">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-251">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="6134b-251">minimumWarningOsVersion</span></span>|<span data-ttu-id="6134b-252">String</span><span class="sxs-lookup"><span data-stu-id="6134b-252">String</span></span>|<span data-ttu-id="6134b-253">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6134b-253">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="6134b-254">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-254">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-255">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="6134b-255">minimumRequiredAppVersion</span></span>|<span data-ttu-id="6134b-256">String</span><span class="sxs-lookup"><span data-stu-id="6134b-256">String</span></span>|<span data-ttu-id="6134b-257">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="6134b-257">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="6134b-258">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-258">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-259">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="6134b-259">minimumWarningAppVersion</span></span>|<span data-ttu-id="6134b-260">String</span><span class="sxs-lookup"><span data-stu-id="6134b-260">String</span></span>|<span data-ttu-id="6134b-261">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="6134b-261">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="6134b-262">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6134b-262">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="6134b-263">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="6134b-263">appDataEncryptionType</span></span>|[<span data-ttu-id="6134b-264">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="6134b-264">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="6134b-265">管理対象アプリのデータに使用する暗号化の種類。</span><span class="sxs-lookup"><span data-stu-id="6134b-265">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="6134b-266">(iOS のみ)。</span><span class="sxs-lookup"><span data-stu-id="6134b-266">(iOS Only).</span></span> <span data-ttu-id="6134b-267">使用可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。</span><span class="sxs-lookup"><span data-stu-id="6134b-267">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="6134b-268">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="6134b-268">screenCaptureBlocked</span></span>|<span data-ttu-id="6134b-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-269">Boolean</span></span>|<span data-ttu-id="6134b-270">画面キャプチャがブロックされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-270">Indicates whether screen capture is blocked.</span></span> <span data-ttu-id="6134b-271">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="6134b-271">(Android only)</span></span>|
|<span data-ttu-id="6134b-272">encryptAppData</span><span class="sxs-lookup"><span data-stu-id="6134b-272">encryptAppData</span></span>|<span data-ttu-id="6134b-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-273">Boolean</span></span>|<span data-ttu-id="6134b-274">管理対象アプリのデータを暗号化するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-274">Indicates whether managed-app data should be encrypted.</span></span> <span data-ttu-id="6134b-275">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="6134b-275">(Android only)</span></span>|
|<span data-ttu-id="6134b-276">disableAppEncryptionIfDeviceEncryptionIsEnabled</span><span class="sxs-lookup"><span data-stu-id="6134b-276">disableAppEncryptionIfDeviceEncryptionIsEnabled</span></span>|<span data-ttu-id="6134b-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-277">Boolean</span></span>|<span data-ttu-id="6134b-278">この設定を有効にすると、デバイスレベルの暗号化が有効になっている場合、アプリレベルの暗号化が無効になります。</span><span class="sxs-lookup"><span data-stu-id="6134b-278">When this setting is enabled, app level encryption is disabled if device level encryption is enabled.</span></span> <span data-ttu-id="6134b-279">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="6134b-279">(Android only)</span></span>|
|<span data-ttu-id="6134b-280">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="6134b-280">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="6134b-281">String</span><span class="sxs-lookup"><span data-stu-id="6134b-281">String</span></span>|<span data-ttu-id="6134b-282">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="6134b-282">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="6134b-283">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="6134b-283">(iOS Only)</span></span>|
|<span data-ttu-id="6134b-284">customSettings</span><span class="sxs-lookup"><span data-stu-id="6134b-284">customSettings</span></span>|<span data-ttu-id="6134b-285">[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6134b-285">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6134b-286">このサービスで変更されずに、影響を受けるユーザーに送信される、文字列のキーと文字列の値のペアのセット</span><span class="sxs-lookup"><span data-stu-id="6134b-286">A set of string key and string value pairs to be sent to the affected users, unalterned by this service</span></span>|
|<span data-ttu-id="6134b-287">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="6134b-287">deployedAppCount</span></span>|<span data-ttu-id="6134b-288">Int32</span><span class="sxs-lookup"><span data-stu-id="6134b-288">Int32</span></span>|<span data-ttu-id="6134b-289">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="6134b-289">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="6134b-290">minimumRequiredPatchVersion</span><span class="sxs-lookup"><span data-stu-id="6134b-290">minimumRequiredPatchVersion</span></span>|<span data-ttu-id="6134b-291">String</span><span class="sxs-lookup"><span data-stu-id="6134b-291">String</span></span>|<span data-ttu-id="6134b-292">ユーザーがアプリに安全にアクセスできるための、最も古い、必須の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="6134b-292">Define the oldest required Android security patch level a user can have to gain secure access to the app.</span></span> <span data-ttu-id="6134b-293">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="6134b-293">(Android only)</span></span>|
|<span data-ttu-id="6134b-294">minimumWarningPatchVersion</span><span class="sxs-lookup"><span data-stu-id="6134b-294">minimumWarningPatchVersion</span></span>|<span data-ttu-id="6134b-295">String</span><span class="sxs-lookup"><span data-stu-id="6134b-295">String</span></span>|<span data-ttu-id="6134b-296">ユーザーがアプリに安全にアクセスできるための、最も古い、推奨の Android セキュリティ パッチのレベルを定義します。</span><span class="sxs-lookup"><span data-stu-id="6134b-296">Define the oldest recommended Android security patch level a user can have for secure access to the app.</span></span> <span data-ttu-id="6134b-297">(Android のみ)</span><span class="sxs-lookup"><span data-stu-id="6134b-297">(Android only)</span></span>|
|<span data-ttu-id="6134b-298">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="6134b-298">faceIdBlocked</span></span>|<span data-ttu-id="6134b-299">Boolean</span><span class="sxs-lookup"><span data-stu-id="6134b-299">Boolean</span></span>|<span data-ttu-id="6134b-300">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6134b-300">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="6134b-301">(iOS のみ)</span><span class="sxs-lookup"><span data-stu-id="6134b-301">(iOS Only)</span></span>|



## <a name="response"></a><span data-ttu-id="6134b-302">応答</span><span class="sxs-lookup"><span data-stu-id="6134b-302">Response</span></span>
<span data-ttu-id="6134b-303">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6134b-303">If successful, this method returns a `201 Created` response code and a [defaultManagedAppProtection](../resources/intune-mam-defaultmanagedappprotection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6134b-304">例</span><span class="sxs-lookup"><span data-stu-id="6134b-304">Example</span></span>

### <a name="request"></a><span data-ttu-id="6134b-305">要求</span><span class="sxs-lookup"><span data-stu-id="6134b-305">Request</span></span>
<span data-ttu-id="6134b-306">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6134b-306">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6134b-307">応答</span><span class="sxs-lookup"><span data-stu-id="6134b-307">Response</span></span>
<span data-ttu-id="6134b-p141">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6134b-p141">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



