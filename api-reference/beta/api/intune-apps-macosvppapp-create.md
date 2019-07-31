---
title: MacOsVppApp を作成する
description: 新しい macOsVppApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3bc3acdd5250e4002a232e3cba3b31ba9e81b764
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35962044"
---
# <a name="create-macosvppapp"></a><span data-ttu-id="27cb4-103">MacOsVppApp を作成する</span><span class="sxs-lookup"><span data-stu-id="27cb4-103">Create macOsVppApp</span></span>

> <span data-ttu-id="27cb4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27cb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27cb4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="27cb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27cb4-106">新しい[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-106">Create a new [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27cb4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="27cb4-107">Prerequisites</span></span>
<span data-ttu-id="27cb4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="27cb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27cb4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="27cb4-110">Permission type</span></span>|<span data-ttu-id="27cb4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="27cb4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27cb4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="27cb4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="27cb4-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27cb4-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="27cb4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="27cb4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27cb4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27cb4-115">Not supported.</span></span>|
|<span data-ttu-id="27cb4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="27cb4-116">Application</span></span>|<span data-ttu-id="27cb4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27cb4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27cb4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="27cb4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="27cb4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27cb4-119">Request headers</span></span>
|<span data-ttu-id="27cb4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="27cb4-120">Header</span></span>|<span data-ttu-id="27cb4-121">値</span><span class="sxs-lookup"><span data-stu-id="27cb4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27cb4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="27cb4-122">Authorization</span></span>|<span data-ttu-id="27cb4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="27cb4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27cb4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="27cb4-124">Accept</span></span>|<span data-ttu-id="27cb4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="27cb4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27cb4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="27cb4-126">Request body</span></span>
<span data-ttu-id="27cb4-127">要求本文で、macOsVppApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-127">In the request body, supply a JSON representation for the macOsVppApp object.</span></span>

<span data-ttu-id="27cb4-128">次の表に、macOsVppApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-128">The following table shows the properties that are required when you create the macOsVppApp.</span></span>

|<span data-ttu-id="27cb4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27cb4-129">Property</span></span>|<span data-ttu-id="27cb4-130">型</span><span class="sxs-lookup"><span data-stu-id="27cb4-130">Type</span></span>|<span data-ttu-id="27cb4-131">説明</span><span class="sxs-lookup"><span data-stu-id="27cb4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27cb4-132">id</span><span class="sxs-lookup"><span data-stu-id="27cb4-132">id</span></span>|<span data-ttu-id="27cb4-133">文字列</span><span class="sxs-lookup"><span data-stu-id="27cb4-133">String</span></span>|<span data-ttu-id="27cb4-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="27cb4-134">Key of the entity.</span></span> <span data-ttu-id="27cb4-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="27cb4-136">displayName</span></span>|<span data-ttu-id="27cb4-137">文字列</span><span class="sxs-lookup"><span data-stu-id="27cb4-137">String</span></span>|<span data-ttu-id="27cb4-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="27cb4-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="27cb4-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-140">description</span><span class="sxs-lookup"><span data-stu-id="27cb4-140">description</span></span>|<span data-ttu-id="27cb4-141">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-141">String</span></span>|<span data-ttu-id="27cb4-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="27cb4-142">The description of the app.</span></span> <span data-ttu-id="27cb4-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-144">publisher</span><span class="sxs-lookup"><span data-stu-id="27cb4-144">publisher</span></span>|<span data-ttu-id="27cb4-145">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-145">String</span></span>|<span data-ttu-id="27cb4-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="27cb4-146">The publisher of the app.</span></span> <span data-ttu-id="27cb4-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="27cb4-148">largeIcon</span></span>|[<span data-ttu-id="27cb4-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="27cb4-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="27cb4-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="27cb4-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="27cb4-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27cb4-152">createdDateTime</span></span>|<span data-ttu-id="27cb4-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cb4-153">DateTimeOffset</span></span>|<span data-ttu-id="27cb4-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="27cb4-154">The date and time the app was created.</span></span> <span data-ttu-id="27cb4-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27cb4-156">lastModifiedDateTime</span></span>|<span data-ttu-id="27cb4-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cb4-157">DateTimeOffset</span></span>|<span data-ttu-id="27cb4-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="27cb4-158">The date and time the app was last modified.</span></span> <span data-ttu-id="27cb4-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="27cb4-160">isFeatured</span></span>|<span data-ttu-id="27cb4-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cb4-161">Boolean</span></span>|<span data-ttu-id="27cb4-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="27cb4-163">privacyInformationUrl</span></span>|<span data-ttu-id="27cb4-164">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-164">String</span></span>|<span data-ttu-id="27cb4-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="27cb4-165">The privacy statement Url.</span></span> <span data-ttu-id="27cb4-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="27cb4-167">informationUrl</span></span>|<span data-ttu-id="27cb4-168">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-168">String</span></span>|<span data-ttu-id="27cb4-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="27cb4-169">The more information Url.</span></span> <span data-ttu-id="27cb4-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-171">owner</span><span class="sxs-lookup"><span data-stu-id="27cb4-171">owner</span></span>|<span data-ttu-id="27cb4-172">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-172">String</span></span>|<span data-ttu-id="27cb4-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="27cb4-173">The owner of the app.</span></span> <span data-ttu-id="27cb4-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-175">developer</span><span class="sxs-lookup"><span data-stu-id="27cb4-175">developer</span></span>|<span data-ttu-id="27cb4-176">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-176">String</span></span>|<span data-ttu-id="27cb4-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="27cb4-177">The developer of the app.</span></span> <span data-ttu-id="27cb4-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-179">notes</span><span class="sxs-lookup"><span data-stu-id="27cb4-179">notes</span></span>|<span data-ttu-id="27cb4-180">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-180">String</span></span>|<span data-ttu-id="27cb4-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="27cb4-181">Notes for the app.</span></span> <span data-ttu-id="27cb4-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="27cb4-183">uploadState</span></span>|<span data-ttu-id="27cb4-184">Int32</span><span class="sxs-lookup"><span data-stu-id="27cb4-184">Int32</span></span>|<span data-ttu-id="27cb4-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="27cb4-185">The upload state.</span></span> <span data-ttu-id="27cb4-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="27cb4-187">publishingState</span></span>|[<span data-ttu-id="27cb4-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="27cb4-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="27cb4-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="27cb4-189">The publishing state for the app.</span></span> <span data-ttu-id="27cb4-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="27cb4-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="27cb4-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="27cb4-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="27cb4-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="27cb4-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="27cb4-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="27cb4-193">isAssigned</span></span>|<span data-ttu-id="27cb4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="27cb4-194">Boolean</span></span>|<span data-ttu-id="27cb4-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="27cb4-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="27cb4-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="27cb4-197">roleScopeTagIds</span></span>|<span data-ttu-id="27cb4-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="27cb4-198">String collection</span></span>|<span data-ttu-id="27cb4-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="27cb4-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="27cb4-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="27cb4-201">dependentAppCount</span></span>|<span data-ttu-id="27cb4-202">Int32</span><span class="sxs-lookup"><span data-stu-id="27cb4-202">Int32</span></span>|<span data-ttu-id="27cb4-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="27cb4-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="27cb4-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="27cb4-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="27cb4-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="27cb4-205">usedLicenseCount</span></span>|<span data-ttu-id="27cb4-206">Int32</span><span class="sxs-lookup"><span data-stu-id="27cb4-206">Int32</span></span>|<span data-ttu-id="27cb4-207">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="27cb4-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="27cb4-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="27cb4-208">totalLicenseCount</span></span>|<span data-ttu-id="27cb4-209">Int32</span><span class="sxs-lookup"><span data-stu-id="27cb4-209">Int32</span></span>|<span data-ttu-id="27cb4-210">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="27cb4-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="27cb4-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="27cb4-211">releaseDateTime</span></span>|<span data-ttu-id="27cb4-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27cb4-212">DateTimeOffset</span></span>|<span data-ttu-id="27cb4-213">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="27cb4-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="27cb4-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="27cb4-214">appStoreUrl</span></span>|<span data-ttu-id="27cb4-215">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-215">String</span></span>|<span data-ttu-id="27cb4-216">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="27cb4-216">The store URL.</span></span>|
|<span data-ttu-id="27cb4-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="27cb4-217">licensingType</span></span>|[<span data-ttu-id="27cb4-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="27cb4-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="27cb4-219">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="27cb4-219">The supported License Type.</span></span>|
|<span data-ttu-id="27cb4-220">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="27cb4-220">vppTokenOrganizationName</span></span>|<span data-ttu-id="27cb4-221">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-221">String</span></span>|<span data-ttu-id="27cb4-222">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="27cb4-222">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="27cb4-223">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="27cb4-223">vppTokenAccountType</span></span>|[<span data-ttu-id="27cb4-224">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="27cb4-224">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="27cb4-225">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="27cb4-225">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="27cb4-226">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="27cb4-226">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="27cb4-227">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="27cb4-227">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="27cb4-228">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="27cb4-228">vppTokenAppleId</span></span>|<span data-ttu-id="27cb4-229">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-229">String</span></span>|<span data-ttu-id="27cb4-230">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="27cb4-230">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="27cb4-231">bundleId</span><span class="sxs-lookup"><span data-stu-id="27cb4-231">bundleId</span></span>|<span data-ttu-id="27cb4-232">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="27cb4-232">String</span></span>|<span data-ttu-id="27cb4-233">ID 名。</span><span class="sxs-lookup"><span data-stu-id="27cb4-233">The Identity Name.</span></span>|
|<span data-ttu-id="27cb4-234">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="27cb4-234">vppTokenId</span></span>|<span data-ttu-id="27cb4-235">String</span><span class="sxs-lookup"><span data-stu-id="27cb4-235">String</span></span>|<span data-ttu-id="27cb4-236">このアプリに関連付けられている VPP トークンの識別子。</span><span class="sxs-lookup"><span data-stu-id="27cb4-236">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="27cb4-237">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="27cb4-237">revokeLicenseActionResults</span></span>|<span data-ttu-id="27cb4-238">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="27cb4-238">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="27cb4-239">このアプリでのライセンスの取り消しアクションの結果。</span><span class="sxs-lookup"><span data-stu-id="27cb4-239">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="27cb4-240">応答</span><span class="sxs-lookup"><span data-stu-id="27cb4-240">Response</span></span>
<span data-ttu-id="27cb4-241">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="27cb4-241">If successful, this method returns a `201 Created` response code and a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27cb4-242">例</span><span class="sxs-lookup"><span data-stu-id="27cb4-242">Example</span></span>

### <a name="request"></a><span data-ttu-id="27cb4-243">要求</span><span class="sxs-lookup"><span data-stu-id="27cb4-243">Request</span></span>
<span data-ttu-id="27cb4-244">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="27cb4-244">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1869

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="27cb4-245">応答</span><span class="sxs-lookup"><span data-stu-id="27cb4-245">Response</span></span>
<span data-ttu-id="27cb4-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="27cb4-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2041

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
    "supportUserLicensing": true,
    "supportDeviceLicensing": true,
    "supportsUserLicensing": true,
    "supportsDeviceLicensing": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
      "userId": "User Id value",
      "managedDeviceId": "Managed Device Id value",
      "totalLicensesCount": 2,
      "failedLicensesCount": 3,
      "actionFailureReason": "appleFailure",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ]
}
```





