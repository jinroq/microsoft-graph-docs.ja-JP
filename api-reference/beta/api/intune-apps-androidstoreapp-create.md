---
title: androidStoreApp の作成
description: 新しい androidStoreApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a85a3c0fbf163f35dc0b9d88546d65d1c5acf9c0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952108"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="83dea-103">androidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="83dea-103">Create androidStoreApp</span></span>

> <span data-ttu-id="83dea-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83dea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83dea-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="83dea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83dea-106">新しい [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="83dea-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83dea-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="83dea-107">Prerequisites</span></span>
<span data-ttu-id="83dea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83dea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83dea-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83dea-110">Permission type</span></span>|<span data-ttu-id="83dea-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="83dea-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83dea-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83dea-112">Delegated (work or school account)</span></span>|<span data-ttu-id="83dea-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83dea-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83dea-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83dea-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83dea-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83dea-115">Not supported.</span></span>|
|<span data-ttu-id="83dea-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83dea-116">Application</span></span>|<span data-ttu-id="83dea-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83dea-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83dea-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83dea-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="83dea-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83dea-119">Request headers</span></span>
|<span data-ttu-id="83dea-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83dea-120">Header</span></span>|<span data-ttu-id="83dea-121">値</span><span class="sxs-lookup"><span data-stu-id="83dea-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83dea-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="83dea-122">Authorization</span></span>|<span data-ttu-id="83dea-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="83dea-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83dea-124">承諾</span><span class="sxs-lookup"><span data-stu-id="83dea-124">Accept</span></span>|<span data-ttu-id="83dea-125">application/json</span><span class="sxs-lookup"><span data-stu-id="83dea-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83dea-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="83dea-126">Request body</span></span>
<span data-ttu-id="83dea-127">要求本文で、androidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="83dea-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="83dea-128">次の表に、androidStoreApp の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="83dea-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="83dea-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="83dea-129">Property</span></span>|<span data-ttu-id="83dea-130">型</span><span class="sxs-lookup"><span data-stu-id="83dea-130">Type</span></span>|<span data-ttu-id="83dea-131">説明</span><span class="sxs-lookup"><span data-stu-id="83dea-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83dea-132">id</span><span class="sxs-lookup"><span data-stu-id="83dea-132">id</span></span>|<span data-ttu-id="83dea-133">文字列</span><span class="sxs-lookup"><span data-stu-id="83dea-133">String</span></span>|<span data-ttu-id="83dea-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="83dea-134">Key of the entity.</span></span> <span data-ttu-id="83dea-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-136">displayName</span><span class="sxs-lookup"><span data-stu-id="83dea-136">displayName</span></span>|<span data-ttu-id="83dea-137">文字列</span><span class="sxs-lookup"><span data-stu-id="83dea-137">String</span></span>|<span data-ttu-id="83dea-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="83dea-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="83dea-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-140">description</span><span class="sxs-lookup"><span data-stu-id="83dea-140">description</span></span>|<span data-ttu-id="83dea-141">String</span><span class="sxs-lookup"><span data-stu-id="83dea-141">String</span></span>|<span data-ttu-id="83dea-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="83dea-142">The description of the app.</span></span> <span data-ttu-id="83dea-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-144">publisher</span><span class="sxs-lookup"><span data-stu-id="83dea-144">publisher</span></span>|<span data-ttu-id="83dea-145">String</span><span class="sxs-lookup"><span data-stu-id="83dea-145">String</span></span>|<span data-ttu-id="83dea-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="83dea-146">The publisher of the app.</span></span> <span data-ttu-id="83dea-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="83dea-148">largeIcon</span></span>|[<span data-ttu-id="83dea-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="83dea-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="83dea-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="83dea-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="83dea-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="83dea-152">createdDateTime</span></span>|<span data-ttu-id="83dea-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83dea-153">DateTimeOffset</span></span>|<span data-ttu-id="83dea-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="83dea-154">The date and time the app was created.</span></span> <span data-ttu-id="83dea-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83dea-156">lastModifiedDateTime</span></span>|<span data-ttu-id="83dea-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="83dea-157">DateTimeOffset</span></span>|<span data-ttu-id="83dea-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="83dea-158">The date and time the app was last modified.</span></span> <span data-ttu-id="83dea-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="83dea-160">isFeatured</span></span>|<span data-ttu-id="83dea-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="83dea-161">Boolean</span></span>|<span data-ttu-id="83dea-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="83dea-163">privacyInformationUrl</span></span>|<span data-ttu-id="83dea-164">String</span><span class="sxs-lookup"><span data-stu-id="83dea-164">String</span></span>|<span data-ttu-id="83dea-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="83dea-165">The privacy statement Url.</span></span> <span data-ttu-id="83dea-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="83dea-167">informationUrl</span></span>|<span data-ttu-id="83dea-168">String</span><span class="sxs-lookup"><span data-stu-id="83dea-168">String</span></span>|<span data-ttu-id="83dea-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="83dea-169">The more information Url.</span></span> <span data-ttu-id="83dea-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-171">owner</span><span class="sxs-lookup"><span data-stu-id="83dea-171">owner</span></span>|<span data-ttu-id="83dea-172">String</span><span class="sxs-lookup"><span data-stu-id="83dea-172">String</span></span>|<span data-ttu-id="83dea-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="83dea-173">The owner of the app.</span></span> <span data-ttu-id="83dea-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-175">developer</span><span class="sxs-lookup"><span data-stu-id="83dea-175">developer</span></span>|<span data-ttu-id="83dea-176">String</span><span class="sxs-lookup"><span data-stu-id="83dea-176">String</span></span>|<span data-ttu-id="83dea-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="83dea-177">The developer of the app.</span></span> <span data-ttu-id="83dea-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-179">notes</span><span class="sxs-lookup"><span data-stu-id="83dea-179">notes</span></span>|<span data-ttu-id="83dea-180">String</span><span class="sxs-lookup"><span data-stu-id="83dea-180">String</span></span>|<span data-ttu-id="83dea-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="83dea-181">Notes for the app.</span></span> <span data-ttu-id="83dea-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="83dea-183">uploadState</span></span>|<span data-ttu-id="83dea-184">Int32</span><span class="sxs-lookup"><span data-stu-id="83dea-184">Int32</span></span>|<span data-ttu-id="83dea-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="83dea-185">The upload state.</span></span> <span data-ttu-id="83dea-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="83dea-187">publishingState</span></span>|[<span data-ttu-id="83dea-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="83dea-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="83dea-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="83dea-189">The publishing state for the app.</span></span> <span data-ttu-id="83dea-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="83dea-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="83dea-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="83dea-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="83dea-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="83dea-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="83dea-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="83dea-193">isAssigned</span></span>|<span data-ttu-id="83dea-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="83dea-194">Boolean</span></span>|<span data-ttu-id="83dea-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="83dea-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="83dea-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="83dea-197">roleScopeTagIds</span></span>|<span data-ttu-id="83dea-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="83dea-198">String collection</span></span>|<span data-ttu-id="83dea-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="83dea-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="83dea-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="83dea-201">dependentAppCount</span></span>|<span data-ttu-id="83dea-202">Int32</span><span class="sxs-lookup"><span data-stu-id="83dea-202">Int32</span></span>|<span data-ttu-id="83dea-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="83dea-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="83dea-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="83dea-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="83dea-205">packageId</span><span class="sxs-lookup"><span data-stu-id="83dea-205">packageId</span></span>|<span data-ttu-id="83dea-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="83dea-206">String</span></span>|<span data-ttu-id="83dea-207">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="83dea-207">The package identifier.</span></span>|
|<span data-ttu-id="83dea-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="83dea-208">appIdentifier</span></span>|<span data-ttu-id="83dea-209">String</span><span class="sxs-lookup"><span data-stu-id="83dea-209">String</span></span>|<span data-ttu-id="83dea-210">ID 名。</span><span class="sxs-lookup"><span data-stu-id="83dea-210">The Identity Name.</span></span>|
|<span data-ttu-id="83dea-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="83dea-211">appStoreUrl</span></span>|<span data-ttu-id="83dea-212">String</span><span class="sxs-lookup"><span data-stu-id="83dea-212">String</span></span>|<span data-ttu-id="83dea-213">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="83dea-213">The Android app store URL.</span></span>|
|<span data-ttu-id="83dea-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="83dea-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="83dea-215">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="83dea-215">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="83dea-216">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="83dea-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="83dea-217">応答</span><span class="sxs-lookup"><span data-stu-id="83dea-217">Response</span></span>
<span data-ttu-id="83dea-218">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="83dea-218">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83dea-219">例</span><span class="sxs-lookup"><span data-stu-id="83dea-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="83dea-220">要求</span><span class="sxs-lookup"><span data-stu-id="83dea-220">Request</span></span>
<span data-ttu-id="83dea-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83dea-221">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1230

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```

### <a name="response"></a><span data-ttu-id="83dea-222">応答</span><span class="sxs-lookup"><span data-stu-id="83dea-222">Response</span></span>
<span data-ttu-id="83dea-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83dea-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1402

{
  "@odata.type": "#microsoft.graph.androidStoreApp",
  "id": "1f2b7654-7654-1f2b-5476-2b1f54762b1f",
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
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  }
}
```





