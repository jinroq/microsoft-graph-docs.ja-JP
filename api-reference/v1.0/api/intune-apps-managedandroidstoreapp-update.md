---
title: managedAndroidStoreApp の更新
description: managedAndroidStoreApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 810efdaab711694ede6e507edf5aef272918e064
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917917"
---
# <a name="update-managedandroidstoreapp"></a><span data-ttu-id="b2a3b-103">managedAndroidStoreApp の更新</span><span class="sxs-lookup"><span data-stu-id="b2a3b-103">Update managedAndroidStoreApp</span></span>

> <span data-ttu-id="b2a3b-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b2a3b-105">[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-105">Update the properties of a [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b2a3b-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b2a3b-106">Prerequisites</span></span>
<span data-ttu-id="b2a3b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2a3b-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b2a3b-109">Permission type</span></span>|<span data-ttu-id="b2a3b-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b2a3b-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b2a3b-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b2a3b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b2a3b-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2a3b-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b2a3b-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b2a3b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b2a3b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-114">Not supported.</span></span>|
|<span data-ttu-id="b2a3b-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b2a3b-115">Application</span></span>|<span data-ttu-id="b2a3b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b2a3b-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b2a3b-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="b2a3b-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2a3b-118">Request headers</span></span>
|<span data-ttu-id="b2a3b-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b2a3b-119">Header</span></span>|<span data-ttu-id="b2a3b-120">値</span><span class="sxs-lookup"><span data-stu-id="b2a3b-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b2a3b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2a3b-121">Authorization</span></span>|<span data-ttu-id="b2a3b-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b2a3b-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b2a3b-123">Accept</span></span>|<span data-ttu-id="b2a3b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b2a3b-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2a3b-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b2a3b-125">Request body</span></span>
<span data-ttu-id="b2a3b-126">要求本文で、[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-126">In the request body, supply a JSON representation for the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object.</span></span>

<span data-ttu-id="b2a3b-127">次の表に、[managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-127">The following table shows the properties that are required when you create the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md).</span></span>

|<span data-ttu-id="b2a3b-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2a3b-128">Property</span></span>|<span data-ttu-id="b2a3b-129">種類</span><span class="sxs-lookup"><span data-stu-id="b2a3b-129">Type</span></span>|<span data-ttu-id="b2a3b-130">説明</span><span class="sxs-lookup"><span data-stu-id="b2a3b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2a3b-131">ID</span><span class="sxs-lookup"><span data-stu-id="b2a3b-131">id</span></span>|<span data-ttu-id="b2a3b-132">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-132">String</span></span>|<span data-ttu-id="b2a3b-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-133">Key of the entity.</span></span> <span data-ttu-id="b2a3b-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b2a3b-135">displayName</span></span>|<span data-ttu-id="b2a3b-136">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-136">String</span></span>|<span data-ttu-id="b2a3b-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b2a3b-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-139">説明</span><span class="sxs-lookup"><span data-stu-id="b2a3b-139">description</span></span>|<span data-ttu-id="b2a3b-140">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-140">String</span></span>|<span data-ttu-id="b2a3b-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-141">The description of the app.</span></span> <span data-ttu-id="b2a3b-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-143">publisher</span><span class="sxs-lookup"><span data-stu-id="b2a3b-143">publisher</span></span>|<span data-ttu-id="b2a3b-144">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-144">String</span></span>|<span data-ttu-id="b2a3b-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-145">The publisher of the app.</span></span> <span data-ttu-id="b2a3b-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b2a3b-147">largeIcon</span></span>|[<span data-ttu-id="b2a3b-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b2a3b-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b2a3b-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b2a3b-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b2a3b-151">createdDateTime</span></span>|<span data-ttu-id="b2a3b-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2a3b-152">DateTimeOffset</span></span>|<span data-ttu-id="b2a3b-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-153">The date and time the app was created.</span></span> <span data-ttu-id="b2a3b-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b2a3b-155">lastModifiedDateTime</span></span>|<span data-ttu-id="b2a3b-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2a3b-156">DateTimeOffset</span></span>|<span data-ttu-id="b2a3b-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-157">The date and time the app was last modified.</span></span> <span data-ttu-id="b2a3b-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b2a3b-159">isFeatured</span></span>|<span data-ttu-id="b2a3b-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="b2a3b-160">Boolean</span></span>|<span data-ttu-id="b2a3b-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b2a3b-162">privacyInformationUrl</span></span>|<span data-ttu-id="b2a3b-163">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-163">String</span></span>|<span data-ttu-id="b2a3b-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-164">The privacy statement Url.</span></span> <span data-ttu-id="b2a3b-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b2a3b-166">informationUrl</span></span>|<span data-ttu-id="b2a3b-167">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-167">String</span></span>|<span data-ttu-id="b2a3b-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-168">The more information Url.</span></span> <span data-ttu-id="b2a3b-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-170">owner</span><span class="sxs-lookup"><span data-stu-id="b2a3b-170">owner</span></span>|<span data-ttu-id="b2a3b-171">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-171">String</span></span>|<span data-ttu-id="b2a3b-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-172">The owner of the app.</span></span> <span data-ttu-id="b2a3b-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-174">developer</span><span class="sxs-lookup"><span data-stu-id="b2a3b-174">developer</span></span>|<span data-ttu-id="b2a3b-175">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-175">String</span></span>|<span data-ttu-id="b2a3b-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-176">The developer of the app.</span></span> <span data-ttu-id="b2a3b-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-178">notes</span><span class="sxs-lookup"><span data-stu-id="b2a3b-178">notes</span></span>|<span data-ttu-id="b2a3b-179">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-179">String</span></span>|<span data-ttu-id="b2a3b-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-180">Notes for the app.</span></span> <span data-ttu-id="b2a3b-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b2a3b-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="b2a3b-182">publishingState</span></span>|[<span data-ttu-id="b2a3b-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b2a3b-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b2a3b-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-184">The publishing state for the app.</span></span> <span data-ttu-id="b2a3b-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b2a3b-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b2a3b-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b2a3b-188">appAvailability</span><span class="sxs-lookup"><span data-stu-id="b2a3b-188">appAvailability</span></span>|[<span data-ttu-id="b2a3b-189">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="b2a3b-189">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="b2a3b-190">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-190">The Application's availability.</span></span> <span data-ttu-id="b2a3b-191">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-191">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="b2a3b-192">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-192">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="b2a3b-193">version</span><span class="sxs-lookup"><span data-stu-id="b2a3b-193">version</span></span>|<span data-ttu-id="b2a3b-194">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-194">String</span></span>|<span data-ttu-id="b2a3b-195">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-195">The Application's version.</span></span> <span data-ttu-id="b2a3b-196">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b2a3b-196">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="b2a3b-197">packageId</span><span class="sxs-lookup"><span data-stu-id="b2a3b-197">packageId</span></span>|<span data-ttu-id="b2a3b-198">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-198">String</span></span>|<span data-ttu-id="b2a3b-199">アプリのパッケージ ID。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-199">The app's package ID.</span></span>|
|<span data-ttu-id="b2a3b-200">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="b2a3b-200">appStoreUrl</span></span>|<span data-ttu-id="b2a3b-201">String</span><span class="sxs-lookup"><span data-stu-id="b2a3b-201">String</span></span>|<span data-ttu-id="b2a3b-202">Android の AppStoreUrl。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-202">The Android AppStoreUrl.</span></span>|
|<span data-ttu-id="b2a3b-203">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b2a3b-203">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="b2a3b-204">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="b2a3b-204">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="b2a3b-205">サポートされているオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-205">The value for the minimum supported operating system.</span></span>|



## <a name="response"></a><span data-ttu-id="b2a3b-206">応答</span><span class="sxs-lookup"><span data-stu-id="b2a3b-206">Response</span></span>
<span data-ttu-id="b2a3b-207">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-207">If successful, this method returns a `200 OK` response code and an updated [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2a3b-208">例</span><span class="sxs-lookup"><span data-stu-id="b2a3b-208">Example</span></span>
### <a name="request"></a><span data-ttu-id="b2a3b-209">要求</span><span class="sxs-lookup"><span data-stu-id="b2a3b-209">Request</span></span>
<span data-ttu-id="b2a3b-210">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-210">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1016

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
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
  "packageId": "Package Id value",
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
    "v5_1": true
  }
}
```

### <a name="response"></a><span data-ttu-id="b2a3b-211">応答</span><span class="sxs-lookup"><span data-stu-id="b2a3b-211">Response</span></span>
<span data-ttu-id="b2a3b-p117">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b2a3b-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1188

{
  "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
  "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
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
  "packageId": "Package Id value",
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
    "v5_1": true
  }
}
```



