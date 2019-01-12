---
title: managedIOSLobApp の更新
description: managedIOSLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 209c9be20b3fd1b6a3c96161e4f36b49215d28b8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971439"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="69184-103">managedIOSLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="69184-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="69184-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="69184-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69184-105">[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="69184-105">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="69184-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="69184-106">Prerequisites</span></span>
<span data-ttu-id="69184-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="69184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="69184-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="69184-109">Permission type</span></span>|<span data-ttu-id="69184-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="69184-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69184-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="69184-111">Delegated (work or school account)</span></span>|<span data-ttu-id="69184-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="69184-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="69184-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="69184-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69184-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69184-114">Not supported.</span></span>|
|<span data-ttu-id="69184-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="69184-115">Application</span></span>|<span data-ttu-id="69184-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="69184-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69184-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="69184-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="69184-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69184-118">Request headers</span></span>
|<span data-ttu-id="69184-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="69184-119">Header</span></span>|<span data-ttu-id="69184-120">値</span><span class="sxs-lookup"><span data-stu-id="69184-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69184-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="69184-121">Authorization</span></span>|<span data-ttu-id="69184-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="69184-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69184-123">Accept</span><span class="sxs-lookup"><span data-stu-id="69184-123">Accept</span></span>|<span data-ttu-id="69184-124">application/json</span><span class="sxs-lookup"><span data-stu-id="69184-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69184-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="69184-125">Request body</span></span>
<span data-ttu-id="69184-126">要求本文で、[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="69184-126">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="69184-127">次の表に、[managedDeviceOverview](../resources/intune-apps-managedioslobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="69184-127">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="69184-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="69184-128">Property</span></span>|<span data-ttu-id="69184-129">種類</span><span class="sxs-lookup"><span data-stu-id="69184-129">Type</span></span>|<span data-ttu-id="69184-130">説明</span><span class="sxs-lookup"><span data-stu-id="69184-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69184-131">ID</span><span class="sxs-lookup"><span data-stu-id="69184-131">id</span></span>|<span data-ttu-id="69184-132">String</span><span class="sxs-lookup"><span data-stu-id="69184-132">String</span></span>|<span data-ttu-id="69184-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="69184-133">Key of the entity.</span></span> <span data-ttu-id="69184-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-135">displayName</span><span class="sxs-lookup"><span data-stu-id="69184-135">displayName</span></span>|<span data-ttu-id="69184-136">String</span><span class="sxs-lookup"><span data-stu-id="69184-136">String</span></span>|<span data-ttu-id="69184-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="69184-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="69184-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-139">説明</span><span class="sxs-lookup"><span data-stu-id="69184-139">description</span></span>|<span data-ttu-id="69184-140">String</span><span class="sxs-lookup"><span data-stu-id="69184-140">String</span></span>|<span data-ttu-id="69184-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="69184-141">The description of the app.</span></span> <span data-ttu-id="69184-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-143">publisher</span><span class="sxs-lookup"><span data-stu-id="69184-143">publisher</span></span>|<span data-ttu-id="69184-144">String</span><span class="sxs-lookup"><span data-stu-id="69184-144">String</span></span>|<span data-ttu-id="69184-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="69184-145">The publisher of the app.</span></span> <span data-ttu-id="69184-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="69184-147">largeIcon</span></span>|[<span data-ttu-id="69184-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="69184-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="69184-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="69184-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="69184-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="69184-151">createdDateTime</span></span>|<span data-ttu-id="69184-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69184-152">DateTimeOffset</span></span>|<span data-ttu-id="69184-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="69184-153">The date and time the app was created.</span></span> <span data-ttu-id="69184-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="69184-155">lastModifiedDateTime</span></span>|<span data-ttu-id="69184-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69184-156">DateTimeOffset</span></span>|<span data-ttu-id="69184-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="69184-157">The date and time the app was last modified.</span></span> <span data-ttu-id="69184-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="69184-159">isFeatured</span></span>|<span data-ttu-id="69184-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="69184-160">Boolean</span></span>|<span data-ttu-id="69184-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="69184-162">privacyInformationUrl</span></span>|<span data-ttu-id="69184-163">String</span><span class="sxs-lookup"><span data-stu-id="69184-163">String</span></span>|<span data-ttu-id="69184-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="69184-164">The privacy statement Url.</span></span> <span data-ttu-id="69184-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="69184-166">informationUrl</span></span>|<span data-ttu-id="69184-167">String</span><span class="sxs-lookup"><span data-stu-id="69184-167">String</span></span>|<span data-ttu-id="69184-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="69184-168">The more information Url.</span></span> <span data-ttu-id="69184-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-170">owner</span><span class="sxs-lookup"><span data-stu-id="69184-170">owner</span></span>|<span data-ttu-id="69184-171">String</span><span class="sxs-lookup"><span data-stu-id="69184-171">String</span></span>|<span data-ttu-id="69184-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="69184-172">The owner of the app.</span></span> <span data-ttu-id="69184-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-174">developer</span><span class="sxs-lookup"><span data-stu-id="69184-174">developer</span></span>|<span data-ttu-id="69184-175">String</span><span class="sxs-lookup"><span data-stu-id="69184-175">String</span></span>|<span data-ttu-id="69184-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="69184-176">The developer of the app.</span></span> <span data-ttu-id="69184-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-178">notes</span><span class="sxs-lookup"><span data-stu-id="69184-178">notes</span></span>|<span data-ttu-id="69184-179">String</span><span class="sxs-lookup"><span data-stu-id="69184-179">String</span></span>|<span data-ttu-id="69184-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="69184-180">Notes for the app.</span></span> <span data-ttu-id="69184-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="69184-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="69184-182">publishingState</span></span>|[<span data-ttu-id="69184-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="69184-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="69184-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="69184-184">The publishing state for the app.</span></span> <span data-ttu-id="69184-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="69184-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="69184-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="69184-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="69184-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="69184-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="69184-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="69184-188">appAvailability</span></span>|[<span data-ttu-id="69184-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="69184-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="69184-190">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="69184-190">The Application's availability.</span></span> <span data-ttu-id="69184-191">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="69184-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="69184-192">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="69184-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="69184-193">version</span><span class="sxs-lookup"><span data-stu-id="69184-193">version</span></span>|<span data-ttu-id="69184-194">String</span><span class="sxs-lookup"><span data-stu-id="69184-194">String</span></span>|<span data-ttu-id="69184-195">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="69184-195">The Application's version.</span></span> <span data-ttu-id="69184-196">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="69184-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="69184-197">committedContentVersion</span></span>|<span data-ttu-id="69184-198">String</span><span class="sxs-lookup"><span data-stu-id="69184-198">String</span></span>|<span data-ttu-id="69184-199">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="69184-199">The internal committed content version.</span></span> <span data-ttu-id="69184-200">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="69184-201">fileName</span><span class="sxs-lookup"><span data-stu-id="69184-201">fileName</span></span>|<span data-ttu-id="69184-202">String</span><span class="sxs-lookup"><span data-stu-id="69184-202">String</span></span>|<span data-ttu-id="69184-203">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="69184-203">The name of the main Lob application file.</span></span> <span data-ttu-id="69184-204">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="69184-205">size</span><span class="sxs-lookup"><span data-stu-id="69184-205">size</span></span>|<span data-ttu-id="69184-206">Int64</span><span class="sxs-lookup"><span data-stu-id="69184-206">Int64</span></span>|<span data-ttu-id="69184-207">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="69184-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="69184-208">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="69184-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="69184-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="69184-209">bundleId</span></span>|<span data-ttu-id="69184-210">String</span><span class="sxs-lookup"><span data-stu-id="69184-210">String</span></span>|<span data-ttu-id="69184-211">ID 名。</span><span class="sxs-lookup"><span data-stu-id="69184-211">The Identity Name.</span></span>|
|<span data-ttu-id="69184-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="69184-212">applicableDeviceType</span></span>|[<span data-ttu-id="69184-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="69184-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="69184-214">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="69184-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="69184-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="69184-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="69184-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="69184-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="69184-217">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="69184-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="69184-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="69184-218">expirationDateTime</span></span>|<span data-ttu-id="69184-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="69184-219">DateTimeOffset</span></span>|<span data-ttu-id="69184-220">有効期限。</span><span class="sxs-lookup"><span data-stu-id="69184-220">The expiration time.</span></span>|
|<span data-ttu-id="69184-221">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="69184-221">versionNumber</span></span>|<span data-ttu-id="69184-222">String</span><span class="sxs-lookup"><span data-stu-id="69184-222">String</span></span>|<span data-ttu-id="69184-223">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="69184-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="69184-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="69184-224">buildNumber</span></span>|<span data-ttu-id="69184-225">String</span><span class="sxs-lookup"><span data-stu-id="69184-225">String</span></span>|<span data-ttu-id="69184-226">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="69184-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="69184-227">応答</span><span class="sxs-lookup"><span data-stu-id="69184-227">Response</span></span>
<span data-ttu-id="69184-228">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="69184-228">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69184-229">例</span><span class="sxs-lookup"><span data-stu-id="69184-229">Example</span></span>
### <a name="request"></a><span data-ttu-id="69184-230">要求</span><span class="sxs-lookup"><span data-stu-id="69184-230">Request</span></span>
<span data-ttu-id="69184-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="69184-231">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1287

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="69184-232">応答</span><span class="sxs-lookup"><span data-stu-id="69184-232">Response</span></span>
<span data-ttu-id="69184-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="69184-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1459

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```



