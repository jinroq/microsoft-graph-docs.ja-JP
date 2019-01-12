---
title: Create iosVppApp
description: 新しい iosVppApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 562f9f87effc78ed1723042a3270592ad2d08206
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971355"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="55f59-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="55f59-103">Create iosVppApp</span></span>

> <span data-ttu-id="55f59-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="55f59-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55f59-105">新しい [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="55f59-105">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="55f59-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="55f59-106">Prerequisites</span></span>
<span data-ttu-id="55f59-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55f59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55f59-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55f59-109">Permission type</span></span>|<span data-ttu-id="55f59-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="55f59-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55f59-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="55f59-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55f59-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55f59-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="55f59-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55f59-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55f59-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55f59-114">Not supported.</span></span>|
|<span data-ttu-id="55f59-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55f59-115">Application</span></span>|<span data-ttu-id="55f59-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55f59-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55f59-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55f59-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="55f59-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55f59-118">Request headers</span></span>
|<span data-ttu-id="55f59-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55f59-119">Header</span></span>|<span data-ttu-id="55f59-120">値</span><span class="sxs-lookup"><span data-stu-id="55f59-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55f59-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="55f59-121">Authorization</span></span>|<span data-ttu-id="55f59-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="55f59-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55f59-123">Accept</span><span class="sxs-lookup"><span data-stu-id="55f59-123">Accept</span></span>|<span data-ttu-id="55f59-124">application/json</span><span class="sxs-lookup"><span data-stu-id="55f59-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55f59-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="55f59-125">Request body</span></span>
<span data-ttu-id="55f59-126">要求本文で、iosVppApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="55f59-126">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="55f59-127">次の表に、iosVppApp 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="55f59-127">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="55f59-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55f59-128">Property</span></span>|<span data-ttu-id="55f59-129">種類</span><span class="sxs-lookup"><span data-stu-id="55f59-129">Type</span></span>|<span data-ttu-id="55f59-130">説明</span><span class="sxs-lookup"><span data-stu-id="55f59-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55f59-131">ID</span><span class="sxs-lookup"><span data-stu-id="55f59-131">id</span></span>|<span data-ttu-id="55f59-132">String</span><span class="sxs-lookup"><span data-stu-id="55f59-132">String</span></span>|<span data-ttu-id="55f59-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="55f59-133">Key of the entity.</span></span> <span data-ttu-id="55f59-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-135">displayName</span><span class="sxs-lookup"><span data-stu-id="55f59-135">displayName</span></span>|<span data-ttu-id="55f59-136">String</span><span class="sxs-lookup"><span data-stu-id="55f59-136">String</span></span>|<span data-ttu-id="55f59-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="55f59-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="55f59-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-139">説明</span><span class="sxs-lookup"><span data-stu-id="55f59-139">description</span></span>|<span data-ttu-id="55f59-140">String</span><span class="sxs-lookup"><span data-stu-id="55f59-140">String</span></span>|<span data-ttu-id="55f59-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="55f59-141">The description of the app.</span></span> <span data-ttu-id="55f59-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-143">publisher</span><span class="sxs-lookup"><span data-stu-id="55f59-143">publisher</span></span>|<span data-ttu-id="55f59-144">String</span><span class="sxs-lookup"><span data-stu-id="55f59-144">String</span></span>|<span data-ttu-id="55f59-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="55f59-145">The publisher of the app.</span></span> <span data-ttu-id="55f59-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="55f59-147">largeIcon</span></span>|[<span data-ttu-id="55f59-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="55f59-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="55f59-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="55f59-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="55f59-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="55f59-151">createdDateTime</span></span>|<span data-ttu-id="55f59-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55f59-152">DateTimeOffset</span></span>|<span data-ttu-id="55f59-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="55f59-153">The date and time the app was created.</span></span> <span data-ttu-id="55f59-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="55f59-155">lastModifiedDateTime</span></span>|<span data-ttu-id="55f59-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55f59-156">DateTimeOffset</span></span>|<span data-ttu-id="55f59-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="55f59-157">The date and time the app was last modified.</span></span> <span data-ttu-id="55f59-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="55f59-159">isFeatured</span></span>|<span data-ttu-id="55f59-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f59-160">Boolean</span></span>|<span data-ttu-id="55f59-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="55f59-162">privacyInformationUrl</span></span>|<span data-ttu-id="55f59-163">String</span><span class="sxs-lookup"><span data-stu-id="55f59-163">String</span></span>|<span data-ttu-id="55f59-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="55f59-164">The privacy statement Url.</span></span> <span data-ttu-id="55f59-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="55f59-166">informationUrl</span></span>|<span data-ttu-id="55f59-167">String</span><span class="sxs-lookup"><span data-stu-id="55f59-167">String</span></span>|<span data-ttu-id="55f59-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="55f59-168">The more information Url.</span></span> <span data-ttu-id="55f59-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-170">owner</span><span class="sxs-lookup"><span data-stu-id="55f59-170">owner</span></span>|<span data-ttu-id="55f59-171">String</span><span class="sxs-lookup"><span data-stu-id="55f59-171">String</span></span>|<span data-ttu-id="55f59-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="55f59-172">The owner of the app.</span></span> <span data-ttu-id="55f59-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-174">developer</span><span class="sxs-lookup"><span data-stu-id="55f59-174">developer</span></span>|<span data-ttu-id="55f59-175">String</span><span class="sxs-lookup"><span data-stu-id="55f59-175">String</span></span>|<span data-ttu-id="55f59-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="55f59-176">The developer of the app.</span></span> <span data-ttu-id="55f59-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-178">notes</span><span class="sxs-lookup"><span data-stu-id="55f59-178">notes</span></span>|<span data-ttu-id="55f59-179">String</span><span class="sxs-lookup"><span data-stu-id="55f59-179">String</span></span>|<span data-ttu-id="55f59-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="55f59-180">Notes for the app.</span></span> <span data-ttu-id="55f59-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="55f59-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="55f59-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="55f59-182">publishingState</span></span>|[<span data-ttu-id="55f59-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="55f59-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="55f59-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="55f59-184">The publishing state for the app.</span></span> <span data-ttu-id="55f59-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="55f59-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="55f59-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="55f59-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="55f59-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="55f59-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="55f59-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="55f59-188">usedLicenseCount</span></span>|<span data-ttu-id="55f59-189">Int32</span><span class="sxs-lookup"><span data-stu-id="55f59-189">Int32</span></span>|<span data-ttu-id="55f59-190">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="55f59-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="55f59-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="55f59-191">totalLicenseCount</span></span>|<span data-ttu-id="55f59-192">Int32</span><span class="sxs-lookup"><span data-stu-id="55f59-192">Int32</span></span>|<span data-ttu-id="55f59-193">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="55f59-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="55f59-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="55f59-194">releaseDateTime</span></span>|<span data-ttu-id="55f59-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="55f59-195">DateTimeOffset</span></span>|<span data-ttu-id="55f59-196">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="55f59-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="55f59-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="55f59-197">appStoreUrl</span></span>|<span data-ttu-id="55f59-198">String</span><span class="sxs-lookup"><span data-stu-id="55f59-198">String</span></span>|<span data-ttu-id="55f59-199">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="55f59-199">The store URL.</span></span>|
|<span data-ttu-id="55f59-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="55f59-200">licensingType</span></span>|[<span data-ttu-id="55f59-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="55f59-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="55f59-202">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="55f59-202">The supported License Type.</span></span>|
|<span data-ttu-id="55f59-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="55f59-203">applicableDeviceType</span></span>|[<span data-ttu-id="55f59-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="55f59-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="55f59-205">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="55f59-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="55f59-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="55f59-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="55f59-207">String</span><span class="sxs-lookup"><span data-stu-id="55f59-207">String</span></span>|<span data-ttu-id="55f59-208">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="55f59-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="55f59-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="55f59-209">vppTokenAccountType</span></span>|[<span data-ttu-id="55f59-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="55f59-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="55f59-211">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="55f59-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="55f59-212">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="55f59-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="55f59-213">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="55f59-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="55f59-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="55f59-214">vppTokenAppleId</span></span>|<span data-ttu-id="55f59-215">String</span><span class="sxs-lookup"><span data-stu-id="55f59-215">String</span></span>|<span data-ttu-id="55f59-216">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="55f59-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="55f59-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="55f59-217">bundleId</span></span>|<span data-ttu-id="55f59-218">String</span><span class="sxs-lookup"><span data-stu-id="55f59-218">String</span></span>|<span data-ttu-id="55f59-219">ID 名。</span><span class="sxs-lookup"><span data-stu-id="55f59-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="55f59-220">応答</span><span class="sxs-lookup"><span data-stu-id="55f59-220">Response</span></span>
<span data-ttu-id="55f59-221">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="55f59-221">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55f59-222">例</span><span class="sxs-lookup"><span data-stu-id="55f59-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="55f59-223">要求</span><span class="sxs-lookup"><span data-stu-id="55f59-223">Request</span></span>
<span data-ttu-id="55f59-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="55f59-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1222

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
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
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
  "bundleId": "Bundle Id value"
}
```

### <a name="response"></a><span data-ttu-id="55f59-225">応答</span><span class="sxs-lookup"><span data-stu-id="55f59-225">Response</span></span>
<span data-ttu-id="55f59-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="55f59-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1394

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
  "publishingState": "processing",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "appStoreUrl": "https://example.com/appStoreUrl/",
  "licensingType": {
    "@odata.type": "microsoft.graph.vppLicensingType",
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
  "bundleId": "Bundle Id value"
}
```



