---
title: managedIOSLobApp の更新
description: managedIOSLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ad1e323932a2190c7e442820600129430ace90c2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013851"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="4fcc7-103">managedIOSLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="4fcc7-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="4fcc7-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fcc7-105">[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-105">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fcc7-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4fcc7-106">Prerequisites</span></span>
<span data-ttu-id="4fcc7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fcc7-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4fcc7-109">Permission type</span></span>|<span data-ttu-id="4fcc7-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4fcc7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fcc7-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4fcc7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4fcc7-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fcc7-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4fcc7-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4fcc7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fcc7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-114">Not supported.</span></span>|
|<span data-ttu-id="4fcc7-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4fcc7-115">Application</span></span>|<span data-ttu-id="4fcc7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fcc7-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fcc7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="4fcc7-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fcc7-118">Request headers</span></span>
|<span data-ttu-id="4fcc7-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fcc7-119">Header</span></span>|<span data-ttu-id="4fcc7-120">値</span><span class="sxs-lookup"><span data-stu-id="4fcc7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fcc7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fcc7-121">Authorization</span></span>|<span data-ttu-id="4fcc7-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fcc7-123">承諾</span><span class="sxs-lookup"><span data-stu-id="4fcc7-123">Accept</span></span>|<span data-ttu-id="4fcc7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4fcc7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fcc7-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fcc7-125">Request body</span></span>
<span data-ttu-id="4fcc7-126">要求本文で、[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-126">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="4fcc7-127">次の表に、[managedDeviceOverview](../resources/intune-apps-managedioslobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-127">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="4fcc7-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fcc7-128">Property</span></span>|<span data-ttu-id="4fcc7-129">型</span><span class="sxs-lookup"><span data-stu-id="4fcc7-129">Type</span></span>|<span data-ttu-id="4fcc7-130">説明</span><span class="sxs-lookup"><span data-stu-id="4fcc7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fcc7-131">id</span><span class="sxs-lookup"><span data-stu-id="4fcc7-131">id</span></span>|<span data-ttu-id="4fcc7-132">文字列</span><span class="sxs-lookup"><span data-stu-id="4fcc7-132">String</span></span>|<span data-ttu-id="4fcc7-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-133">Key of the entity.</span></span> <span data-ttu-id="4fcc7-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4fcc7-135">displayName</span></span>|<span data-ttu-id="4fcc7-136">文字列</span><span class="sxs-lookup"><span data-stu-id="4fcc7-136">String</span></span>|<span data-ttu-id="4fcc7-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="4fcc7-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-139">description</span><span class="sxs-lookup"><span data-stu-id="4fcc7-139">description</span></span>|<span data-ttu-id="4fcc7-140">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-140">String</span></span>|<span data-ttu-id="4fcc7-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-141">The description of the app.</span></span> <span data-ttu-id="4fcc7-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-143">publisher</span><span class="sxs-lookup"><span data-stu-id="4fcc7-143">publisher</span></span>|<span data-ttu-id="4fcc7-144">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-144">String</span></span>|<span data-ttu-id="4fcc7-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-145">The publisher of the app.</span></span> <span data-ttu-id="4fcc7-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="4fcc7-147">largeIcon</span></span>|[<span data-ttu-id="4fcc7-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="4fcc7-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="4fcc7-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="4fcc7-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4fcc7-151">createdDateTime</span></span>|<span data-ttu-id="4fcc7-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fcc7-152">DateTimeOffset</span></span>|<span data-ttu-id="4fcc7-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-153">The date and time the app was created.</span></span> <span data-ttu-id="4fcc7-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fcc7-155">lastModifiedDateTime</span></span>|<span data-ttu-id="4fcc7-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fcc7-156">DateTimeOffset</span></span>|<span data-ttu-id="4fcc7-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-157">The date and time the app was last modified.</span></span> <span data-ttu-id="4fcc7-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="4fcc7-159">isFeatured</span></span>|<span data-ttu-id="4fcc7-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="4fcc7-160">Boolean</span></span>|<span data-ttu-id="4fcc7-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="4fcc7-162">privacyInformationUrl</span></span>|<span data-ttu-id="4fcc7-163">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-163">String</span></span>|<span data-ttu-id="4fcc7-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-164">The privacy statement Url.</span></span> <span data-ttu-id="4fcc7-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="4fcc7-166">informationUrl</span></span>|<span data-ttu-id="4fcc7-167">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-167">String</span></span>|<span data-ttu-id="4fcc7-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-168">The more information Url.</span></span> <span data-ttu-id="4fcc7-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-170">owner</span><span class="sxs-lookup"><span data-stu-id="4fcc7-170">owner</span></span>|<span data-ttu-id="4fcc7-171">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-171">String</span></span>|<span data-ttu-id="4fcc7-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-172">The owner of the app.</span></span> <span data-ttu-id="4fcc7-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-174">developer</span><span class="sxs-lookup"><span data-stu-id="4fcc7-174">developer</span></span>|<span data-ttu-id="4fcc7-175">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-175">String</span></span>|<span data-ttu-id="4fcc7-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-176">The developer of the app.</span></span> <span data-ttu-id="4fcc7-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-178">notes</span><span class="sxs-lookup"><span data-stu-id="4fcc7-178">notes</span></span>|<span data-ttu-id="4fcc7-179">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-179">String</span></span>|<span data-ttu-id="4fcc7-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-180">Notes for the app.</span></span> <span data-ttu-id="4fcc7-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="4fcc7-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="4fcc7-182">publishingState</span></span>|[<span data-ttu-id="4fcc7-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="4fcc7-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="4fcc7-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-184">The publishing state for the app.</span></span> <span data-ttu-id="4fcc7-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="4fcc7-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="4fcc7-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="4fcc7-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="4fcc7-188">appAvailability</span></span>|[<span data-ttu-id="4fcc7-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="4fcc7-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="4fcc7-190">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-190">The Application's availability.</span></span> <span data-ttu-id="4fcc7-191">[Managedapp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="4fcc7-192">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="4fcc7-193">version</span><span class="sxs-lookup"><span data-stu-id="4fcc7-193">version</span></span>|<span data-ttu-id="4fcc7-194">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-194">String</span></span>|<span data-ttu-id="4fcc7-195">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-195">The Application's version.</span></span> <span data-ttu-id="4fcc7-196">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="4fcc7-197">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="4fcc7-197">committedContentVersion</span></span>|<span data-ttu-id="4fcc7-198">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-198">String</span></span>|<span data-ttu-id="4fcc7-199">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-199">The internal committed content version.</span></span> <span data-ttu-id="4fcc7-200">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-200">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4fcc7-201">fileName</span><span class="sxs-lookup"><span data-stu-id="4fcc7-201">fileName</span></span>|<span data-ttu-id="4fcc7-202">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-202">String</span></span>|<span data-ttu-id="4fcc7-203">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-203">The name of the main Lob application file.</span></span> <span data-ttu-id="4fcc7-204">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-204">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4fcc7-205">size</span><span class="sxs-lookup"><span data-stu-id="4fcc7-205">size</span></span>|<span data-ttu-id="4fcc7-206">Int64</span><span class="sxs-lookup"><span data-stu-id="4fcc7-206">Int64</span></span>|<span data-ttu-id="4fcc7-207">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-207">The total size, including all uploaded files.</span></span> <span data-ttu-id="4fcc7-208">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="4fcc7-208">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="4fcc7-209">bundleId</span><span class="sxs-lookup"><span data-stu-id="4fcc7-209">bundleId</span></span>|<span data-ttu-id="4fcc7-210">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-210">String</span></span>|<span data-ttu-id="4fcc7-211">ID 名。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-211">The Identity Name.</span></span>|
|<span data-ttu-id="4fcc7-212">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="4fcc7-212">applicableDeviceType</span></span>|[<span data-ttu-id="4fcc7-213">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="4fcc7-213">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="4fcc7-214">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-214">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="4fcc7-215">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4fcc7-215">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="4fcc7-216">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="4fcc7-216">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="4fcc7-217">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-217">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="4fcc7-218">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="4fcc7-218">expirationDateTime</span></span>|<span data-ttu-id="4fcc7-219">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fcc7-219">DateTimeOffset</span></span>|<span data-ttu-id="4fcc7-220">有効期限。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-220">The expiration time.</span></span>|
|<span data-ttu-id="4fcc7-221">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="4fcc7-221">versionNumber</span></span>|<span data-ttu-id="4fcc7-222">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-222">String</span></span>|<span data-ttu-id="4fcc7-223">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-223">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="4fcc7-224">buildNumber</span><span class="sxs-lookup"><span data-stu-id="4fcc7-224">buildNumber</span></span>|<span data-ttu-id="4fcc7-225">String</span><span class="sxs-lookup"><span data-stu-id="4fcc7-225">String</span></span>|<span data-ttu-id="4fcc7-226">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-226">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="4fcc7-227">応答</span><span class="sxs-lookup"><span data-stu-id="4fcc7-227">Response</span></span>
<span data-ttu-id="4fcc7-228">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-228">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fcc7-229">例</span><span class="sxs-lookup"><span data-stu-id="4fcc7-229">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fcc7-230">要求</span><span class="sxs-lookup"><span data-stu-id="4fcc7-230">Request</span></span>
<span data-ttu-id="4fcc7-231">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-231">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="4fcc7-232">応答</span><span class="sxs-lookup"><span data-stu-id="4fcc7-232">Response</span></span>
<span data-ttu-id="4fcc7-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4fcc7-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



