---
title: Create iosVppApp
description: 新しい iosVppApp オブジェクトを作成します。
ms.openlocfilehash: df16640ea92296e793a6ebd965530e00112afac1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071411"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="7f3d7-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="7f3d7-103">Create iosVppApp</span></span>

> <span data-ttu-id="7f3d7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7f3d7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7f3d7-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7f3d7-107">新しい [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-107">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7f3d7-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f3d7-108">Prerequisites</span></span>
<span data-ttu-id="7f3d7-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f3d7-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f3d7-111">Permission type</span></span>|<span data-ttu-id="7f3d7-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f3d7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f3d7-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f3d7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7f3d7-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f3d7-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7f3d7-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f3d7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f3d7-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-116">Not supported.</span></span>|
|<span data-ttu-id="7f3d7-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f3d7-117">Application</span></span>|<span data-ttu-id="7f3d7-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f3d7-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f3d7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="7f3d7-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f3d7-120">Request headers</span></span>
|<span data-ttu-id="7f3d7-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f3d7-121">Header</span></span>|<span data-ttu-id="7f3d7-122">値</span><span class="sxs-lookup"><span data-stu-id="7f3d7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f3d7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f3d7-123">Authorization</span></span>|<span data-ttu-id="7f3d7-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f3d7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7f3d7-125">Accept</span></span>|<span data-ttu-id="7f3d7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7f3d7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f3d7-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f3d7-127">Request body</span></span>
<span data-ttu-id="7f3d7-128">要求本文で、iosVppApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-128">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="7f3d7-129">次の表に、iosVppApp 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-129">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="7f3d7-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7f3d7-130">Property</span></span>|<span data-ttu-id="7f3d7-131">型</span><span class="sxs-lookup"><span data-stu-id="7f3d7-131">Type</span></span>|<span data-ttu-id="7f3d7-132">説明</span><span class="sxs-lookup"><span data-stu-id="7f3d7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f3d7-133">id</span><span class="sxs-lookup"><span data-stu-id="7f3d7-133">id</span></span>|<span data-ttu-id="7f3d7-134">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-134">String</span></span>|<span data-ttu-id="7f3d7-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-135">Key of the entity.</span></span> <span data-ttu-id="7f3d7-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-137">displayName</span><span class="sxs-lookup"><span data-stu-id="7f3d7-137">displayName</span></span>|<span data-ttu-id="7f3d7-138">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-138">String</span></span>|<span data-ttu-id="7f3d7-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="7f3d7-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-141">説明</span><span class="sxs-lookup"><span data-stu-id="7f3d7-141">description</span></span>|<span data-ttu-id="7f3d7-142">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-142">String</span></span>|<span data-ttu-id="7f3d7-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-143">The description of the app.</span></span> <span data-ttu-id="7f3d7-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-145">publisher</span><span class="sxs-lookup"><span data-stu-id="7f3d7-145">publisher</span></span>|<span data-ttu-id="7f3d7-146">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-146">String</span></span>|<span data-ttu-id="7f3d7-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-147">The publisher of the app.</span></span> <span data-ttu-id="7f3d7-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="7f3d7-149">largeIcon</span></span>|[<span data-ttu-id="7f3d7-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="7f3d7-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="7f3d7-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="7f3d7-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f3d7-153">createdDateTime</span></span>|<span data-ttu-id="7f3d7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f3d7-154">DateTimeOffset</span></span>|<span data-ttu-id="7f3d7-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-155">The date and time the app was created.</span></span> <span data-ttu-id="7f3d7-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f3d7-157">lastModifiedDateTime</span></span>|<span data-ttu-id="7f3d7-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f3d7-158">DateTimeOffset</span></span>|<span data-ttu-id="7f3d7-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-159">The date and time the app was last modified.</span></span> <span data-ttu-id="7f3d7-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="7f3d7-161">isFeatured</span></span>|<span data-ttu-id="7f3d7-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f3d7-162">Boolean</span></span>|<span data-ttu-id="7f3d7-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="7f3d7-164">privacyInformationUrl</span></span>|<span data-ttu-id="7f3d7-165">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-165">String</span></span>|<span data-ttu-id="7f3d7-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-166">The privacy statement Url.</span></span> <span data-ttu-id="7f3d7-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="7f3d7-168">informationUrl</span></span>|<span data-ttu-id="7f3d7-169">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-169">String</span></span>|<span data-ttu-id="7f3d7-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-170">The more information Url.</span></span> <span data-ttu-id="7f3d7-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-172">owner</span><span class="sxs-lookup"><span data-stu-id="7f3d7-172">owner</span></span>|<span data-ttu-id="7f3d7-173">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-173">String</span></span>|<span data-ttu-id="7f3d7-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-174">The owner of the app.</span></span> <span data-ttu-id="7f3d7-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-176">developer</span><span class="sxs-lookup"><span data-stu-id="7f3d7-176">developer</span></span>|<span data-ttu-id="7f3d7-177">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-177">String</span></span>|<span data-ttu-id="7f3d7-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-178">The developer of the app.</span></span> <span data-ttu-id="7f3d7-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-180">notes</span><span class="sxs-lookup"><span data-stu-id="7f3d7-180">notes</span></span>|<span data-ttu-id="7f3d7-181">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-181">String</span></span>|<span data-ttu-id="7f3d7-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-182">Notes for the app.</span></span> <span data-ttu-id="7f3d7-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="7f3d7-184">uploadState</span></span>|<span data-ttu-id="7f3d7-185">Int32</span><span class="sxs-lookup"><span data-stu-id="7f3d7-185">Int32</span></span>|<span data-ttu-id="7f3d7-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-186">The upload state.</span></span> <span data-ttu-id="7f3d7-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="7f3d7-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="7f3d7-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="7f3d7-188">publishingState</span></span>|[<span data-ttu-id="7f3d7-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="7f3d7-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="7f3d7-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-190">The publishing state for the app.</span></span> <span data-ttu-id="7f3d7-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="7f3d7-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="7f3d7-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="7f3d7-194">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7f3d7-194">usedLicenseCount</span></span>|<span data-ttu-id="7f3d7-195">Int32</span><span class="sxs-lookup"><span data-stu-id="7f3d7-195">Int32</span></span>|<span data-ttu-id="7f3d7-196">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-196">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="7f3d7-197">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="7f3d7-197">totalLicenseCount</span></span>|<span data-ttu-id="7f3d7-198">Int32</span><span class="sxs-lookup"><span data-stu-id="7f3d7-198">Int32</span></span>|<span data-ttu-id="7f3d7-199">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-199">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="7f3d7-200">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="7f3d7-200">releaseDateTime</span></span>|<span data-ttu-id="7f3d7-201">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f3d7-201">DateTimeOffset</span></span>|<span data-ttu-id="7f3d7-202">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-202">The VPP application release date and time.</span></span>|
|<span data-ttu-id="7f3d7-203">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="7f3d7-203">appStoreUrl</span></span>|<span data-ttu-id="7f3d7-204">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-204">String</span></span>|<span data-ttu-id="7f3d7-205">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-205">The store URL.</span></span>|
|<span data-ttu-id="7f3d7-206">licensingType</span><span class="sxs-lookup"><span data-stu-id="7f3d7-206">licensingType</span></span>|[<span data-ttu-id="7f3d7-207">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="7f3d7-207">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="7f3d7-208">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-208">The supported License Type.</span></span>|
|<span data-ttu-id="7f3d7-209">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="7f3d7-209">applicableDeviceType</span></span>|[<span data-ttu-id="7f3d7-210">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="7f3d7-210">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="7f3d7-211">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-211">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="7f3d7-212">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="7f3d7-212">vppTokenOrganizationName</span></span>|<span data-ttu-id="7f3d7-213">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-213">String</span></span>|<span data-ttu-id="7f3d7-214">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="7f3d7-214">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="7f3d7-215">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="7f3d7-215">vppTokenAccountType</span></span>|[<span data-ttu-id="7f3d7-216">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="7f3d7-216">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="7f3d7-217">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-217">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="7f3d7-218">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-218">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="7f3d7-219">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-219">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="7f3d7-220">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="7f3d7-220">vppTokenAppleId</span></span>|<span data-ttu-id="7f3d7-221">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-221">String</span></span>|<span data-ttu-id="7f3d7-222">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-222">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="7f3d7-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="7f3d7-223">bundleId</span></span>|<span data-ttu-id="7f3d7-224">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-224">String</span></span>|<span data-ttu-id="7f3d7-225">ID 名。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-225">The Identity Name.</span></span>|
|<span data-ttu-id="7f3d7-226">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="7f3d7-226">vppTokenId</span></span>|<span data-ttu-id="7f3d7-227">String</span><span class="sxs-lookup"><span data-stu-id="7f3d7-227">String</span></span>|<span data-ttu-id="7f3d7-228">このアプリケーションに関連付けられている VPP トークンの識別子です。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-228">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="7f3d7-229">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="7f3d7-229">revokeLicenseActionResults</span></span>|<span data-ttu-id="7f3d7-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="7f3d7-230">[iosVppAppRevokeLicensesActionResult](../resources/intune-apps-iosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="7f3d7-231">結果は、このアプリケーションについてのライセンスを失効します。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-231">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="7f3d7-232">応答</span><span class="sxs-lookup"><span data-stu-id="7f3d7-232">Response</span></span>
<span data-ttu-id="7f3d7-233">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-233">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f3d7-234">例</span><span class="sxs-lookup"><span data-stu-id="7f3d7-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="7f3d7-235">要求</span><span class="sxs-lookup"><span data-stu-id="7f3d7-235">Request</span></span>
<span data-ttu-id="7f3d7-236">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1951

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
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
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

### <a name="response"></a><span data-ttu-id="7f3d7-237">応答</span><span class="sxs-lookup"><span data-stu-id="7f3d7-237">Response</span></span>
<span data-ttu-id="7f3d7-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f3d7-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2059

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





