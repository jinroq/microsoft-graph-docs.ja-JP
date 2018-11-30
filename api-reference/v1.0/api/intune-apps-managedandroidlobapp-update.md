---
title: managedAndroidLobApp の更新
description: managedAndroidLobApp オブジェクトのプロパティを更新します。
ms.openlocfilehash: 8991efc1a3957100902a3801a284a17ee93c659a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022328"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="eeeba-103">managedAndroidLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="eeeba-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="eeeba-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="eeeba-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eeeba-105">[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="eeeba-105">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eeeba-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="eeeba-106">Prerequisites</span></span>
<span data-ttu-id="eeeba-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eeeba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eeeba-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="eeeba-109">Permission type</span></span>|<span data-ttu-id="eeeba-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="eeeba-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eeeba-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="eeeba-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eeeba-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eeeba-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="eeeba-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="eeeba-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eeeba-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeeba-114">Not supported.</span></span>|
|<span data-ttu-id="eeeba-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="eeeba-115">Application</span></span>|<span data-ttu-id="eeeba-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="eeeba-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eeeba-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="eeeba-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="eeeba-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeeba-118">Request headers</span></span>
|<span data-ttu-id="eeeba-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="eeeba-119">Header</span></span>|<span data-ttu-id="eeeba-120">値</span><span class="sxs-lookup"><span data-stu-id="eeeba-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eeeba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eeeba-121">Authorization</span></span>|<span data-ttu-id="eeeba-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="eeeba-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eeeba-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eeeba-123">Accept</span></span>|<span data-ttu-id="eeeba-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eeeba-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eeeba-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="eeeba-125">Request body</span></span>
<span data-ttu-id="eeeba-126">要求本文で、[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="eeeba-126">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="eeeba-127">次の表に、[managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="eeeba-127">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="eeeba-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="eeeba-128">Property</span></span>|<span data-ttu-id="eeeba-129">型</span><span class="sxs-lookup"><span data-stu-id="eeeba-129">Type</span></span>|<span data-ttu-id="eeeba-130">説明</span><span class="sxs-lookup"><span data-stu-id="eeeba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eeeba-131">id</span><span class="sxs-lookup"><span data-stu-id="eeeba-131">id</span></span>|<span data-ttu-id="eeeba-132">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-132">String</span></span>|<span data-ttu-id="eeeba-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="eeeba-133">Key of the entity.</span></span> <span data-ttu-id="eeeba-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-135">displayName</span><span class="sxs-lookup"><span data-stu-id="eeeba-135">displayName</span></span>|<span data-ttu-id="eeeba-136">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-136">String</span></span>|<span data-ttu-id="eeeba-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="eeeba-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="eeeba-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-139">説明</span><span class="sxs-lookup"><span data-stu-id="eeeba-139">description</span></span>|<span data-ttu-id="eeeba-140">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-140">String</span></span>|<span data-ttu-id="eeeba-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="eeeba-141">The description of the app.</span></span> <span data-ttu-id="eeeba-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-143">publisher</span><span class="sxs-lookup"><span data-stu-id="eeeba-143">publisher</span></span>|<span data-ttu-id="eeeba-144">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-144">String</span></span>|<span data-ttu-id="eeeba-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="eeeba-145">The publisher of the app.</span></span> <span data-ttu-id="eeeba-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="eeeba-147">largeIcon</span></span>|[<span data-ttu-id="eeeba-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="eeeba-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="eeeba-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="eeeba-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="eeeba-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eeeba-151">createdDateTime</span></span>|<span data-ttu-id="eeeba-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeeba-152">DateTimeOffset</span></span>|<span data-ttu-id="eeeba-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="eeeba-153">The date and time the app was created.</span></span> <span data-ttu-id="eeeba-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eeeba-155">lastModifiedDateTime</span></span>|<span data-ttu-id="eeeba-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eeeba-156">DateTimeOffset</span></span>|<span data-ttu-id="eeeba-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="eeeba-157">The date and time the app was last modified.</span></span> <span data-ttu-id="eeeba-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="eeeba-159">isFeatured</span></span>|<span data-ttu-id="eeeba-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="eeeba-160">Boolean</span></span>|<span data-ttu-id="eeeba-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="eeeba-162">privacyInformationUrl</span></span>|<span data-ttu-id="eeeba-163">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-163">String</span></span>|<span data-ttu-id="eeeba-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="eeeba-164">The privacy statement Url.</span></span> <span data-ttu-id="eeeba-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="eeeba-166">informationUrl</span></span>|<span data-ttu-id="eeeba-167">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-167">String</span></span>|<span data-ttu-id="eeeba-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="eeeba-168">The more information Url.</span></span> <span data-ttu-id="eeeba-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-170">owner</span><span class="sxs-lookup"><span data-stu-id="eeeba-170">owner</span></span>|<span data-ttu-id="eeeba-171">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-171">String</span></span>|<span data-ttu-id="eeeba-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="eeeba-172">The owner of the app.</span></span> <span data-ttu-id="eeeba-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-174">developer</span><span class="sxs-lookup"><span data-stu-id="eeeba-174">developer</span></span>|<span data-ttu-id="eeeba-175">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-175">String</span></span>|<span data-ttu-id="eeeba-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="eeeba-176">The developer of the app.</span></span> <span data-ttu-id="eeeba-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-178">notes</span><span class="sxs-lookup"><span data-stu-id="eeeba-178">notes</span></span>|<span data-ttu-id="eeeba-179">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-179">String</span></span>|<span data-ttu-id="eeeba-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="eeeba-180">Notes for the app.</span></span> <span data-ttu-id="eeeba-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="eeeba-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="eeeba-182">publishingState</span></span>|[<span data-ttu-id="eeeba-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="eeeba-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="eeeba-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="eeeba-184">The publishing state for the app.</span></span> <span data-ttu-id="eeeba-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="eeeba-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="eeeba-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="eeeba-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="eeeba-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="eeeba-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="eeeba-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="eeeba-188">appAvailability</span></span>|[<span data-ttu-id="eeeba-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="eeeba-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="eeeba-190">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="eeeba-190">The Application's availability.</span></span> <span data-ttu-id="eeeba-191">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="eeeba-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="eeeba-192">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="eeeba-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="eeeba-193">version</span><span class="sxs-lookup"><span data-stu-id="eeeba-193">version</span></span>|<span data-ttu-id="eeeba-194">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-194">String</span></span>|<span data-ttu-id="eeeba-195">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="eeeba-195">The Application's version.</span></span> <span data-ttu-id="eeeba-196">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="eeeba-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="eeeba-197">committedContentVersion</span></span>|<span data-ttu-id="eeeba-198">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-198">String</span></span>|<span data-ttu-id="eeeba-199">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="eeeba-199">The internal committed content version.</span></span> <span data-ttu-id="eeeba-200">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="eeeba-201">fileName</span><span class="sxs-lookup"><span data-stu-id="eeeba-201">fileName</span></span>|<span data-ttu-id="eeeba-202">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-202">String</span></span>|<span data-ttu-id="eeeba-203">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="eeeba-203">The name of the main Lob application file.</span></span> <span data-ttu-id="eeeba-204">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="eeeba-205">size</span><span class="sxs-lookup"><span data-stu-id="eeeba-205">size</span></span>|<span data-ttu-id="eeeba-206">Int64</span><span class="sxs-lookup"><span data-stu-id="eeeba-206">Int64</span></span>|<span data-ttu-id="eeeba-207">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="eeeba-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="eeeba-208">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="eeeba-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="eeeba-209">packageId</span><span class="sxs-lookup"><span data-stu-id="eeeba-209">packageId</span></span>|<span data-ttu-id="eeeba-210">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-210">String</span></span>|<span data-ttu-id="eeeba-211">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="eeeba-211">The package identifier.</span></span>|
|<span data-ttu-id="eeeba-212">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eeeba-212">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="eeeba-213">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="eeeba-213">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="eeeba-214">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="eeeba-214">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="eeeba-215">versionName</span><span class="sxs-lookup"><span data-stu-id="eeeba-215">versionName</span></span>|<span data-ttu-id="eeeba-216">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-216">String</span></span>|<span data-ttu-id="eeeba-217">管理対象 Android 基幹業務 (LoB) アプリのバージョン名。</span><span class="sxs-lookup"><span data-stu-id="eeeba-217">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="eeeba-218">versionCode</span><span class="sxs-lookup"><span data-stu-id="eeeba-218">versionCode</span></span>|<span data-ttu-id="eeeba-219">String</span><span class="sxs-lookup"><span data-stu-id="eeeba-219">String</span></span>|<span data-ttu-id="eeeba-220">管理対象 Android 基幹業務 (LoB) アプリのバージョン コード。</span><span class="sxs-lookup"><span data-stu-id="eeeba-220">The version code of managed Android Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="eeeba-221">応答</span><span class="sxs-lookup"><span data-stu-id="eeeba-221">Response</span></span>
<span data-ttu-id="eeeba-222">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="eeeba-222">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eeeba-223">例</span><span class="sxs-lookup"><span data-stu-id="eeeba-223">Example</span></span>
### <a name="request"></a><span data-ttu-id="eeeba-224">要求</span><span class="sxs-lookup"><span data-stu-id="eeeba-224">Request</span></span>
<span data-ttu-id="eeeba-225">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="eeeba-225">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="eeeba-226">応答</span><span class="sxs-lookup"><span data-stu-id="eeeba-226">Response</span></span>
<span data-ttu-id="eeeba-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="eeeba-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



