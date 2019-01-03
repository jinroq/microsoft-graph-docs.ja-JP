---
title: iosVppApp の更新
description: iosVppApp オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 05da16de7fc9d9cf5c556fd48f29d327bd6cd6eb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348007"
---
# <a name="update-iosvppapp"></a><span data-ttu-id="da00e-103">iosVppApp の更新</span><span class="sxs-lookup"><span data-stu-id="da00e-103">Update iosVppApp</span></span>

> <span data-ttu-id="da00e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="da00e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da00e-105">[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="da00e-105">Update the properties of a [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da00e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="da00e-106">Prerequisites</span></span>
<span data-ttu-id="da00e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="da00e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da00e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="da00e-109">Permission type</span></span>|<span data-ttu-id="da00e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="da00e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da00e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="da00e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="da00e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da00e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="da00e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="da00e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da00e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da00e-114">Not supported.</span></span>|
|<span data-ttu-id="da00e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="da00e-115">Application</span></span>|<span data-ttu-id="da00e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="da00e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da00e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="da00e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="da00e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da00e-118">Request headers</span></span>
|<span data-ttu-id="da00e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="da00e-119">Header</span></span>|<span data-ttu-id="da00e-120">値</span><span class="sxs-lookup"><span data-stu-id="da00e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da00e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="da00e-121">Authorization</span></span>|<span data-ttu-id="da00e-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="da00e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da00e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="da00e-123">Accept</span></span>|<span data-ttu-id="da00e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="da00e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da00e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="da00e-125">Request body</span></span>
<span data-ttu-id="da00e-126">要求本文で、[iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="da00e-126">In the request body, supply a JSON representation for the [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

<span data-ttu-id="da00e-127">次の表に、[iosVppApp](../resources/intune-apps-iosvppapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="da00e-127">The following table shows the properties that are required when you create the [iosVppApp](../resources/intune-apps-iosvppapp.md).</span></span>

|<span data-ttu-id="da00e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="da00e-128">Property</span></span>|<span data-ttu-id="da00e-129">種類</span><span class="sxs-lookup"><span data-stu-id="da00e-129">Type</span></span>|<span data-ttu-id="da00e-130">説明</span><span class="sxs-lookup"><span data-stu-id="da00e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da00e-131">ID</span><span class="sxs-lookup"><span data-stu-id="da00e-131">id</span></span>|<span data-ttu-id="da00e-132">String</span><span class="sxs-lookup"><span data-stu-id="da00e-132">String</span></span>|<span data-ttu-id="da00e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="da00e-133">Key of the entity.</span></span> <span data-ttu-id="da00e-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-135">displayName</span><span class="sxs-lookup"><span data-stu-id="da00e-135">displayName</span></span>|<span data-ttu-id="da00e-136">String</span><span class="sxs-lookup"><span data-stu-id="da00e-136">String</span></span>|<span data-ttu-id="da00e-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="da00e-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="da00e-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-139">説明</span><span class="sxs-lookup"><span data-stu-id="da00e-139">description</span></span>|<span data-ttu-id="da00e-140">String</span><span class="sxs-lookup"><span data-stu-id="da00e-140">String</span></span>|<span data-ttu-id="da00e-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="da00e-141">The description of the app.</span></span> <span data-ttu-id="da00e-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-143">publisher</span><span class="sxs-lookup"><span data-stu-id="da00e-143">publisher</span></span>|<span data-ttu-id="da00e-144">String</span><span class="sxs-lookup"><span data-stu-id="da00e-144">String</span></span>|<span data-ttu-id="da00e-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="da00e-145">The publisher of the app.</span></span> <span data-ttu-id="da00e-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="da00e-147">largeIcon</span></span>|[<span data-ttu-id="da00e-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="da00e-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="da00e-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="da00e-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="da00e-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="da00e-151">createdDateTime</span></span>|<span data-ttu-id="da00e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da00e-152">DateTimeOffset</span></span>|<span data-ttu-id="da00e-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="da00e-153">The date and time the app was created.</span></span> <span data-ttu-id="da00e-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="da00e-155">lastModifiedDateTime</span></span>|<span data-ttu-id="da00e-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da00e-156">DateTimeOffset</span></span>|<span data-ttu-id="da00e-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="da00e-157">The date and time the app was last modified.</span></span> <span data-ttu-id="da00e-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="da00e-159">isFeatured</span></span>|<span data-ttu-id="da00e-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="da00e-160">Boolean</span></span>|<span data-ttu-id="da00e-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="da00e-162">privacyInformationUrl</span></span>|<span data-ttu-id="da00e-163">String</span><span class="sxs-lookup"><span data-stu-id="da00e-163">String</span></span>|<span data-ttu-id="da00e-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="da00e-164">The privacy statement Url.</span></span> <span data-ttu-id="da00e-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="da00e-166">informationUrl</span></span>|<span data-ttu-id="da00e-167">String</span><span class="sxs-lookup"><span data-stu-id="da00e-167">String</span></span>|<span data-ttu-id="da00e-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="da00e-168">The more information Url.</span></span> <span data-ttu-id="da00e-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-170">owner</span><span class="sxs-lookup"><span data-stu-id="da00e-170">owner</span></span>|<span data-ttu-id="da00e-171">String</span><span class="sxs-lookup"><span data-stu-id="da00e-171">String</span></span>|<span data-ttu-id="da00e-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="da00e-172">The owner of the app.</span></span> <span data-ttu-id="da00e-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-174">developer</span><span class="sxs-lookup"><span data-stu-id="da00e-174">developer</span></span>|<span data-ttu-id="da00e-175">String</span><span class="sxs-lookup"><span data-stu-id="da00e-175">String</span></span>|<span data-ttu-id="da00e-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="da00e-176">The developer of the app.</span></span> <span data-ttu-id="da00e-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-178">notes</span><span class="sxs-lookup"><span data-stu-id="da00e-178">notes</span></span>|<span data-ttu-id="da00e-179">String</span><span class="sxs-lookup"><span data-stu-id="da00e-179">String</span></span>|<span data-ttu-id="da00e-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="da00e-180">Notes for the app.</span></span> <span data-ttu-id="da00e-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="da00e-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="da00e-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="da00e-182">publishingState</span></span>|[<span data-ttu-id="da00e-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="da00e-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="da00e-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="da00e-184">The publishing state for the app.</span></span> <span data-ttu-id="da00e-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="da00e-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="da00e-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="da00e-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="da00e-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="da00e-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="da00e-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="da00e-188">usedLicenseCount</span></span>|<span data-ttu-id="da00e-189">Int32</span><span class="sxs-lookup"><span data-stu-id="da00e-189">Int32</span></span>|<span data-ttu-id="da00e-190">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="da00e-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="da00e-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="da00e-191">totalLicenseCount</span></span>|<span data-ttu-id="da00e-192">Int32</span><span class="sxs-lookup"><span data-stu-id="da00e-192">Int32</span></span>|<span data-ttu-id="da00e-193">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="da00e-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="da00e-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="da00e-194">releaseDateTime</span></span>|<span data-ttu-id="da00e-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="da00e-195">DateTimeOffset</span></span>|<span data-ttu-id="da00e-196">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="da00e-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="da00e-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="da00e-197">appStoreUrl</span></span>|<span data-ttu-id="da00e-198">String</span><span class="sxs-lookup"><span data-stu-id="da00e-198">String</span></span>|<span data-ttu-id="da00e-199">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="da00e-199">The store URL.</span></span>|
|<span data-ttu-id="da00e-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="da00e-200">licensingType</span></span>|[<span data-ttu-id="da00e-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="da00e-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="da00e-202">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="da00e-202">The supported License Type.</span></span>|
|<span data-ttu-id="da00e-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="da00e-203">applicableDeviceType</span></span>|[<span data-ttu-id="da00e-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="da00e-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="da00e-205">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="da00e-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="da00e-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="da00e-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="da00e-207">String</span><span class="sxs-lookup"><span data-stu-id="da00e-207">String</span></span>|<span data-ttu-id="da00e-208">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="da00e-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="da00e-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="da00e-209">vppTokenAccountType</span></span>|[<span data-ttu-id="da00e-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="da00e-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="da00e-211">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="da00e-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="da00e-212">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="da00e-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="da00e-213">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="da00e-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="da00e-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="da00e-214">vppTokenAppleId</span></span>|<span data-ttu-id="da00e-215">String</span><span class="sxs-lookup"><span data-stu-id="da00e-215">String</span></span>|<span data-ttu-id="da00e-216">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="da00e-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="da00e-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="da00e-217">bundleId</span></span>|<span data-ttu-id="da00e-218">String</span><span class="sxs-lookup"><span data-stu-id="da00e-218">String</span></span>|<span data-ttu-id="da00e-219">ID 名。</span><span class="sxs-lookup"><span data-stu-id="da00e-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="da00e-220">応答</span><span class="sxs-lookup"><span data-stu-id="da00e-220">Response</span></span>
<span data-ttu-id="da00e-221">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="da00e-221">If successful, this method returns a `200 OK` response code and an updated [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da00e-222">例</span><span class="sxs-lookup"><span data-stu-id="da00e-222">Example</span></span>
### <a name="request"></a><span data-ttu-id="da00e-223">要求</span><span class="sxs-lookup"><span data-stu-id="da00e-223">Request</span></span>
<span data-ttu-id="da00e-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="da00e-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
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

### <a name="response"></a><span data-ttu-id="da00e-225">応答</span><span class="sxs-lookup"><span data-stu-id="da00e-225">Response</span></span>
<span data-ttu-id="da00e-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="da00e-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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


