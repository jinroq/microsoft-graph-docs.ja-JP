---
title: Androidforwork アプリの作成
description: 新しい Androidforwork App オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2c0f589e7955ae5f5663f83ec26b327eea9100a5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952465"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="e79c2-103">Androidforwork アプリの作成</span><span class="sxs-lookup"><span data-stu-id="e79c2-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="e79c2-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e79c2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e79c2-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e79c2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e79c2-106">新しい[Androidforwork app](../resources/intune-apps-androidforworkapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e79c2-106">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e79c2-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e79c2-107">Prerequisites</span></span>
<span data-ttu-id="e79c2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e79c2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e79c2-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e79c2-110">Permission type</span></span>|<span data-ttu-id="e79c2-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e79c2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e79c2-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e79c2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e79c2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e79c2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e79c2-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e79c2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e79c2-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e79c2-115">Not supported.</span></span>|
|<span data-ttu-id="e79c2-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e79c2-116">Application</span></span>|<span data-ttu-id="e79c2-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e79c2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e79c2-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e79c2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="e79c2-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e79c2-119">Request headers</span></span>
|<span data-ttu-id="e79c2-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e79c2-120">Header</span></span>|<span data-ttu-id="e79c2-121">値</span><span class="sxs-lookup"><span data-stu-id="e79c2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e79c2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e79c2-122">Authorization</span></span>|<span data-ttu-id="e79c2-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e79c2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e79c2-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e79c2-124">Accept</span></span>|<span data-ttu-id="e79c2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e79c2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e79c2-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e79c2-126">Request body</span></span>
<span data-ttu-id="e79c2-127">要求本文で、Androidforwork App オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e79c2-127">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="e79c2-128">次の表に、Androidforwork アプリの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e79c2-128">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="e79c2-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e79c2-129">Property</span></span>|<span data-ttu-id="e79c2-130">型</span><span class="sxs-lookup"><span data-stu-id="e79c2-130">Type</span></span>|<span data-ttu-id="e79c2-131">説明</span><span class="sxs-lookup"><span data-stu-id="e79c2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e79c2-132">id</span><span class="sxs-lookup"><span data-stu-id="e79c2-132">id</span></span>|<span data-ttu-id="e79c2-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e79c2-133">String</span></span>|<span data-ttu-id="e79c2-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e79c2-134">Key of the entity.</span></span> <span data-ttu-id="e79c2-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e79c2-136">displayName</span></span>|<span data-ttu-id="e79c2-137">文字列</span><span class="sxs-lookup"><span data-stu-id="e79c2-137">String</span></span>|<span data-ttu-id="e79c2-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="e79c2-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="e79c2-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-140">description</span><span class="sxs-lookup"><span data-stu-id="e79c2-140">description</span></span>|<span data-ttu-id="e79c2-141">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-141">String</span></span>|<span data-ttu-id="e79c2-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="e79c2-142">The description of the app.</span></span> <span data-ttu-id="e79c2-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-144">publisher</span><span class="sxs-lookup"><span data-stu-id="e79c2-144">publisher</span></span>|<span data-ttu-id="e79c2-145">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-145">String</span></span>|<span data-ttu-id="e79c2-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="e79c2-146">The publisher of the app.</span></span> <span data-ttu-id="e79c2-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="e79c2-148">largeIcon</span></span>|[<span data-ttu-id="e79c2-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="e79c2-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="e79c2-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="e79c2-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="e79c2-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e79c2-152">createdDateTime</span></span>|<span data-ttu-id="e79c2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e79c2-153">DateTimeOffset</span></span>|<span data-ttu-id="e79c2-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e79c2-154">The date and time the app was created.</span></span> <span data-ttu-id="e79c2-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e79c2-156">lastModifiedDateTime</span></span>|<span data-ttu-id="e79c2-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e79c2-157">DateTimeOffset</span></span>|<span data-ttu-id="e79c2-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="e79c2-158">The date and time the app was last modified.</span></span> <span data-ttu-id="e79c2-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="e79c2-160">isFeatured</span></span>|<span data-ttu-id="e79c2-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="e79c2-161">Boolean</span></span>|<span data-ttu-id="e79c2-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="e79c2-163">privacyInformationUrl</span></span>|<span data-ttu-id="e79c2-164">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-164">String</span></span>|<span data-ttu-id="e79c2-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="e79c2-165">The privacy statement Url.</span></span> <span data-ttu-id="e79c2-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="e79c2-167">informationUrl</span></span>|<span data-ttu-id="e79c2-168">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-168">String</span></span>|<span data-ttu-id="e79c2-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="e79c2-169">The more information Url.</span></span> <span data-ttu-id="e79c2-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-171">owner</span><span class="sxs-lookup"><span data-stu-id="e79c2-171">owner</span></span>|<span data-ttu-id="e79c2-172">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-172">String</span></span>|<span data-ttu-id="e79c2-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="e79c2-173">The owner of the app.</span></span> <span data-ttu-id="e79c2-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-175">developer</span><span class="sxs-lookup"><span data-stu-id="e79c2-175">developer</span></span>|<span data-ttu-id="e79c2-176">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-176">String</span></span>|<span data-ttu-id="e79c2-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="e79c2-177">The developer of the app.</span></span> <span data-ttu-id="e79c2-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-179">notes</span><span class="sxs-lookup"><span data-stu-id="e79c2-179">notes</span></span>|<span data-ttu-id="e79c2-180">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-180">String</span></span>|<span data-ttu-id="e79c2-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="e79c2-181">Notes for the app.</span></span> <span data-ttu-id="e79c2-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="e79c2-183">uploadState</span></span>|<span data-ttu-id="e79c2-184">Int32</span><span class="sxs-lookup"><span data-stu-id="e79c2-184">Int32</span></span>|<span data-ttu-id="e79c2-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="e79c2-185">The upload state.</span></span> <span data-ttu-id="e79c2-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="e79c2-187">publishingState</span></span>|[<span data-ttu-id="e79c2-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="e79c2-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="e79c2-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="e79c2-189">The publishing state for the app.</span></span> <span data-ttu-id="e79c2-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="e79c2-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="e79c2-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="e79c2-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="e79c2-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="e79c2-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="e79c2-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="e79c2-193">isAssigned</span></span>|<span data-ttu-id="e79c2-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e79c2-194">Boolean</span></span>|<span data-ttu-id="e79c2-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="e79c2-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="e79c2-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e79c2-197">roleScopeTagIds</span></span>|<span data-ttu-id="e79c2-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="e79c2-198">String collection</span></span>|<span data-ttu-id="e79c2-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="e79c2-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="e79c2-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="e79c2-201">dependentAppCount</span></span>|<span data-ttu-id="e79c2-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e79c2-202">Int32</span></span>|<span data-ttu-id="e79c2-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="e79c2-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="e79c2-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e79c2-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="e79c2-205">packageId</span><span class="sxs-lookup"><span data-stu-id="e79c2-205">packageId</span></span>|<span data-ttu-id="e79c2-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e79c2-206">String</span></span>|<span data-ttu-id="e79c2-207">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="e79c2-207">The package identifier.</span></span>|
|<span data-ttu-id="e79c2-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="e79c2-208">appIdentifier</span></span>|<span data-ttu-id="e79c2-209">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-209">String</span></span>|<span data-ttu-id="e79c2-210">ID 名。</span><span class="sxs-lookup"><span data-stu-id="e79c2-210">The Identity Name.</span></span>|
|<span data-ttu-id="e79c2-211">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e79c2-211">usedLicenseCount</span></span>|<span data-ttu-id="e79c2-212">Int32</span><span class="sxs-lookup"><span data-stu-id="e79c2-212">Int32</span></span>|<span data-ttu-id="e79c2-213">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="e79c2-213">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="e79c2-214">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="e79c2-214">totalLicenseCount</span></span>|<span data-ttu-id="e79c2-215">Int32</span><span class="sxs-lookup"><span data-stu-id="e79c2-215">Int32</span></span>|<span data-ttu-id="e79c2-216">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="e79c2-216">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="e79c2-217">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="e79c2-217">appStoreUrl</span></span>|<span data-ttu-id="e79c2-218">String</span><span class="sxs-lookup"><span data-stu-id="e79c2-218">String</span></span>|<span data-ttu-id="e79c2-219">ワークストアアプリの URL を再生します。</span><span class="sxs-lookup"><span data-stu-id="e79c2-219">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="e79c2-220">応答</span><span class="sxs-lookup"><span data-stu-id="e79c2-220">Response</span></span>
<span data-ttu-id="e79c2-221">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Androidforwork app](../resources/intune-apps-androidforworkapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e79c2-221">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e79c2-222">例</span><span class="sxs-lookup"><span data-stu-id="e79c2-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="e79c2-223">要求</span><span class="sxs-lookup"><span data-stu-id="e79c2-223">Request</span></span>
<span data-ttu-id="e79c2-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e79c2-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 903

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="e79c2-225">応答</span><span class="sxs-lookup"><span data-stu-id="e79c2-225">Response</span></span>
<span data-ttu-id="e79c2-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e79c2-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1075

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "dependentAppCount": 1,
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```





