---
title: androidmanagedstoreapp の作成
description: 新しい androidmanagedstoreapp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7b69c5f734e5609b17dc76057d85278ac60fbfac
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970304"
---
# <a name="create-androidmanagedstoreapp"></a><span data-ttu-id="80a5f-103">androidmanagedstoreapp の作成</span><span class="sxs-lookup"><span data-stu-id="80a5f-103">Create androidManagedStoreApp</span></span>

> <span data-ttu-id="80a5f-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80a5f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="80a5f-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="80a5f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80a5f-106">新しい[androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="80a5f-106">Create a new [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80a5f-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="80a5f-107">Prerequisites</span></span>
<span data-ttu-id="80a5f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="80a5f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80a5f-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="80a5f-110">Permission type</span></span>|<span data-ttu-id="80a5f-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="80a5f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80a5f-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="80a5f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80a5f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80a5f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="80a5f-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="80a5f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80a5f-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80a5f-115">Not supported.</span></span>|
|<span data-ttu-id="80a5f-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="80a5f-116">Application</span></span>|<span data-ttu-id="80a5f-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="80a5f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80a5f-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="80a5f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="80a5f-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80a5f-119">Request headers</span></span>
|<span data-ttu-id="80a5f-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="80a5f-120">Header</span></span>|<span data-ttu-id="80a5f-121">値</span><span class="sxs-lookup"><span data-stu-id="80a5f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80a5f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="80a5f-122">Authorization</span></span>|<span data-ttu-id="80a5f-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="80a5f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80a5f-124">承諾</span><span class="sxs-lookup"><span data-stu-id="80a5f-124">Accept</span></span>|<span data-ttu-id="80a5f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80a5f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80a5f-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="80a5f-126">Request body</span></span>
<span data-ttu-id="80a5f-127">要求本文で、androidmanagedstoreapp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="80a5f-127">In the request body, supply a JSON representation for the androidManagedStoreApp object.</span></span>

<span data-ttu-id="80a5f-128">次の表に、androidmanagedstoreapp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="80a5f-128">The following table shows the properties that are required when you create the androidManagedStoreApp.</span></span>

|<span data-ttu-id="80a5f-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="80a5f-129">Property</span></span>|<span data-ttu-id="80a5f-130">型</span><span class="sxs-lookup"><span data-stu-id="80a5f-130">Type</span></span>|<span data-ttu-id="80a5f-131">説明</span><span class="sxs-lookup"><span data-stu-id="80a5f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80a5f-132">id</span><span class="sxs-lookup"><span data-stu-id="80a5f-132">id</span></span>|<span data-ttu-id="80a5f-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="80a5f-133">String</span></span>|<span data-ttu-id="80a5f-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="80a5f-134">Key of the entity.</span></span> <span data-ttu-id="80a5f-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="80a5f-136">displayName</span></span>|<span data-ttu-id="80a5f-137">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-137">String</span></span>|<span data-ttu-id="80a5f-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="80a5f-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="80a5f-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-140">description</span><span class="sxs-lookup"><span data-stu-id="80a5f-140">description</span></span>|<span data-ttu-id="80a5f-141">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-141">String</span></span>|<span data-ttu-id="80a5f-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="80a5f-142">The description of the app.</span></span> <span data-ttu-id="80a5f-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-144">publisher</span><span class="sxs-lookup"><span data-stu-id="80a5f-144">publisher</span></span>|<span data-ttu-id="80a5f-145">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-145">String</span></span>|<span data-ttu-id="80a5f-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="80a5f-146">The publisher of the app.</span></span> <span data-ttu-id="80a5f-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="80a5f-148">largeIcon</span></span>|[<span data-ttu-id="80a5f-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="80a5f-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="80a5f-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="80a5f-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="80a5f-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80a5f-152">createdDateTime</span></span>|<span data-ttu-id="80a5f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a5f-153">DateTimeOffset</span></span>|<span data-ttu-id="80a5f-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="80a5f-154">The date and time the app was created.</span></span> <span data-ttu-id="80a5f-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80a5f-156">lastModifiedDateTime</span></span>|<span data-ttu-id="80a5f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a5f-157">DateTimeOffset</span></span>|<span data-ttu-id="80a5f-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="80a5f-158">The date and time the app was last modified.</span></span> <span data-ttu-id="80a5f-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="80a5f-160">isFeatured</span></span>|<span data-ttu-id="80a5f-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a5f-161">Boolean</span></span>|<span data-ttu-id="80a5f-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="80a5f-163">privacyInformationUrl</span></span>|<span data-ttu-id="80a5f-164">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-164">String</span></span>|<span data-ttu-id="80a5f-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="80a5f-165">The privacy statement Url.</span></span> <span data-ttu-id="80a5f-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="80a5f-167">informationUrl</span></span>|<span data-ttu-id="80a5f-168">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-168">String</span></span>|<span data-ttu-id="80a5f-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="80a5f-169">The more information Url.</span></span> <span data-ttu-id="80a5f-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-171">owner</span><span class="sxs-lookup"><span data-stu-id="80a5f-171">owner</span></span>|<span data-ttu-id="80a5f-172">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-172">String</span></span>|<span data-ttu-id="80a5f-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="80a5f-173">The owner of the app.</span></span> <span data-ttu-id="80a5f-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-175">developer</span><span class="sxs-lookup"><span data-stu-id="80a5f-175">developer</span></span>|<span data-ttu-id="80a5f-176">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-176">String</span></span>|<span data-ttu-id="80a5f-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="80a5f-177">The developer of the app.</span></span> <span data-ttu-id="80a5f-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-179">notes</span><span class="sxs-lookup"><span data-stu-id="80a5f-179">notes</span></span>|<span data-ttu-id="80a5f-180">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-180">String</span></span>|<span data-ttu-id="80a5f-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="80a5f-181">Notes for the app.</span></span> <span data-ttu-id="80a5f-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="80a5f-183">uploadState</span></span>|<span data-ttu-id="80a5f-184">Int32</span><span class="sxs-lookup"><span data-stu-id="80a5f-184">Int32</span></span>|<span data-ttu-id="80a5f-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="80a5f-185">The upload state.</span></span> <span data-ttu-id="80a5f-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="80a5f-187">publishingState</span></span>|[<span data-ttu-id="80a5f-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="80a5f-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="80a5f-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="80a5f-189">The publishing state for the app.</span></span> <span data-ttu-id="80a5f-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="80a5f-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="80a5f-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="80a5f-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="80a5f-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="80a5f-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="80a5f-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="80a5f-193">isAssigned</span></span>|<span data-ttu-id="80a5f-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a5f-194">Boolean</span></span>|<span data-ttu-id="80a5f-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="80a5f-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="80a5f-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="80a5f-197">roleScopeTagIds</span></span>|<span data-ttu-id="80a5f-198">String collection</span><span class="sxs-lookup"><span data-stu-id="80a5f-198">String collection</span></span>|<span data-ttu-id="80a5f-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="80a5f-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="80a5f-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="80a5f-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="80a5f-201">packageId</span><span class="sxs-lookup"><span data-stu-id="80a5f-201">packageId</span></span>|<span data-ttu-id="80a5f-202">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="80a5f-202">String</span></span>|<span data-ttu-id="80a5f-203">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="80a5f-203">The package identifier.</span></span>|
|<span data-ttu-id="80a5f-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="80a5f-204">appIdentifier</span></span>|<span data-ttu-id="80a5f-205">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-205">String</span></span>|<span data-ttu-id="80a5f-206">ID 名。</span><span class="sxs-lookup"><span data-stu-id="80a5f-206">The Identity Name.</span></span>|
|<span data-ttu-id="80a5f-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="80a5f-207">usedLicenseCount</span></span>|<span data-ttu-id="80a5f-208">Int32</span><span class="sxs-lookup"><span data-stu-id="80a5f-208">Int32</span></span>|<span data-ttu-id="80a5f-209">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="80a5f-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="80a5f-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="80a5f-210">totalLicenseCount</span></span>|<span data-ttu-id="80a5f-211">Int32</span><span class="sxs-lookup"><span data-stu-id="80a5f-211">Int32</span></span>|<span data-ttu-id="80a5f-212">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="80a5f-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="80a5f-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="80a5f-213">appStoreUrl</span></span>|<span data-ttu-id="80a5f-214">String</span><span class="sxs-lookup"><span data-stu-id="80a5f-214">String</span></span>|<span data-ttu-id="80a5f-215">ワークストアアプリの URL を再生します。</span><span class="sxs-lookup"><span data-stu-id="80a5f-215">The Play for Work Store app URL.</span></span>|
|<span data-ttu-id="80a5f-216">supportsoemconfig</span><span class="sxs-lookup"><span data-stu-id="80a5f-216">supportsOemConfig</span></span>|<span data-ttu-id="80a5f-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a5f-217">Boolean</span></span>|<span data-ttu-id="80a5f-218">このアプリが oemconfig ポリシーをサポートするかどうか。</span><span class="sxs-lookup"><span data-stu-id="80a5f-218">Whether this app supports OEMConfig policy.</span></span>|



## <a name="response"></a><span data-ttu-id="80a5f-219">応答</span><span class="sxs-lookup"><span data-stu-id="80a5f-219">Response</span></span>
<span data-ttu-id="80a5f-220">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidmanagedstoreapp](../resources/intune-apps-androidmanagedstoreapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="80a5f-220">If successful, this method returns a `201 Created` response code and a [androidManagedStoreApp](../resources/intune-apps-androidmanagedstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80a5f-221">例</span><span class="sxs-lookup"><span data-stu-id="80a5f-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="80a5f-222">要求</span><span class="sxs-lookup"><span data-stu-id="80a5f-222">Request</span></span>
<span data-ttu-id="80a5f-223">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="80a5f-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 911

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```

### <a name="response"></a><span data-ttu-id="80a5f-224">応答</span><span class="sxs-lookup"><span data-stu-id="80a5f-224">Response</span></span>
<span data-ttu-id="80a5f-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="80a5f-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1083

{
  "@odata.type": "#microsoft.graph.androidManagedStoreApp",
  "id": "87247525-7525-8724-2575-248725752487",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "supportsOemConfig": true
}
```




