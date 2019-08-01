---
title: managedAppProtection リソース タイプ
description: 指定した一連のアプリの詳細な管理設定を構成するために使用されるポリシー
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 017687178f87107060600e5888eef9e13bbdadcf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037920"
---
# <a name="managedappprotection-resource-type"></a><span data-ttu-id="c64c5-103">managedAppProtection リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="c64c5-103">managedAppProtection resource type</span></span>

> <span data-ttu-id="c64c5-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c64c5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c64c5-105">指定した一連のアプリの詳細な管理設定を構成するために使用されるポリシー</span><span class="sxs-lookup"><span data-stu-id="c64c5-105">Policy used to configure detailed management settings for a specified set of apps</span></span>


<span data-ttu-id="c64c5-106">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c64c5-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="c64c5-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="c64c5-107">Methods</span></span>
|<span data-ttu-id="c64c5-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="c64c5-108">Method</span></span>|<span data-ttu-id="c64c5-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="c64c5-109">Return Type</span></span>|<span data-ttu-id="c64c5-110">説明</span><span class="sxs-lookup"><span data-stu-id="c64c5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c64c5-111">List managedAppProtections</span><span class="sxs-lookup"><span data-stu-id="c64c5-111">List managedAppProtections</span></span>](../api/intune-mam-managedappprotection-list.md)|<span data-ttu-id="c64c5-112">[managedAppProtection](../resources/intune-mam-managedappprotection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="c64c5-112">[managedAppProtection](../resources/intune-mam-managedappprotection.md) collection</span></span>|<span data-ttu-id="c64c5-113">[managedAppProtection](../resources/intune-mam-managedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="c64c5-113">List properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) objects.</span></span>|
|[<span data-ttu-id="c64c5-114">Get managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c64c5-114">Get managedAppProtection</span></span>](../api/intune-mam-managedappprotection-get.md)|[<span data-ttu-id="c64c5-115">managedAppProtection</span><span class="sxs-lookup"><span data-stu-id="c64c5-115">managedAppProtection</span></span>](../resources/intune-mam-managedappprotection.md)|<span data-ttu-id="c64c5-116">[managedAppProtection](../resources/intune-mam-managedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c64c5-116">Read properties and relationships of the [managedAppProtection](../resources/intune-mam-managedappprotection.md) object.</span></span>|
|[<span data-ttu-id="c64c5-117">targetApps action</span><span class="sxs-lookup"><span data-stu-id="c64c5-117">targetApps action</span></span>](../api/intune-mam-managedappprotection-targetapps.md)|<span data-ttu-id="c64c5-118">なし</span><span class="sxs-lookup"><span data-stu-id="c64c5-118">None</span></span>|<span data-ttu-id="c64c5-119">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="c64c5-119">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="c64c5-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c64c5-120">Properties</span></span>
|<span data-ttu-id="c64c5-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c64c5-121">Property</span></span>|<span data-ttu-id="c64c5-122">型</span><span class="sxs-lookup"><span data-stu-id="c64c5-122">Type</span></span>|<span data-ttu-id="c64c5-123">説明</span><span class="sxs-lookup"><span data-stu-id="c64c5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c64c5-124">displayName</span><span class="sxs-lookup"><span data-stu-id="c64c5-124">displayName</span></span>|<span data-ttu-id="c64c5-125">String</span><span class="sxs-lookup"><span data-stu-id="c64c5-125">String</span></span>|<span data-ttu-id="c64c5-126">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="c64c5-126">Policy display name.</span></span> <span data-ttu-id="c64c5-127">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c64c5-127">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c64c5-128">description</span><span class="sxs-lookup"><span data-stu-id="c64c5-128">description</span></span>|<span data-ttu-id="c64c5-129">String</span><span class="sxs-lookup"><span data-stu-id="c64c5-129">String</span></span>|<span data-ttu-id="c64c5-130">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="c64c5-130">The policy's description.</span></span> <span data-ttu-id="c64c5-131">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c64c5-131">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c64c5-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c64c5-132">createdDateTime</span></span>|<span data-ttu-id="c64c5-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c64c5-133">DateTimeOffset</span></span>|<span data-ttu-id="c64c5-134">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="c64c5-134">The date and time the policy was created.</span></span> <span data-ttu-id="c64c5-135">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c64c5-135">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c64c5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c64c5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c64c5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c64c5-137">DateTimeOffset</span></span>|<span data-ttu-id="c64c5-138">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="c64c5-138">Last time the policy was modified.</span></span> <span data-ttu-id="c64c5-139">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c64c5-139">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c64c5-140">id</span><span class="sxs-lookup"><span data-stu-id="c64c5-140">id</span></span>|<span data-ttu-id="c64c5-141">文字列</span><span class="sxs-lookup"><span data-stu-id="c64c5-141">String</span></span>|<span data-ttu-id="c64c5-142">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c64c5-142">Key of the entity.</span></span> <span data-ttu-id="c64c5-143">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c64c5-143">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c64c5-144">version</span><span class="sxs-lookup"><span data-stu-id="c64c5-144">version</span></span>|<span data-ttu-id="c64c5-145">String</span><span class="sxs-lookup"><span data-stu-id="c64c5-145">String</span></span>|<span data-ttu-id="c64c5-146">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="c64c5-146">Version of the entity.</span></span> <span data-ttu-id="c64c5-147">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="c64c5-147">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="c64c5-148">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="c64c5-148">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="c64c5-149">期間</span><span class="sxs-lookup"><span data-stu-id="c64c5-149">Duration</span></span>|<span data-ttu-id="c64c5-150">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="c64c5-150">The period after which access is checked when the device is not connected to the internet.</span></span>|
|<span data-ttu-id="c64c5-151">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="c64c5-151">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="c64c5-152">期間</span><span class="sxs-lookup"><span data-stu-id="c64c5-152">Duration</span></span>|<span data-ttu-id="c64c5-153">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="c64c5-153">The period after which access is checked when the device is connected to the internet.</span></span>|
|<span data-ttu-id="c64c5-154">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="c64c5-154">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="c64c5-155">Managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="c64c5-155">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="c64c5-156">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="c64c5-156">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="c64c5-157">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="c64c5-157">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="c64c5-158">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="c64c5-158">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="c64c5-159">Managedappdatatransフェリーレベル</span><span class="sxs-lookup"><span data-stu-id="c64c5-159">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="c64c5-160">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="c64c5-160">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="c64c5-161">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="c64c5-161">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="c64c5-162">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="c64c5-162">organizationalCredentialsRequired</span></span>|<span data-ttu-id="c64c5-163">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-163">Boolean</span></span>|<span data-ttu-id="c64c5-164">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-164">Indicates whether organizational credentials are required for app use.</span></span>|
|<span data-ttu-id="c64c5-165">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="c64c5-165">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="c64c5-166">Managedappクリップボードの Sharinglevel</span><span class="sxs-lookup"><span data-stu-id="c64c5-166">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="c64c5-167">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="c64c5-167">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="c64c5-168">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="c64c5-168">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="c64c5-169">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="c64c5-169">dataBackupBlocked</span></span>|<span data-ttu-id="c64c5-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-170">Boolean</span></span>|<span data-ttu-id="c64c5-171">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-171">Indicates whether the backup of a managed app's data is blocked.</span></span>|
|<span data-ttu-id="c64c5-172">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="c64c5-172">deviceComplianceRequired</span></span>|<span data-ttu-id="c64c5-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-173">Boolean</span></span>|<span data-ttu-id="c64c5-174">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-174">Indicates whether device compliance is required.</span></span>|
|<span data-ttu-id="c64c5-175">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="c64c5-175">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="c64c5-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-176">Boolean</span></span>|<span data-ttu-id="c64c5-177">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-177">Indicates whether internet links should be opened in the managed browser app.</span></span>|
|<span data-ttu-id="c64c5-178">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="c64c5-178">saveAsBlocked</span></span>|<span data-ttu-id="c64c5-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-179">Boolean</span></span>|<span data-ttu-id="c64c5-180">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-180">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span>|
|<span data-ttu-id="c64c5-181">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="c64c5-181">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="c64c5-182">期間</span><span class="sxs-lookup"><span data-stu-id="c64c5-182">Duration</span></span>|<span data-ttu-id="c64c5-183">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="c64c5-183">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span>|
|<span data-ttu-id="c64c5-184">pinRequired</span><span class="sxs-lookup"><span data-stu-id="c64c5-184">pinRequired</span></span>|<span data-ttu-id="c64c5-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-185">Boolean</span></span>|<span data-ttu-id="c64c5-186">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-186">Indicates whether an app-level pin is required.</span></span>|
|<span data-ttu-id="c64c5-187">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="c64c5-187">maximumPinRetries</span></span>|<span data-ttu-id="c64c5-188">Int32</span><span class="sxs-lookup"><span data-stu-id="c64c5-188">Int32</span></span>|<span data-ttu-id="c64c5-189">管理対象アプリがブロックまたはワイプされるまでの、正しくない pin の再試行回数の最大数。</span><span class="sxs-lookup"><span data-stu-id="c64c5-189">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span>|
|<span data-ttu-id="c64c5-190">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="c64c5-190">simplePinBlocked</span></span>|<span data-ttu-id="c64c5-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-191">Boolean</span></span>|<span data-ttu-id="c64c5-192">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-192">Indicates whether simplePin is blocked.</span></span>|
|<span data-ttu-id="c64c5-193">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="c64c5-193">minimumPinLength</span></span>|<span data-ttu-id="c64c5-194">Int32</span><span class="sxs-lookup"><span data-stu-id="c64c5-194">Int32</span></span>|<span data-ttu-id="c64c5-195">PinRequired が True に設定されている場合に、アプリ レベルの pin に必要な最小の pin の長さ</span><span class="sxs-lookup"><span data-stu-id="c64c5-195">Minimum pin length required for an app-level pin if PinRequired is set to True</span></span>|
|<span data-ttu-id="c64c5-196">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="c64c5-196">pinCharacterSet</span></span>|[<span data-ttu-id="c64c5-197">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="c64c5-197">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="c64c5-198">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="c64c5-198">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="c64c5-199">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="c64c5-199">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="c64c5-200">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="c64c5-200">periodBeforePinReset</span></span>|<span data-ttu-id="c64c5-201">Duration</span><span class="sxs-lookup"><span data-stu-id="c64c5-201">Duration</span></span>|<span data-ttu-id="c64c5-202">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="c64c5-202">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span>|
|<span data-ttu-id="c64c5-203">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="c64c5-203">allowedDataStorageLocations</span></span>|<span data-ttu-id="c64c5-204">[Managedappdatastoragelocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="c64c5-204">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="c64c5-205">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="c64c5-205">Data storage locations where a user may store managed data.</span></span>|
|<span data-ttu-id="c64c5-206">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="c64c5-206">contactSyncBlocked</span></span>|<span data-ttu-id="c64c5-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-207">Boolean</span></span>|<span data-ttu-id="c64c5-208">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-208">Indicates whether contacts can be synced to the user's device.</span></span>|
|<span data-ttu-id="c64c5-209">printBlocked</span><span class="sxs-lookup"><span data-stu-id="c64c5-209">printBlocked</span></span>|<span data-ttu-id="c64c5-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-210">Boolean</span></span>|<span data-ttu-id="c64c5-211">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-211">Indicates whether printing is allowed from managed apps.</span></span>|
|<span data-ttu-id="c64c5-212">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="c64c5-212">fingerprintBlocked</span></span>|<span data-ttu-id="c64c5-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-213">Boolean</span></span>|<span data-ttu-id="c64c5-214">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-214">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span>|
|<span data-ttu-id="c64c5-215">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="c64c5-215">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="c64c5-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="c64c5-216">Boolean</span></span>|<span data-ttu-id="c64c5-217">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c64c5-217">Indicates whether use of the app pin is required if the device pin is set.</span></span>|
|<span data-ttu-id="c64c5-218">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="c64c5-218">minimumRequiredOsVersion</span></span>|<span data-ttu-id="c64c5-219">String</span><span class="sxs-lookup"><span data-stu-id="c64c5-219">String</span></span>|<span data-ttu-id="c64c5-220">OS のバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="c64c5-220">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="c64c5-221">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="c64c5-221">minimumWarningOsVersion</span></span>|<span data-ttu-id="c64c5-222">String</span><span class="sxs-lookup"><span data-stu-id="c64c5-222">String</span></span>|<span data-ttu-id="c64c5-223">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="c64c5-223">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span>|
|<span data-ttu-id="c64c5-224">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="c64c5-224">minimumRequiredAppVersion</span></span>|<span data-ttu-id="c64c5-225">String</span><span class="sxs-lookup"><span data-stu-id="c64c5-225">String</span></span>|<span data-ttu-id="c64c5-226">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="c64c5-226">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="c64c5-227">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="c64c5-227">minimumWarningAppVersion</span></span>|<span data-ttu-id="c64c5-228">String</span><span class="sxs-lookup"><span data-stu-id="c64c5-228">String</span></span>|<span data-ttu-id="c64c5-229">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="c64c5-229">Versions less than the specified version will result in warning message on the managed app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c64c5-230">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="c64c5-230">Relationships</span></span>
<span data-ttu-id="c64c5-231">なし</span><span class="sxs-lookup"><span data-stu-id="c64c5-231">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c64c5-232">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c64c5-232">JSON Representation</span></span>
<span data-ttu-id="c64c5-233">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c64c5-233">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppProtection",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "periodOfflineBeforeAccessCheck": "String (duration)",
  "periodOnlineBeforeAccessCheck": "String (duration)",
  "allowedInboundDataTransferSources": "String",
  "allowedOutboundDataTransferDestinations": "String",
  "organizationalCredentialsRequired": true,
  "allowedOutboundClipboardSharingLevel": "String",
  "dataBackupBlocked": true,
  "deviceComplianceRequired": true,
  "managedBrowserToOpenLinksRequired": true,
  "saveAsBlocked": true,
  "periodOfflineBeforeWipeIsEnforced": "String (duration)",
  "pinRequired": true,
  "maximumPinRetries": 1024,
  "simplePinBlocked": true,
  "minimumPinLength": 1024,
  "pinCharacterSet": "String",
  "periodBeforePinReset": "String (duration)",
  "allowedDataStorageLocations": [
    "String"
  ],
  "contactSyncBlocked": true,
  "printBlocked": true,
  "fingerprintBlocked": true,
  "disableAppPinIfDevicePinIsSet": true,
  "minimumRequiredOsVersion": "String",
  "minimumWarningOsVersion": "String",
  "minimumRequiredAppVersion": "String",
  "minimumWarningAppVersion": "String"
}
```


<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-managedappprotection.md/microsoft.graph.managedAppProtection/allowedDataStorageLocations:
    Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->

