---
title: androidStoreApp の作成
description: 新しい androidStoreApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4e2fc78d02ac0afc367cd9d5d8b43331cd2744b9
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34965215"
---
# <a name="create-androidstoreapp"></a><span data-ttu-id="0b542-103">androidStoreApp の作成</span><span class="sxs-lookup"><span data-stu-id="0b542-103">Create androidStoreApp</span></span>

> <span data-ttu-id="0b542-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b542-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b542-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b542-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b542-106">新しい [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0b542-106">Create a new [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0b542-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0b542-107">Prerequisites</span></span>
<span data-ttu-id="0b542-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0b542-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b542-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0b542-110">Permission type</span></span>|<span data-ttu-id="0b542-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0b542-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b542-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0b542-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0b542-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b542-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b542-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0b542-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b542-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b542-115">Not supported.</span></span>|
|<span data-ttu-id="0b542-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0b542-116">Application</span></span>|<span data-ttu-id="0b542-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0b542-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b542-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0b542-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0b542-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b542-119">Request headers</span></span>
|<span data-ttu-id="0b542-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b542-120">Header</span></span>|<span data-ttu-id="0b542-121">値</span><span class="sxs-lookup"><span data-stu-id="0b542-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b542-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b542-122">Authorization</span></span>|<span data-ttu-id="0b542-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0b542-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0b542-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0b542-124">Accept</span></span>|<span data-ttu-id="0b542-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0b542-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b542-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0b542-126">Request body</span></span>
<span data-ttu-id="0b542-127">要求本文で、androidStoreApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0b542-127">In the request body, supply a JSON representation for the androidStoreApp object.</span></span>

<span data-ttu-id="0b542-128">次の表に、androidStoreApp の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0b542-128">The following table shows the properties that are required when you create the androidStoreApp.</span></span>

|<span data-ttu-id="0b542-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0b542-129">Property</span></span>|<span data-ttu-id="0b542-130">型</span><span class="sxs-lookup"><span data-stu-id="0b542-130">Type</span></span>|<span data-ttu-id="0b542-131">説明</span><span class="sxs-lookup"><span data-stu-id="0b542-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b542-132">id</span><span class="sxs-lookup"><span data-stu-id="0b542-132">id</span></span>|<span data-ttu-id="0b542-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0b542-133">String</span></span>|<span data-ttu-id="0b542-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0b542-134">Key of the entity.</span></span> <span data-ttu-id="0b542-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0b542-136">displayName</span></span>|<span data-ttu-id="0b542-137">文字列</span><span class="sxs-lookup"><span data-stu-id="0b542-137">String</span></span>|<span data-ttu-id="0b542-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="0b542-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="0b542-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-140">description</span><span class="sxs-lookup"><span data-stu-id="0b542-140">description</span></span>|<span data-ttu-id="0b542-141">String</span><span class="sxs-lookup"><span data-stu-id="0b542-141">String</span></span>|<span data-ttu-id="0b542-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="0b542-142">The description of the app.</span></span> <span data-ttu-id="0b542-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-144">publisher</span><span class="sxs-lookup"><span data-stu-id="0b542-144">publisher</span></span>|<span data-ttu-id="0b542-145">String</span><span class="sxs-lookup"><span data-stu-id="0b542-145">String</span></span>|<span data-ttu-id="0b542-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="0b542-146">The publisher of the app.</span></span> <span data-ttu-id="0b542-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="0b542-148">largeIcon</span></span>|[<span data-ttu-id="0b542-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="0b542-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="0b542-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="0b542-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="0b542-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0b542-152">createdDateTime</span></span>|<span data-ttu-id="0b542-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b542-153">DateTimeOffset</span></span>|<span data-ttu-id="0b542-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="0b542-154">The date and time the app was created.</span></span> <span data-ttu-id="0b542-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0b542-156">lastModifiedDateTime</span></span>|<span data-ttu-id="0b542-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0b542-157">DateTimeOffset</span></span>|<span data-ttu-id="0b542-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0b542-158">The date and time the app was last modified.</span></span> <span data-ttu-id="0b542-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="0b542-160">isFeatured</span></span>|<span data-ttu-id="0b542-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b542-161">Boolean</span></span>|<span data-ttu-id="0b542-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="0b542-163">privacyInformationUrl</span></span>|<span data-ttu-id="0b542-164">String</span><span class="sxs-lookup"><span data-stu-id="0b542-164">String</span></span>|<span data-ttu-id="0b542-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="0b542-165">The privacy statement Url.</span></span> <span data-ttu-id="0b542-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="0b542-167">informationUrl</span></span>|<span data-ttu-id="0b542-168">String</span><span class="sxs-lookup"><span data-stu-id="0b542-168">String</span></span>|<span data-ttu-id="0b542-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="0b542-169">The more information Url.</span></span> <span data-ttu-id="0b542-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-171">owner</span><span class="sxs-lookup"><span data-stu-id="0b542-171">owner</span></span>|<span data-ttu-id="0b542-172">String</span><span class="sxs-lookup"><span data-stu-id="0b542-172">String</span></span>|<span data-ttu-id="0b542-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="0b542-173">The owner of the app.</span></span> <span data-ttu-id="0b542-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-175">developer</span><span class="sxs-lookup"><span data-stu-id="0b542-175">developer</span></span>|<span data-ttu-id="0b542-176">String</span><span class="sxs-lookup"><span data-stu-id="0b542-176">String</span></span>|<span data-ttu-id="0b542-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="0b542-177">The developer of the app.</span></span> <span data-ttu-id="0b542-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-179">notes</span><span class="sxs-lookup"><span data-stu-id="0b542-179">notes</span></span>|<span data-ttu-id="0b542-180">String</span><span class="sxs-lookup"><span data-stu-id="0b542-180">String</span></span>|<span data-ttu-id="0b542-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="0b542-181">Notes for the app.</span></span> <span data-ttu-id="0b542-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="0b542-183">uploadState</span></span>|<span data-ttu-id="0b542-184">Int32</span><span class="sxs-lookup"><span data-stu-id="0b542-184">Int32</span></span>|<span data-ttu-id="0b542-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="0b542-185">The upload state.</span></span> <span data-ttu-id="0b542-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="0b542-187">publishingState</span></span>|[<span data-ttu-id="0b542-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="0b542-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="0b542-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="0b542-189">The publishing state for the app.</span></span> <span data-ttu-id="0b542-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="0b542-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="0b542-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0b542-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="0b542-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="0b542-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="0b542-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="0b542-193">isAssigned</span></span>|<span data-ttu-id="0b542-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b542-194">Boolean</span></span>|<span data-ttu-id="0b542-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="0b542-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="0b542-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0b542-197">roleScopeTagIds</span></span>|<span data-ttu-id="0b542-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0b542-198">String collection</span></span>|<span data-ttu-id="0b542-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="0b542-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="0b542-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="0b542-201">dependentAppCount</span></span>|<span data-ttu-id="0b542-202">Int32</span><span class="sxs-lookup"><span data-stu-id="0b542-202">Int32</span></span>|<span data-ttu-id="0b542-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="0b542-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="0b542-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0b542-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="0b542-205">packageId</span><span class="sxs-lookup"><span data-stu-id="0b542-205">packageId</span></span>|<span data-ttu-id="0b542-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="0b542-206">String</span></span>|<span data-ttu-id="0b542-207">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="0b542-207">The package identifier.</span></span>|
|<span data-ttu-id="0b542-208">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="0b542-208">appIdentifier</span></span>|<span data-ttu-id="0b542-209">String</span><span class="sxs-lookup"><span data-stu-id="0b542-209">String</span></span>|<span data-ttu-id="0b542-210">ID 名。</span><span class="sxs-lookup"><span data-stu-id="0b542-210">The Identity Name.</span></span>|
|<span data-ttu-id="0b542-211">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="0b542-211">appStoreUrl</span></span>|<span data-ttu-id="0b542-212">String</span><span class="sxs-lookup"><span data-stu-id="0b542-212">String</span></span>|<span data-ttu-id="0b542-213">Android アプリ ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="0b542-213">The Android app store URL.</span></span>|
|<span data-ttu-id="0b542-214">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0b542-214">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="0b542-215">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="0b542-215">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="0b542-216">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="0b542-216">The value for the minimum applicable operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="0b542-217">応答</span><span class="sxs-lookup"><span data-stu-id="0b542-217">Response</span></span>
<span data-ttu-id="0b542-218">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidStoreApp](../resources/intune-apps-androidstoreapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0b542-218">If successful, this method returns a `201 Created` response code and a [androidStoreApp](../resources/intune-apps-androidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b542-219">例</span><span class="sxs-lookup"><span data-stu-id="0b542-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="0b542-220">要求</span><span class="sxs-lookup"><span data-stu-id="0b542-220">Request</span></span>
<span data-ttu-id="0b542-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0b542-221">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0b542-222">応答</span><span class="sxs-lookup"><span data-stu-id="0b542-222">Response</span></span>
<span data-ttu-id="0b542-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0b542-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





