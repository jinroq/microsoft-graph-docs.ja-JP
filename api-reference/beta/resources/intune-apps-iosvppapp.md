---
title: iosVppApp リソース タイプ
description: iOS ボリューム購入プログラム (VPP) アプリのプロパティと継承されたプロパティが含まれます。
author: tfitzmac
ms.openlocfilehash: 565bcf04bb7a5b903060c6492000377fdefeb495
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27333167"
---
# <a name="iosvppapp-resource-type"></a><span data-ttu-id="e7d1c-103">iosVppApp リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="e7d1c-103">iosVppApp resource type</span></span>

> <span data-ttu-id="e7d1c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e7d1c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e7d1c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7d1c-107">iOS ボリューム購入プログラム (VPP) アプリのプロパティと継承されたプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-107">Contains properties and inherited properties for iOS Volume-Purchased Program (VPP) Apps.</span></span>

<span data-ttu-id="e7d1c-108">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-108">Inherits from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e7d1c-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7d1c-109">Methods</span></span>
|<span data-ttu-id="e7d1c-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="e7d1c-110">Method</span></span>|<span data-ttu-id="e7d1c-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e7d1c-111">Return Type</span></span>|<span data-ttu-id="e7d1c-112">説明</span><span class="sxs-lookup"><span data-stu-id="e7d1c-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e7d1c-113">List iosVppApps</span><span class="sxs-lookup"><span data-stu-id="e7d1c-113">List iosVppApps</span></span>](../api/intune-apps-iosvppapp-list.md)|<span data-ttu-id="e7d1c-114">[iosVppApp](../resources/intune-apps-iosvppapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-114">[iosVppApp](../resources/intune-apps-iosvppapp.md) collection</span></span>|<span data-ttu-id="e7d1c-115">[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-115">List properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) objects.</span></span>|
|[<span data-ttu-id="e7d1c-116">Get iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e7d1c-116">Get iosVppApp</span></span>](../api/intune-apps-iosvppapp-get.md)|[<span data-ttu-id="e7d1c-117">iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e7d1c-117">iosVppApp</span></span>](../resources/intune-apps-iosvppapp.md)|<span data-ttu-id="e7d1c-118">[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-118">Read properties and relationships of the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>|
|[<span data-ttu-id="e7d1c-119">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e7d1c-119">Create iosVppApp</span></span>](../api/intune-apps-iosvppapp-create.md)|[<span data-ttu-id="e7d1c-120">iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e7d1c-120">iosVppApp</span></span>](../resources/intune-apps-iosvppapp.md)|<span data-ttu-id="e7d1c-121">新しい [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-121">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>|
|[<span data-ttu-id="e7d1c-122">Delete iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e7d1c-122">Delete iosVppApp</span></span>](../api/intune-apps-iosvppapp-delete.md)|<span data-ttu-id="e7d1c-123">なし</span><span class="sxs-lookup"><span data-stu-id="e7d1c-123">None</span></span>|<span data-ttu-id="e7d1c-124">[iosVppApp](../resources/intune-apps-iosvppapp.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-124">Deletes a [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>|
|[<span data-ttu-id="e7d1c-125">Update iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e7d1c-125">Update iosVppApp</span></span>](../api/intune-apps-iosvppapp-update.md)|[<span data-ttu-id="e7d1c-126">iosVppApp</span><span class="sxs-lookup"><span data-stu-id="e7d1c-126">iosVppApp</span></span>](../resources/intune-apps-iosvppapp.md)|<span data-ttu-id="e7d1c-127">[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-127">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>|
|[<span data-ttu-id="e7d1c-128">revokeAllLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-128">revokeAllLicenses action</span></span>](../api/intune-apps-iosvppapp-revokealllicenses.md)|<span data-ttu-id="e7d1c-129">なし</span><span class="sxs-lookup"><span data-stu-id="e7d1c-129">None</span></span>|<span data-ttu-id="e7d1c-130">VPP は割り当てられているすべて取り消し iOS のアプリケーションが指定されているライセンスです。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-130">Revoke all assigned iOS VPP licenses for given app.</span></span>|
|[<span data-ttu-id="e7d1c-131">revokeUserLicense アクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-131">revokeUserLicense action</span></span>](../api/intune-apps-iosvppapp-revokeuserlicense.md)|<span data-ttu-id="e7d1c-132">なし</span><span class="sxs-lookup"><span data-stu-id="e7d1c-132">None</span></span>|<span data-ttu-id="e7d1c-133">Revoke が割り当てられている iOS VPP ユーザー ライセンスは、アプリケーションを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-133">Revoke assigned iOS VPP user license for given app.</span></span>|
|[<span data-ttu-id="e7d1c-134">revokeDeviceLicense アクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-134">revokeDeviceLicense action</span></span>](../api/intune-apps-iosvppapp-revokedevicelicense.md)|<span data-ttu-id="e7d1c-135">なし</span><span class="sxs-lookup"><span data-stu-id="e7d1c-135">None</span></span>|<span data-ttu-id="e7d1c-136">取り消しが割り当てられている iOS の VPP デバイスのライセンスは、アプリケーションを指定します。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-136">Revoke assigned iOS VPP device license for given app.</span></span>|

## <a name="properties"></a><span data-ttu-id="e7d1c-137">Properties</span><span class="sxs-lookup"><span data-stu-id="e7d1c-137">Properties</span></span>
|<span data-ttu-id="e7d1c-138">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7d1c-138">Property</span></span>|<span data-ttu-id="e7d1c-139">種類</span><span class="sxs-lookup"><span data-stu-id="e7d1c-139">Type</span></span>|<span data-ttu-id="e7d1c-140">説明</span><span class="sxs-lookup"><span data-stu-id="e7d1c-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d1c-141">ID</span><span class="sxs-lookup"><span data-stu-id="e7d1c-141">id</span></span>|<span data-ttu-id="e7d1c-142">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-142">String</span></span>|<span data-ttu-id="e7d1c-143">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-143">Key of the entity.</span></span> <span data-ttu-id="e7d1c-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e7d1c-145">displayName</span></span>|<span data-ttu-id="e7d1c-146">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-146">String</span></span>|<span data-ttu-id="e7d1c-147">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-147">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e7d1c-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-149">説明</span><span class="sxs-lookup"><span data-stu-id="e7d1c-149">description</span></span>|<span data-ttu-id="e7d1c-150">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-150">String</span></span>|<span data-ttu-id="e7d1c-151">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-151">The description of the app.</span></span> <span data-ttu-id="e7d1c-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-153">publisher</span><span class="sxs-lookup"><span data-stu-id="e7d1c-153">publisher</span></span>|<span data-ttu-id="e7d1c-154">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-154">String</span></span>|<span data-ttu-id="e7d1c-155">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-155">The publisher of the app.</span></span> <span data-ttu-id="e7d1c-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-157">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e7d1c-157">largeIcon</span></span>|[<span data-ttu-id="e7d1c-158">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e7d1c-158">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e7d1c-159">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-159">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e7d1c-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-161">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d1c-161">createdDateTime</span></span>|<span data-ttu-id="e7d1c-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7d1c-162">DateTimeOffset</span></span>|<span data-ttu-id="e7d1c-163">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-163">The date and time the app was created.</span></span> <span data-ttu-id="e7d1c-164">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-164">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-165">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d1c-165">lastModifiedDateTime</span></span>|<span data-ttu-id="e7d1c-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7d1c-166">DateTimeOffset</span></span>|<span data-ttu-id="e7d1c-167">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-167">The date and time the app was last modified.</span></span> <span data-ttu-id="e7d1c-168">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-168">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-169">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e7d1c-169">isFeatured</span></span>|<span data-ttu-id="e7d1c-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7d1c-170">Boolean</span></span>|<span data-ttu-id="e7d1c-171">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-171">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-172">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e7d1c-172">privacyInformationUrl</span></span>|<span data-ttu-id="e7d1c-173">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-173">String</span></span>|<span data-ttu-id="e7d1c-174">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-174">The privacy statement Url.</span></span> <span data-ttu-id="e7d1c-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-176">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e7d1c-176">informationUrl</span></span>|<span data-ttu-id="e7d1c-177">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-177">String</span></span>|<span data-ttu-id="e7d1c-178">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-178">The more information Url.</span></span> <span data-ttu-id="e7d1c-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-180">owner</span><span class="sxs-lookup"><span data-stu-id="e7d1c-180">owner</span></span>|<span data-ttu-id="e7d1c-181">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-181">String</span></span>|<span data-ttu-id="e7d1c-182">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-182">The owner of the app.</span></span> <span data-ttu-id="e7d1c-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-184">developer</span><span class="sxs-lookup"><span data-stu-id="e7d1c-184">developer</span></span>|<span data-ttu-id="e7d1c-185">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-185">String</span></span>|<span data-ttu-id="e7d1c-186">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-186">The developer of the app.</span></span> <span data-ttu-id="e7d1c-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-188">notes</span><span class="sxs-lookup"><span data-stu-id="e7d1c-188">notes</span></span>|<span data-ttu-id="e7d1c-189">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-189">String</span></span>|<span data-ttu-id="e7d1c-190">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-190">Notes for the app.</span></span> <span data-ttu-id="e7d1c-191">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-192">uploadState</span><span class="sxs-lookup"><span data-stu-id="e7d1c-192">uploadState</span></span>|<span data-ttu-id="e7d1c-193">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d1c-193">Int32</span></span>|<span data-ttu-id="e7d1c-194">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-194">The upload state.</span></span> <span data-ttu-id="e7d1c-195">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-195">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-196">publishingState</span><span class="sxs-lookup"><span data-stu-id="e7d1c-196">publishingState</span></span>|[<span data-ttu-id="e7d1c-197">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e7d1c-197">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e7d1c-198">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-198">The publishing state for the app.</span></span> <span data-ttu-id="e7d1c-199">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-199">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e7d1c-200">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e7d1c-201">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-201">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e7d1c-202">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e7d1c-202">usedLicenseCount</span></span>|<span data-ttu-id="e7d1c-203">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d1c-203">Int32</span></span>|<span data-ttu-id="e7d1c-204">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-204">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="e7d1c-205">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e7d1c-205">totalLicenseCount</span></span>|<span data-ttu-id="e7d1c-206">Int32</span><span class="sxs-lookup"><span data-stu-id="e7d1c-206">Int32</span></span>|<span data-ttu-id="e7d1c-207">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-207">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="e7d1c-208">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="e7d1c-208">releaseDateTime</span></span>|<span data-ttu-id="e7d1c-209">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7d1c-209">DateTimeOffset</span></span>|<span data-ttu-id="e7d1c-210">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-210">The VPP application release date and time.</span></span>|
|<span data-ttu-id="e7d1c-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e7d1c-211">appStoreUrl</span></span>|<span data-ttu-id="e7d1c-212">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-212">String</span></span>|<span data-ttu-id="e7d1c-213">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-213">The store URL.</span></span>|
|<span data-ttu-id="e7d1c-214">licensingType</span><span class="sxs-lookup"><span data-stu-id="e7d1c-214">licensingType</span></span>|[<span data-ttu-id="e7d1c-215">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="e7d1c-215">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="e7d1c-216">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-216">The supported License Type.</span></span>|
|<span data-ttu-id="e7d1c-217">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="e7d1c-217">applicableDeviceType</span></span>|[<span data-ttu-id="e7d1c-218">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="e7d1c-218">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="e7d1c-219">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-219">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="e7d1c-220">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="e7d1c-220">vppTokenOrganizationName</span></span>|<span data-ttu-id="e7d1c-221">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-221">String</span></span>|<span data-ttu-id="e7d1c-222">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="e7d1c-222">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="e7d1c-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="e7d1c-223">vppTokenAccountType</span></span>|[<span data-ttu-id="e7d1c-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="e7d1c-224">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="e7d1c-225">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-225">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="e7d1c-226">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-226">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="e7d1c-227">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-227">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="e7d1c-228">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="e7d1c-228">vppTokenAppleId</span></span>|<span data-ttu-id="e7d1c-229">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-229">String</span></span>|<span data-ttu-id="e7d1c-230">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-230">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="e7d1c-231">bundleId</span><span class="sxs-lookup"><span data-stu-id="e7d1c-231">bundleId</span></span>|<span data-ttu-id="e7d1c-232">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-232">String</span></span>|<span data-ttu-id="e7d1c-233">ID 名。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-233">The Identity Name.</span></span>|
|<span data-ttu-id="e7d1c-234">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="e7d1c-234">vppTokenId</span></span>|<span data-ttu-id="e7d1c-235">String</span><span class="sxs-lookup"><span data-stu-id="e7d1c-235">String</span></span>|<span data-ttu-id="e7d1c-236">このアプリケーションに関連付けられている VPP トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-236">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="e7d1c-237">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="e7d1c-237">revokeLicenseActionResults</span></span>|<span data-ttu-id="e7d1c-238">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-238">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="e7d1c-239">結果は、このアプリケーションについてのライセンスを失効します。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-239">Results of revoke license actions on this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e7d1c-240">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7d1c-240">Relationships</span></span>
|<span data-ttu-id="e7d1c-241">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e7d1c-241">Relationship</span></span>|<span data-ttu-id="e7d1c-242">型</span><span class="sxs-lookup"><span data-stu-id="e7d1c-242">Type</span></span>|<span data-ttu-id="e7d1c-243">説明</span><span class="sxs-lookup"><span data-stu-id="e7d1c-243">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7d1c-244">categories</span><span class="sxs-lookup"><span data-stu-id="e7d1c-244">categories</span></span>|<span data-ttu-id="e7d1c-245">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-245">[mobileAppCategory](../resources/intune-apps-mobileappcategory.md) collection</span></span>|<span data-ttu-id="e7d1c-246">このアプリのカテゴリのリスト。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-246">The list of categories for this app.</span></span> <span data-ttu-id="e7d1c-247">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-247">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-248">assignments</span><span class="sxs-lookup"><span data-stu-id="e7d1c-248">assignments</span></span>|<span data-ttu-id="e7d1c-249">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-249">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) collection</span></span>|<span data-ttu-id="e7d1c-250">このモバイル アプリのグループ割り当てのリスト。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-250">The list of group assignments for this mobile app.</span></span> <span data-ttu-id="e7d1c-251">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-251">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-252">installSummary</span><span class="sxs-lookup"><span data-stu-id="e7d1c-252">installSummary</span></span>|[<span data-ttu-id="e7d1c-253">mobileAppInstallSummary</span><span class="sxs-lookup"><span data-stu-id="e7d1c-253">mobileAppInstallSummary</span></span>](../resources/intune-apps-mobileappinstallsummary.md)|<span data-ttu-id="e7d1c-254">モバイル アプリ インストール概要です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-254">Mobile App Install Summary.</span></span> <span data-ttu-id="e7d1c-255">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-255">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-256">deviceStatuses</span><span class="sxs-lookup"><span data-stu-id="e7d1c-256">deviceStatuses</span></span>|<span data-ttu-id="e7d1c-257">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-257">[mobileAppInstallStatus](../resources/intune-apps-mobileappinstallstatus.md) collection</span></span>|<span data-ttu-id="e7d1c-258">このモバイル アプリケーションのインストール状況の一覧です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-258">The list of installation states for this mobile app.</span></span> <span data-ttu-id="e7d1c-259">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-259">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-260">userStatuses</span><span class="sxs-lookup"><span data-stu-id="e7d1c-260">userStatuses</span></span>|<span data-ttu-id="e7d1c-261">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-261">[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) collection</span></span>|<span data-ttu-id="e7d1c-262">このモバイル アプリケーションのインストール状況の一覧です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-262">The list of installation states for this mobile app.</span></span> <span data-ttu-id="e7d1c-263">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e7d1c-263">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e7d1c-264">assignedLicenses</span><span class="sxs-lookup"><span data-stu-id="e7d1c-264">assignedLicenses</span></span>|<span data-ttu-id="e7d1c-265">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e7d1c-265">[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) collection</span></span>|<span data-ttu-id="e7d1c-266">このアプリケーションに割り当てられているライセンスです。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-266">The licenses assigned to this app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e7d1c-267">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e7d1c-267">JSON Representation</span></span>
<span data-ttu-id="e7d1c-268">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e7d1c-268">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "publisher": "String",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "isFeatured": true,
  "privacyInformationUrl": "String",
  "informationUrl": "String",
  "owner": "String",
  "developer": "String",
  "notes": "String",
  "uploadState": 1024,
  "publishingState": "String",
  "usedLicenseCount": 1024,
  "totalLicenseCount": 1024,
  "releaseDateTime": "String (timestamp)",
  "appStoreUrl": "String",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "String",
  "vppTokenAccountType": "String",
  "vppTokenAppleId": "String",
  "bundleId": "String",
  "vppTokenId": "String",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
      "userId": "String",
      "managedDeviceId": "String",
      "totalLicensesCount": 1024,
      "failedLicensesCount": 1024,
      "actionFailureReason": "String",
      "actionName": "String",
      "actionState": "String",
      "startDateTime": "String (timestamp)",
      "lastUpdatedDateTime": "String (timestamp)"
    }
  ]
}
```




