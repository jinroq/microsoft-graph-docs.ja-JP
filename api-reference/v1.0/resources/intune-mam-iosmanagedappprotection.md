---
title: iosManagedAppProtection リソース タイプ
description: iOS デバイス上の特定のセキュリティ グループおよびアプリの特定のセットを対象とした、管理設定の詳細を構成するために使用するポリシー
author: tfitzmac
ms.openlocfilehash: b0323564851548b31533f9ee0c4c6cd38ae25984
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359956"
---
# <a name="iosmanagedappprotection-resource-type"></a><span data-ttu-id="1b0e1-103">iosManagedAppProtection リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="1b0e1-103">iosManagedAppProtection resource type</span></span>

> <span data-ttu-id="1b0e1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b0e1-105">iOS デバイス上の特定のセキュリティ グループおよびアプリの特定のセットを対象とした、管理設定の詳細を構成するために使用するポリシー</span><span class="sxs-lookup"><span data-stu-id="1b0e1-105">Policy used to configure detailed management settings targeted to specific security groups and for a specified set of apps on an iOS device</span></span>

<span data-ttu-id="1b0e1-106">[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-106">Inherits from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1b0e1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1b0e1-107">Methods</span></span>
|<span data-ttu-id="1b0e1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="1b0e1-108">Method</span></span>|<span data-ttu-id="1b0e1-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1b0e1-109">Return Type</span></span>|<span data-ttu-id="1b0e1-110">説明</span><span class="sxs-lookup"><span data-stu-id="1b0e1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b0e1-111">List iosManagedAppProtections</span><span class="sxs-lookup"><span data-stu-id="1b0e1-111">List iosManagedAppProtections</span></span>](../api/intune-mam-iosmanagedappprotection-list.md)|<span data-ttu-id="1b0e1-112">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1b0e1-112">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) collection</span></span>|<span data-ttu-id="1b0e1-113">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-113">List properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) objects.</span></span>|
|[<span data-ttu-id="1b0e1-114">Get iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1b0e1-114">Get iosManagedAppProtection</span></span>](../api/intune-mam-iosmanagedappprotection-get.md)|[<span data-ttu-id="1b0e1-115">iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1b0e1-115">iosManagedAppProtection</span></span>](../resources/intune-mam-iosmanagedappprotection.md)|<span data-ttu-id="1b0e1-116">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-116">Read properties and relationships of the [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>|
|[<span data-ttu-id="1b0e1-117">Create iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1b0e1-117">Create iosManagedAppProtection</span></span>](../api/intune-mam-iosmanagedappprotection-create.md)|[<span data-ttu-id="1b0e1-118">iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1b0e1-118">iosManagedAppProtection</span></span>](../resources/intune-mam-iosmanagedappprotection.md)|<span data-ttu-id="1b0e1-119">新しい [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-119">Create a new [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>|
|[<span data-ttu-id="1b0e1-120">Delete iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1b0e1-120">Delete iosManagedAppProtection</span></span>](../api/intune-mam-iosmanagedappprotection-delete.md)|<span data-ttu-id="1b0e1-121">なし</span><span class="sxs-lookup"><span data-stu-id="1b0e1-121">None</span></span>|<span data-ttu-id="1b0e1-122">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-122">Deletes a [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md).</span></span>|
|[<span data-ttu-id="1b0e1-123">Update iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1b0e1-123">Update iosManagedAppProtection</span></span>](../api/intune-mam-iosmanagedappprotection-update.md)|[<span data-ttu-id="1b0e1-124">iosManagedAppProtection</span><span class="sxs-lookup"><span data-stu-id="1b0e1-124">iosManagedAppProtection</span></span>](../resources/intune-mam-iosmanagedappprotection.md)|<span data-ttu-id="1b0e1-125">[iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-125">Update the properties of a [iosManagedAppProtection](../resources/intune-mam-iosmanagedappprotection.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b0e1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b0e1-126">Properties</span></span>
|<span data-ttu-id="1b0e1-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b0e1-127">Property</span></span>|<span data-ttu-id="1b0e1-128">種類</span><span class="sxs-lookup"><span data-stu-id="1b0e1-128">Type</span></span>|<span data-ttu-id="1b0e1-129">説明</span><span class="sxs-lookup"><span data-stu-id="1b0e1-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b0e1-130">displayName</span><span class="sxs-lookup"><span data-stu-id="1b0e1-130">displayName</span></span>|<span data-ttu-id="1b0e1-131">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-131">String</span></span>|<span data-ttu-id="1b0e1-132">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-132">Policy display name.</span></span> <span data-ttu-id="1b0e1-133">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b0e1-134">説明</span><span class="sxs-lookup"><span data-stu-id="1b0e1-134">description</span></span>|<span data-ttu-id="1b0e1-135">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-135">String</span></span>|<span data-ttu-id="1b0e1-136">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-136">The policy's description.</span></span> <span data-ttu-id="1b0e1-137">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b0e1-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0e1-138">createdDateTime</span></span>|<span data-ttu-id="1b0e1-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0e1-139">DateTimeOffset</span></span>|<span data-ttu-id="1b0e1-140">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-140">The date and time the policy was created.</span></span> <span data-ttu-id="1b0e1-141">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b0e1-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0e1-142">lastModifiedDateTime</span></span>|<span data-ttu-id="1b0e1-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0e1-143">DateTimeOffset</span></span>|<span data-ttu-id="1b0e1-144">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-144">Last time the policy was modified.</span></span> <span data-ttu-id="1b0e1-145">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b0e1-146">id</span><span class="sxs-lookup"><span data-stu-id="1b0e1-146">id</span></span>|<span data-ttu-id="1b0e1-147">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-147">String</span></span>|<span data-ttu-id="1b0e1-148">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-148">Key of the entity.</span></span> <span data-ttu-id="1b0e1-149">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b0e1-150">version</span><span class="sxs-lookup"><span data-stu-id="1b0e1-150">version</span></span>|<span data-ttu-id="1b0e1-151">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-151">String</span></span>|<span data-ttu-id="1b0e1-152">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-152">Version of the entity.</span></span> <span data-ttu-id="1b0e1-153">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-153">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="1b0e1-154">periodOfflineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="1b0e1-154">periodOfflineBeforeAccessCheck</span></span>|<span data-ttu-id="1b0e1-155">Duration</span><span class="sxs-lookup"><span data-stu-id="1b0e1-155">Duration</span></span>|<span data-ttu-id="1b0e1-156">デバイスがインターネットに接続されていないでこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-156">The period after which access is checked when the device is not connected to the internet.</span></span> <span data-ttu-id="1b0e1-157">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-157">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-158">periodOnlineBeforeAccessCheck</span><span class="sxs-lookup"><span data-stu-id="1b0e1-158">periodOnlineBeforeAccessCheck</span></span>|<span data-ttu-id="1b0e1-159">Duration</span><span class="sxs-lookup"><span data-stu-id="1b0e1-159">Duration</span></span>|<span data-ttu-id="1b0e1-160">デバイスがインターネットに接続されていてこの期間が過ぎると、アクセスがチェックされます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-160">The period after which access is checked when the device is connected to the internet.</span></span> <span data-ttu-id="1b0e1-161">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-161">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-162">allowedInboundDataTransferSources</span><span class="sxs-lookup"><span data-stu-id="1b0e1-162">allowedInboundDataTransferSources</span></span>|[<span data-ttu-id="1b0e1-163">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="1b0e1-163">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="1b0e1-164">データの転送が許可されたソース。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-164">Sources from which data is allowed to be transferred.</span></span> <span data-ttu-id="1b0e1-165">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-165">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="1b0e1-166">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-166">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="1b0e1-167">allowedOutboundDataTransferDestinations</span><span class="sxs-lookup"><span data-stu-id="1b0e1-167">allowedOutboundDataTransferDestinations</span></span>|[<span data-ttu-id="1b0e1-168">managedAppDataTransferLevel</span><span class="sxs-lookup"><span data-stu-id="1b0e1-168">managedAppDataTransferLevel</span></span>](../resources/intune-mam-managedappdatatransferlevel.md)|<span data-ttu-id="1b0e1-169">データの転送が許可された宛先。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-169">Destinations to which data is allowed to be transferred.</span></span> <span data-ttu-id="1b0e1-170">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-170">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="1b0e1-171">可能な値は、`allApps`、`managedApps`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-171">Possible values are: `allApps`, `managedApps`, `none`.</span></span>|
|<span data-ttu-id="1b0e1-172">organizationalCredentialsRequired</span><span class="sxs-lookup"><span data-stu-id="1b0e1-172">organizationalCredentialsRequired</span></span>|<span data-ttu-id="1b0e1-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-173">Boolean</span></span>|<span data-ttu-id="1b0e1-174">アプリを使用するために組織の資格情報が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-174">Indicates whether organizational credentials are required for app use.</span></span> <span data-ttu-id="1b0e1-175">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-175">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-176">allowedOutboundClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="1b0e1-176">allowedOutboundClipboardSharingLevel</span></span>|[<span data-ttu-id="1b0e1-177">managedAppClipboardSharingLevel</span><span class="sxs-lookup"><span data-stu-id="1b0e1-177">managedAppClipboardSharingLevel</span></span>](../resources/intune-mam-managedappclipboardsharinglevel.md)|<span data-ttu-id="1b0e1-178">管理対象デバイスで、アプリ間でクリップボードを共有できるレベル。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-178">The level to which the clipboard may be shared between apps on the managed device.</span></span> <span data-ttu-id="1b0e1-179">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-179">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="1b0e1-180">可能な値は、`allApps`、`managedAppsWithPasteIn`、`managedApps`、`blocked` です。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-180">Possible values are: `allApps`, `managedAppsWithPasteIn`, `managedApps`, `blocked`.</span></span>|
|<span data-ttu-id="1b0e1-181">dataBackupBlocked</span><span class="sxs-lookup"><span data-stu-id="1b0e1-181">dataBackupBlocked</span></span>|<span data-ttu-id="1b0e1-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-182">Boolean</span></span>|<span data-ttu-id="1b0e1-183">管理対象アプリのデータのバックアップがブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-183">Indicates whether the backup of a managed app's data is blocked.</span></span> <span data-ttu-id="1b0e1-184">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-184">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-185">deviceComplianceRequired</span><span class="sxs-lookup"><span data-stu-id="1b0e1-185">deviceComplianceRequired</span></span>|<span data-ttu-id="1b0e1-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-186">Boolean</span></span>|<span data-ttu-id="1b0e1-187">デバイスの準拠が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-187">Indicates whether device compliance is required.</span></span> <span data-ttu-id="1b0e1-188">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-188">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-189">managedBrowserToOpenLinksRequired</span><span class="sxs-lookup"><span data-stu-id="1b0e1-189">managedBrowserToOpenLinksRequired</span></span>|<span data-ttu-id="1b0e1-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-190">Boolean</span></span>|<span data-ttu-id="1b0e1-191">管理対象ブラウザー アプリでインターネット リンクを開く必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-191">Indicates whether internet links should be opened in the managed browser app.</span></span> <span data-ttu-id="1b0e1-192">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-192">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-193">saveAsBlocked</span><span class="sxs-lookup"><span data-stu-id="1b0e1-193">saveAsBlocked</span></span>|<span data-ttu-id="1b0e1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-194">Boolean</span></span>|<span data-ttu-id="1b0e1-195">ユーザーが保護されたファイルのコピーを保存するために、[名前を付けて保存] メニュー項目を使用できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-195">Indicates whether users may use the "Save As" menu item to save a copy of protected files.</span></span> <span data-ttu-id="1b0e1-196">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-196">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-197">periodOfflineBeforeWipeIsEnforced</span><span class="sxs-lookup"><span data-stu-id="1b0e1-197">periodOfflineBeforeWipeIsEnforced</span></span>|<span data-ttu-id="1b0e1-198">Duration</span><span class="sxs-lookup"><span data-stu-id="1b0e1-198">Duration</span></span>|<span data-ttu-id="1b0e1-199">アプリがインターネットから切断されている状態を維持できる時間数。この時間を過ぎると管理対象データはすべて消去されます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-199">The amount of time an app is allowed to remain disconnected from the internet before all managed data it is wiped.</span></span> <span data-ttu-id="1b0e1-200">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-200">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-201">pinRequired</span><span class="sxs-lookup"><span data-stu-id="1b0e1-201">pinRequired</span></span>|<span data-ttu-id="1b0e1-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-202">Boolean</span></span>|<span data-ttu-id="1b0e1-203">アプリ レベルの pin が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-203">Indicates whether an app-level pin is required.</span></span> <span data-ttu-id="1b0e1-204">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-204">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-205">maximumPinRetries</span><span class="sxs-lookup"><span data-stu-id="1b0e1-205">maximumPinRetries</span></span>|<span data-ttu-id="1b0e1-206">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e1-206">Int32</span></span>|<span data-ttu-id="1b0e1-207">間違った暗証番号 (pin) の再試行の最大数は、マネージ アプリケーションがブロックされているかどうかが消去する前にしようとします。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-207">Maximum number of incorrect pin retry attempts before the managed app is either blocked or wiped.</span></span> <span data-ttu-id="1b0e1-208">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-208">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-209">simplePinBlocked</span><span class="sxs-lookup"><span data-stu-id="1b0e1-209">simplePinBlocked</span></span>|<span data-ttu-id="1b0e1-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-210">Boolean</span></span>|<span data-ttu-id="1b0e1-211">simplePin がブロックされるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-211">Indicates whether simplePin is blocked.</span></span> <span data-ttu-id="1b0e1-212">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-212">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-213">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="1b0e1-213">minimumPinLength</span></span>|<span data-ttu-id="1b0e1-214">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e1-214">Int32</span></span>|<span data-ttu-id="1b0e1-215">PinRequired が True に設定されている場合の、アプリ レベルの pin に必要な最小限の pin の長さ ([managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1b0e1-215">Minimum pin length required for an app-level pin if PinRequired is set to True Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-216">pinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="1b0e1-216">pinCharacterSet</span></span>|[<span data-ttu-id="1b0e1-217">managedAppPinCharacterSet</span><span class="sxs-lookup"><span data-stu-id="1b0e1-217">managedAppPinCharacterSet</span></span>](../resources/intune-mam-managedapppincharacterset.md)|<span data-ttu-id="1b0e1-218">PinRequired が True に設定されている場合に、アプリ レベルの pin に使用できる文字セット。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-218">Character set which may be used for an app-level pin if PinRequired is set to True.</span></span> <span data-ttu-id="1b0e1-219">[ManagedAppProtection](../resources/intune-mam-managedappprotection.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-219">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md).</span></span> <span data-ttu-id="1b0e1-220">可能な値は、`numeric`、`alphanumericAndSymbol` です。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-220">Possible values are: `numeric`, `alphanumericAndSymbol`.</span></span>|
|<span data-ttu-id="1b0e1-221">periodBeforePinReset</span><span class="sxs-lookup"><span data-stu-id="1b0e1-221">periodBeforePinReset</span></span>|<span data-ttu-id="1b0e1-222">Duration</span><span class="sxs-lookup"><span data-stu-id="1b0e1-222">Duration</span></span>|<span data-ttu-id="1b0e1-223">PinRequired が True に設定されている場合、この TimePeriod を過ぎると全レベルの pin を再設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-223">TimePeriod before the all-level pin must be reset if PinRequired is set to True.</span></span> <span data-ttu-id="1b0e1-224">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-224">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-225">allowedDataStorageLocations</span><span class="sxs-lookup"><span data-stu-id="1b0e1-225">allowedDataStorageLocations</span></span>|<span data-ttu-id="1b0e1-226">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1b0e1-226">[managedAppDataStorageLocation](../resources/intune-mam-managedappdatastoragelocation.md) collection</span></span>|<span data-ttu-id="1b0e1-227">ユーザーが管理対象データを格納できるデータの保存場所。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-227">Data storage locations where a user may store managed data.</span></span> <span data-ttu-id="1b0e1-228">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-228">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-229">contactSyncBlocked</span><span class="sxs-lookup"><span data-stu-id="1b0e1-229">contactSyncBlocked</span></span>|<span data-ttu-id="1b0e1-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-230">Boolean</span></span>|<span data-ttu-id="1b0e1-231">連絡先をユーザー デバイスに同期できるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-231">Indicates whether contacts can be synced to the user's device.</span></span> <span data-ttu-id="1b0e1-232">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-232">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-233">printBlocked</span><span class="sxs-lookup"><span data-stu-id="1b0e1-233">printBlocked</span></span>|<span data-ttu-id="1b0e1-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-234">Boolean</span></span>|<span data-ttu-id="1b0e1-235">管理対象アプリからの印刷を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-235">Indicates whether printing is allowed from managed apps.</span></span> <span data-ttu-id="1b0e1-236">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-236">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-237">fingerprintBlocked</span><span class="sxs-lookup"><span data-stu-id="1b0e1-237">fingerprintBlocked</span></span>|<span data-ttu-id="1b0e1-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-238">Boolean</span></span>|<span data-ttu-id="1b0e1-239">PinRequired が True に設定されている場合に、pin の代わりに指紋リーダーの使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-239">Indicates whether use of the fingerprint reader is allowed in place of a pin if PinRequired is set to True.</span></span> <span data-ttu-id="1b0e1-240">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-240">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-241">disableAppPinIfDevicePinIsSet</span><span class="sxs-lookup"><span data-stu-id="1b0e1-241">disableAppPinIfDevicePinIsSet</span></span>|<span data-ttu-id="1b0e1-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-242">Boolean</span></span>|<span data-ttu-id="1b0e1-243">デバイスの pin が設定されている場合に、アプリの pin の使用が必要かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-243">Indicates whether use of the app pin is required if the device pin is set.</span></span> <span data-ttu-id="1b0e1-244">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-244">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-245">minimumRequiredOsVersion</span><span class="sxs-lookup"><span data-stu-id="1b0e1-245">minimumRequiredOsVersion</span></span>|<span data-ttu-id="1b0e1-246">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-246">String</span></span>|<span data-ttu-id="1b0e1-247">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-247">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="1b0e1-248">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-248">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-249">minimumWarningOsVersion</span><span class="sxs-lookup"><span data-stu-id="1b0e1-249">minimumWarningOsVersion</span></span>|<span data-ttu-id="1b0e1-250">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-250">String</span></span>|<span data-ttu-id="1b0e1-251">OS のバージョンが、指定されたバージョンよりも小さい場合に、会社のデータへアクセスすると管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-251">Versions less than the specified version will result in warning message on the managed app from accessing company data.</span></span> <span data-ttu-id="1b0e1-252">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-252">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-253">minimumRequiredAppVersion</span><span class="sxs-lookup"><span data-stu-id="1b0e1-253">minimumRequiredAppVersion</span></span>|<span data-ttu-id="1b0e1-254">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-254">String</span></span>|<span data-ttu-id="1b0e1-255">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-255">Versions less than the specified version will block the managed app from accessing company data.</span></span> <span data-ttu-id="1b0e1-256">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-256">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-257">minimumWarningAppVersion</span><span class="sxs-lookup"><span data-stu-id="1b0e1-257">minimumWarningAppVersion</span></span>|<span data-ttu-id="1b0e1-258">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-258">String</span></span>|<span data-ttu-id="1b0e1-259">アプリのバージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリに警告メッセージが表示されます。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-259">Versions less than the specified version will result in warning message on the managed app.</span></span> <span data-ttu-id="1b0e1-260">[managedAppProtection](../resources/intune-mam-managedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-260">Inherited from [managedAppProtection](../resources/intune-mam-managedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-261">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1b0e1-261">isAssigned</span></span>|<span data-ttu-id="1b0e1-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-262">Boolean</span></span>|<span data-ttu-id="1b0e1-263">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-263">Indicates if the policy is deployed to any inclusion groups or not.</span></span> <span data-ttu-id="1b0e1-264">[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-264">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-265">appDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="1b0e1-265">appDataEncryptionType</span></span>|[<span data-ttu-id="1b0e1-266">managedAppDataEncryptionType</span><span class="sxs-lookup"><span data-stu-id="1b0e1-266">managedAppDataEncryptionType</span></span>](../resources/intune-mam-managedappdataencryptiontype.md)|<span data-ttu-id="1b0e1-267">管理対象アプリのデータに使用する暗号化の種類。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-267">Type of encryption which should be used for data in a managed app.</span></span> <span data-ttu-id="1b0e1-268">可能な値は、`useDeviceSettings`、`afterDeviceRestart`、`whenDeviceLockedExceptOpenFiles`、`whenDeviceLocked` です。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-268">Possible values are: `useDeviceSettings`, `afterDeviceRestart`, `whenDeviceLockedExceptOpenFiles`, `whenDeviceLocked`.</span></span>|
|<span data-ttu-id="1b0e1-269">minimumRequiredSdkVersion</span><span class="sxs-lookup"><span data-stu-id="1b0e1-269">minimumRequiredSdkVersion</span></span>|<span data-ttu-id="1b0e1-270">String</span><span class="sxs-lookup"><span data-stu-id="1b0e1-270">String</span></span>|<span data-ttu-id="1b0e1-271">バージョンが、指定されたバージョンよりも小さい場合に、管理対象アプリによる会社のデータへのアクセスをブロックします。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-271">Versions less than the specified version will block the managed app from accessing company data.</span></span>|
|<span data-ttu-id="1b0e1-272">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="1b0e1-272">deployedAppCount</span></span>|<span data-ttu-id="1b0e1-273">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0e1-273">Int32</span></span>|<span data-ttu-id="1b0e1-274">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-274">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="1b0e1-275">faceIdBlocked</span><span class="sxs-lookup"><span data-stu-id="1b0e1-275">faceIdBlocked</span></span>|<span data-ttu-id="1b0e1-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0e1-276">Boolean</span></span>|<span data-ttu-id="1b0e1-277">PinRequired が True に設定されている場合に、pin の代わりに FaceID の使用を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-277">Indicates whether use of the FaceID is allowed in place of a pin if PinRequired is set to True.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b0e1-278">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1b0e1-278">Relationships</span></span>
|<span data-ttu-id="1b0e1-279">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1b0e1-279">Relationship</span></span>|<span data-ttu-id="1b0e1-280">型</span><span class="sxs-lookup"><span data-stu-id="1b0e1-280">Type</span></span>|<span data-ttu-id="1b0e1-281">説明</span><span class="sxs-lookup"><span data-stu-id="1b0e1-281">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b0e1-282">assignments</span><span class="sxs-lookup"><span data-stu-id="1b0e1-282">assignments</span></span>|<span data-ttu-id="1b0e1-283">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1b0e1-283">[targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) collection</span></span>|<span data-ttu-id="1b0e1-284">ポリシーが配置される包含グループと除外グループのリストのナビゲーション プロパティです。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-284">Navigation property to list of inclusion and exclusion groups to which the policy is deployed.</span></span> <span data-ttu-id="1b0e1-285">[targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0e1-285">Inherited from [targetedManagedAppProtection](../resources/intune-mam-targetedmanagedappprotection.md)</span></span>|
|<span data-ttu-id="1b0e1-286">apps</span><span class="sxs-lookup"><span data-stu-id="1b0e1-286">apps</span></span>|<span data-ttu-id="1b0e1-287">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1b0e1-287">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="1b0e1-288">ポリシーが配置されたアプリのリスト。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-288">List of apps to which the policy is deployed.</span></span>|
|<span data-ttu-id="1b0e1-289">deploymentSummary</span><span class="sxs-lookup"><span data-stu-id="1b0e1-289">deploymentSummary</span></span>|[<span data-ttu-id="1b0e1-290">managedAppPolicyDeploymentSummary</span><span class="sxs-lookup"><span data-stu-id="1b0e1-290">managedAppPolicyDeploymentSummary</span></span>](../resources/intune-mam-managedapppolicydeploymentsummary.md)|<span data-ttu-id="1b0e1-291">構成の展開概要のナビゲーション プロパティ。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-291">Navigation property to deployment summary of the configuration.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1b0e1-292">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1b0e1-292">JSON Representation</span></span>
<span data-ttu-id="1b0e1-293">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1b0e1-293">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosManagedAppProtection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosManagedAppProtection",
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
  "minimumWarningAppVersion": "String",
  "isAssigned": true,
  "appDataEncryptionType": "String",
  "minimumRequiredSdkVersion": "String",
  "deployedAppCount": 1024,
  "faceIdBlocked": true
}
```

<!-- {
  "type": "#page.annotation",
  "suppressions": [
     "Warning: /api-reference/v1.0/resources/intune-mam-iosmanagedappprotection.md/microsoft.graph.iosManagedAppProtection/allowedDataStorageLocations:
      Inconsistent types between parameter (String) and table (Object)"
  ],
}
-->


