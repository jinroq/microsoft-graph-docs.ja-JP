---
title: Create managedAndroidLobApp
description: 新しい managedAndroidLobApp オブジェクトを作成します。
ms.openlocfilehash: 0822bbc0679f1cb19ec8e4c3d217a3bf5661cdaf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023658"
---
# <a name="create-managedandroidlobapp"></a><span data-ttu-id="db1fe-103">Create managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="db1fe-103">Create managedAndroidLobApp</span></span>

> <span data-ttu-id="db1fe-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="db1fe-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db1fe-105">新しい [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="db1fe-105">Create a new [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db1fe-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="db1fe-106">Prerequisites</span></span>
<span data-ttu-id="db1fe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="db1fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db1fe-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="db1fe-109">Permission type</span></span>|<span data-ttu-id="db1fe-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="db1fe-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db1fe-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="db1fe-111">Delegated (work or school account)</span></span>|<span data-ttu-id="db1fe-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db1fe-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="db1fe-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="db1fe-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db1fe-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db1fe-114">Not supported.</span></span>|
|<span data-ttu-id="db1fe-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="db1fe-115">Application</span></span>|<span data-ttu-id="db1fe-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="db1fe-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db1fe-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="db1fe-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="db1fe-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db1fe-118">Request headers</span></span>
|<span data-ttu-id="db1fe-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="db1fe-119">Header</span></span>|<span data-ttu-id="db1fe-120">値</span><span class="sxs-lookup"><span data-stu-id="db1fe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db1fe-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db1fe-121">Authorization</span></span>|<span data-ttu-id="db1fe-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="db1fe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db1fe-123">Accept</span><span class="sxs-lookup"><span data-stu-id="db1fe-123">Accept</span></span>|<span data-ttu-id="db1fe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="db1fe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db1fe-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="db1fe-125">Request body</span></span>
<span data-ttu-id="db1fe-126">要求本文で、managedAndroidLobApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="db1fe-126">In the request body, supply a JSON representation for the managedAndroidLobApp object.</span></span>

<span data-ttu-id="db1fe-127">次の表に、managedAndroidLobApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="db1fe-127">The following table shows the properties that are required when you create the managedAndroidLobApp.</span></span>

|<span data-ttu-id="db1fe-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db1fe-128">Property</span></span>|<span data-ttu-id="db1fe-129">型</span><span class="sxs-lookup"><span data-stu-id="db1fe-129">Type</span></span>|<span data-ttu-id="db1fe-130">説明</span><span class="sxs-lookup"><span data-stu-id="db1fe-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db1fe-131">id</span><span class="sxs-lookup"><span data-stu-id="db1fe-131">id</span></span>|<span data-ttu-id="db1fe-132">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-132">String</span></span>|<span data-ttu-id="db1fe-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="db1fe-133">Key of the entity.</span></span> <span data-ttu-id="db1fe-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-135">displayName</span><span class="sxs-lookup"><span data-stu-id="db1fe-135">displayName</span></span>|<span data-ttu-id="db1fe-136">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-136">String</span></span>|<span data-ttu-id="db1fe-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="db1fe-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="db1fe-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-139">説明</span><span class="sxs-lookup"><span data-stu-id="db1fe-139">description</span></span>|<span data-ttu-id="db1fe-140">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-140">String</span></span>|<span data-ttu-id="db1fe-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="db1fe-141">The description of the app.</span></span> <span data-ttu-id="db1fe-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-143">publisher</span><span class="sxs-lookup"><span data-stu-id="db1fe-143">publisher</span></span>|<span data-ttu-id="db1fe-144">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-144">String</span></span>|<span data-ttu-id="db1fe-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="db1fe-145">The publisher of the app.</span></span> <span data-ttu-id="db1fe-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="db1fe-147">largeIcon</span></span>|[<span data-ttu-id="db1fe-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="db1fe-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="db1fe-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="db1fe-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="db1fe-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="db1fe-151">createdDateTime</span></span>|<span data-ttu-id="db1fe-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db1fe-152">DateTimeOffset</span></span>|<span data-ttu-id="db1fe-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="db1fe-153">The date and time the app was created.</span></span> <span data-ttu-id="db1fe-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="db1fe-155">lastModifiedDateTime</span></span>|<span data-ttu-id="db1fe-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="db1fe-156">DateTimeOffset</span></span>|<span data-ttu-id="db1fe-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="db1fe-157">The date and time the app was last modified.</span></span> <span data-ttu-id="db1fe-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="db1fe-159">isFeatured</span></span>|<span data-ttu-id="db1fe-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="db1fe-160">Boolean</span></span>|<span data-ttu-id="db1fe-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="db1fe-162">privacyInformationUrl</span></span>|<span data-ttu-id="db1fe-163">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-163">String</span></span>|<span data-ttu-id="db1fe-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="db1fe-164">The privacy statement Url.</span></span> <span data-ttu-id="db1fe-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="db1fe-166">informationUrl</span></span>|<span data-ttu-id="db1fe-167">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-167">String</span></span>|<span data-ttu-id="db1fe-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="db1fe-168">The more information Url.</span></span> <span data-ttu-id="db1fe-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-170">owner</span><span class="sxs-lookup"><span data-stu-id="db1fe-170">owner</span></span>|<span data-ttu-id="db1fe-171">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-171">String</span></span>|<span data-ttu-id="db1fe-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="db1fe-172">The owner of the app.</span></span> <span data-ttu-id="db1fe-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-174">developer</span><span class="sxs-lookup"><span data-stu-id="db1fe-174">developer</span></span>|<span data-ttu-id="db1fe-175">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-175">String</span></span>|<span data-ttu-id="db1fe-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="db1fe-176">The developer of the app.</span></span> <span data-ttu-id="db1fe-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-178">notes</span><span class="sxs-lookup"><span data-stu-id="db1fe-178">notes</span></span>|<span data-ttu-id="db1fe-179">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-179">String</span></span>|<span data-ttu-id="db1fe-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="db1fe-180">Notes for the app.</span></span> <span data-ttu-id="db1fe-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="db1fe-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="db1fe-182">publishingState</span></span>|[<span data-ttu-id="db1fe-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="db1fe-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="db1fe-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="db1fe-184">The publishing state for the app.</span></span> <span data-ttu-id="db1fe-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="db1fe-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="db1fe-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="db1fe-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="db1fe-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="db1fe-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="db1fe-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="db1fe-188">appAvailability</span></span>|[<span data-ttu-id="db1fe-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="db1fe-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="db1fe-190">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="db1fe-190">The Application's availability.</span></span> <span data-ttu-id="db1fe-191">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="db1fe-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="db1fe-192">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="db1fe-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="db1fe-193">version</span><span class="sxs-lookup"><span data-stu-id="db1fe-193">version</span></span>|<span data-ttu-id="db1fe-194">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-194">String</span></span>|<span data-ttu-id="db1fe-195">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="db1fe-195">The Application's version.</span></span> <span data-ttu-id="db1fe-196">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="db1fe-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="db1fe-197">committedContentVersion</span></span>|<span data-ttu-id="db1fe-198">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-198">String</span></span>|<span data-ttu-id="db1fe-199">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="db1fe-199">The internal committed content version.</span></span> <span data-ttu-id="db1fe-200">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="db1fe-201">fileName</span><span class="sxs-lookup"><span data-stu-id="db1fe-201">fileName</span></span>|<span data-ttu-id="db1fe-202">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-202">String</span></span>|<span data-ttu-id="db1fe-203">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="db1fe-203">The name of the main Lob application file.</span></span> <span data-ttu-id="db1fe-204">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="db1fe-205">size</span><span class="sxs-lookup"><span data-stu-id="db1fe-205">size</span></span>|<span data-ttu-id="db1fe-206">Int64</span><span class="sxs-lookup"><span data-stu-id="db1fe-206">Int64</span></span>|<span data-ttu-id="db1fe-207">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="db1fe-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="db1fe-208">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="db1fe-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="db1fe-209">packageId</span><span class="sxs-lookup"><span data-stu-id="db1fe-209">packageId</span></span>|<span data-ttu-id="db1fe-210">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-210">String</span></span>|<span data-ttu-id="db1fe-211">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="db1fe-211">The package identifier.</span></span>|
|<span data-ttu-id="db1fe-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="db1fe-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="db1fe-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="db1fe-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="db1fe-214">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="db1fe-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="db1fe-215">versionName</span><span class="sxs-lookup"><span data-stu-id="db1fe-215">versionName</span></span>|<span data-ttu-id="db1fe-216">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-216">String</span></span>|<span data-ttu-id="db1fe-217">管理対象 Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="db1fe-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="db1fe-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="db1fe-218">versionCode</span></span>|<span data-ttu-id="db1fe-219">String</span><span class="sxs-lookup"><span data-stu-id="db1fe-219">String</span></span>|<span data-ttu-id="db1fe-220">管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="db1fe-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="db1fe-221">応答</span><span class="sxs-lookup"><span data-stu-id="db1fe-221">Response</span></span>
<span data-ttu-id="db1fe-222">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="db1fe-222">If successful, this method returns a `201 Created` response code and a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db1fe-223">例</span><span class="sxs-lookup"><span data-stu-id="db1fe-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="db1fe-224">要求</span><span class="sxs-lookup"><span data-stu-id="db1fe-224">Request</span></span>
<span data-ttu-id="db1fe-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="db1fe-225">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1153

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```

### <a name="response"></a><span data-ttu-id="db1fe-226">応答</span><span class="sxs-lookup"><span data-stu-id="db1fe-226">Response</span></span>
<span data-ttu-id="db1fe-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="db1fe-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1325

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value"
}
```



