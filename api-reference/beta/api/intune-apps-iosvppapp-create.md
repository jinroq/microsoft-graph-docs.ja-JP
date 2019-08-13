---
title: Create iosVppApp
description: 新しい iosVppApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 74204610a9d46a339a1b99623bd2d553a6cc17a3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36330553"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="b82b1-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="b82b1-103">Create iosVppApp</span></span>

> <span data-ttu-id="b82b1-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b82b1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b82b1-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b82b1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b82b1-106">新しい [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b82b1-106">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b82b1-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b82b1-107">Prerequisites</span></span>
<span data-ttu-id="b82b1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b82b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b82b1-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b82b1-110">Permission type</span></span>|<span data-ttu-id="b82b1-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b82b1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b82b1-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b82b1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b82b1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b82b1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b82b1-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b82b1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b82b1-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b82b1-115">Not supported.</span></span>|
|<span data-ttu-id="b82b1-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b82b1-116">Application</span></span>|<span data-ttu-id="b82b1-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b82b1-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b82b1-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b82b1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b82b1-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b82b1-119">Request headers</span></span>
|<span data-ttu-id="b82b1-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b82b1-120">Header</span></span>|<span data-ttu-id="b82b1-121">値</span><span class="sxs-lookup"><span data-stu-id="b82b1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b82b1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b82b1-122">Authorization</span></span>|<span data-ttu-id="b82b1-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b82b1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b82b1-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b82b1-124">Accept</span></span>|<span data-ttu-id="b82b1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b82b1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b82b1-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b82b1-126">Request body</span></span>
<span data-ttu-id="b82b1-127">要求本文で、iosVppApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b82b1-127">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="b82b1-128">次の表に、iosVppApp 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b82b1-128">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="b82b1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b82b1-129">Property</span></span>|<span data-ttu-id="b82b1-130">型</span><span class="sxs-lookup"><span data-stu-id="b82b1-130">Type</span></span>|<span data-ttu-id="b82b1-131">説明</span><span class="sxs-lookup"><span data-stu-id="b82b1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b82b1-132">id</span><span class="sxs-lookup"><span data-stu-id="b82b1-132">id</span></span>|<span data-ttu-id="b82b1-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b82b1-133">String</span></span>|<span data-ttu-id="b82b1-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b82b1-134">Key of the entity.</span></span> <span data-ttu-id="b82b1-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b82b1-136">displayName</span></span>|<span data-ttu-id="b82b1-137">文字列</span><span class="sxs-lookup"><span data-stu-id="b82b1-137">String</span></span>|<span data-ttu-id="b82b1-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="b82b1-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b82b1-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-140">description</span><span class="sxs-lookup"><span data-stu-id="b82b1-140">description</span></span>|<span data-ttu-id="b82b1-141">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-141">String</span></span>|<span data-ttu-id="b82b1-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b82b1-142">The description of the app.</span></span> <span data-ttu-id="b82b1-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b82b1-144">publisher</span></span>|<span data-ttu-id="b82b1-145">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-145">String</span></span>|<span data-ttu-id="b82b1-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="b82b1-146">The publisher of the app.</span></span> <span data-ttu-id="b82b1-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b82b1-148">largeIcon</span></span>|[<span data-ttu-id="b82b1-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b82b1-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b82b1-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="b82b1-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b82b1-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b82b1-152">createdDateTime</span></span>|<span data-ttu-id="b82b1-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b82b1-153">DateTimeOffset</span></span>|<span data-ttu-id="b82b1-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b82b1-154">The date and time the app was created.</span></span> <span data-ttu-id="b82b1-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b82b1-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b82b1-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b82b1-157">DateTimeOffset</span></span>|<span data-ttu-id="b82b1-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b82b1-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b82b1-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b82b1-160">isFeatured</span></span>|<span data-ttu-id="b82b1-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b82b1-161">Boolean</span></span>|<span data-ttu-id="b82b1-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b82b1-163">privacyInformationUrl</span></span>|<span data-ttu-id="b82b1-164">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-164">String</span></span>|<span data-ttu-id="b82b1-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="b82b1-165">The privacy statement Url.</span></span> <span data-ttu-id="b82b1-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b82b1-167">informationUrl</span></span>|<span data-ttu-id="b82b1-168">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-168">String</span></span>|<span data-ttu-id="b82b1-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="b82b1-169">The more information Url.</span></span> <span data-ttu-id="b82b1-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-171">owner</span><span class="sxs-lookup"><span data-stu-id="b82b1-171">owner</span></span>|<span data-ttu-id="b82b1-172">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-172">String</span></span>|<span data-ttu-id="b82b1-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="b82b1-173">The owner of the app.</span></span> <span data-ttu-id="b82b1-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-175">developer</span><span class="sxs-lookup"><span data-stu-id="b82b1-175">developer</span></span>|<span data-ttu-id="b82b1-176">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-176">String</span></span>|<span data-ttu-id="b82b1-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="b82b1-177">The developer of the app.</span></span> <span data-ttu-id="b82b1-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-179">notes</span><span class="sxs-lookup"><span data-stu-id="b82b1-179">notes</span></span>|<span data-ttu-id="b82b1-180">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-180">String</span></span>|<span data-ttu-id="b82b1-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="b82b1-181">Notes for the app.</span></span> <span data-ttu-id="b82b1-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b82b1-183">uploadState</span></span>|<span data-ttu-id="b82b1-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b82b1-184">Int32</span></span>|<span data-ttu-id="b82b1-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="b82b1-185">The upload state.</span></span> <span data-ttu-id="b82b1-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b82b1-187">publishingState</span></span>|[<span data-ttu-id="b82b1-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b82b1-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b82b1-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="b82b1-189">The publishing state for the app.</span></span> <span data-ttu-id="b82b1-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="b82b1-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b82b1-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b82b1-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b82b1-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="b82b1-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b82b1-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b82b1-193">isAssigned</span></span>|<span data-ttu-id="b82b1-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b82b1-194">Boolean</span></span>|<span data-ttu-id="b82b1-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="b82b1-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b82b1-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b82b1-197">roleScopeTagIds</span></span>|<span data-ttu-id="b82b1-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="b82b1-198">String collection</span></span>|<span data-ttu-id="b82b1-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="b82b1-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b82b1-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b82b1-201">dependentAppCount</span></span>|<span data-ttu-id="b82b1-202">Int32</span><span class="sxs-lookup"><span data-stu-id="b82b1-202">Int32</span></span>|<span data-ttu-id="b82b1-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="b82b1-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="b82b1-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b82b1-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b82b1-205">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b82b1-205">usedLicenseCount</span></span>|<span data-ttu-id="b82b1-206">Int32</span><span class="sxs-lookup"><span data-stu-id="b82b1-206">Int32</span></span>|<span data-ttu-id="b82b1-207">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="b82b1-207">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="b82b1-208">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="b82b1-208">totalLicenseCount</span></span>|<span data-ttu-id="b82b1-209">Int32</span><span class="sxs-lookup"><span data-stu-id="b82b1-209">Int32</span></span>|<span data-ttu-id="b82b1-210">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="b82b1-210">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="b82b1-211">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="b82b1-211">releaseDateTime</span></span>|<span data-ttu-id="b82b1-212">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b82b1-212">DateTimeOffset</span></span>|<span data-ttu-id="b82b1-213">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="b82b1-213">The VPP application release date and time.</span></span>|
|<span data-ttu-id="b82b1-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b82b1-214">appStoreUrl</span></span>|<span data-ttu-id="b82b1-215">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-215">String</span></span>|<span data-ttu-id="b82b1-216">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="b82b1-216">The store URL.</span></span>|
|<span data-ttu-id="b82b1-217">licensingType</span><span class="sxs-lookup"><span data-stu-id="b82b1-217">licensingType</span></span>|[<span data-ttu-id="b82b1-218">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="b82b1-218">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="b82b1-219">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="b82b1-219">The supported License Type.</span></span>|
|<span data-ttu-id="b82b1-220">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="b82b1-220">applicableDeviceType</span></span>|[<span data-ttu-id="b82b1-221">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="b82b1-221">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="b82b1-222">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="b82b1-222">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="b82b1-223">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="b82b1-223">vppTokenOrganizationName</span></span>|<span data-ttu-id="b82b1-224">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-224">String</span></span>|<span data-ttu-id="b82b1-225">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="b82b1-225">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="b82b1-226">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b82b1-226">vppTokenAccountType</span></span>|[<span data-ttu-id="b82b1-227">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="b82b1-227">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="b82b1-228">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="b82b1-228">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="b82b1-229">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="b82b1-229">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="b82b1-230">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="b82b1-230">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="b82b1-231">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="b82b1-231">vppTokenAppleId</span></span>|<span data-ttu-id="b82b1-232">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-232">String</span></span>|<span data-ttu-id="b82b1-233">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="b82b1-233">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="b82b1-234">bundleId</span><span class="sxs-lookup"><span data-stu-id="b82b1-234">bundleId</span></span>|<span data-ttu-id="b82b1-235">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b82b1-235">String</span></span>|<span data-ttu-id="b82b1-236">ID 名。</span><span class="sxs-lookup"><span data-stu-id="b82b1-236">The Identity Name.</span></span>|
|<span data-ttu-id="b82b1-237">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="b82b1-237">vppTokenId</span></span>|<span data-ttu-id="b82b1-238">String</span><span class="sxs-lookup"><span data-stu-id="b82b1-238">String</span></span>|<span data-ttu-id="b82b1-239">このアプリに関連付けられている VPP トークンの識別子。</span><span class="sxs-lookup"><span data-stu-id="b82b1-239">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="b82b1-240">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="b82b1-240">revokeLicenseActionResults</span></span>|<span data-ttu-id="b82b1-241">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b82b1-241">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="b82b1-242">このアプリでのライセンスの取り消しアクションの結果。</span><span class="sxs-lookup"><span data-stu-id="b82b1-242">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="b82b1-243">応答</span><span class="sxs-lookup"><span data-stu-id="b82b1-243">Response</span></span>
<span data-ttu-id="b82b1-244">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b82b1-244">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b82b1-245">例</span><span class="sxs-lookup"><span data-stu-id="b82b1-245">Example</span></span>

### <a name="request"></a><span data-ttu-id="b82b1-246">要求</span><span class="sxs-lookup"><span data-stu-id="b82b1-246">Request</span></span>
<span data-ttu-id="b82b1-247">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b82b1-247">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1999

{
  "@odata.type": "#microsoft.graph.iosVppApp",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
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

### <a name="response"></a><span data-ttu-id="b82b1-248">応答</span><span class="sxs-lookup"><span data-stu-id="b82b1-248">Response</span></span>
<span data-ttu-id="b82b1-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b82b1-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2171

{
  "@odata.type": "#microsoft.graph.iosVppApp",
  "id": "a0ac9b6f-9b6f-a0ac-6f9b-aca06f9baca0",
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
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.iosVppAppRevokeLicensesActionResult",
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






