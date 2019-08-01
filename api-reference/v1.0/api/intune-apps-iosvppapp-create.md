---
title: Create iosVppApp
description: 新しい iosVppApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c58775bc588817b9e1c810b81bd9e3dbadd4d383
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997891"
---
# <a name="create-iosvppapp"></a><span data-ttu-id="91777-103">Create iosVppApp</span><span class="sxs-lookup"><span data-stu-id="91777-103">Create iosVppApp</span></span>

> <span data-ttu-id="91777-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91777-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91777-105">新しい [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="91777-105">Create a new [iosVppApp](../resources/intune-apps-iosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91777-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="91777-106">Prerequisites</span></span>
<span data-ttu-id="91777-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91777-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91777-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91777-109">Permission type</span></span>|<span data-ttu-id="91777-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="91777-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91777-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91777-111">Delegated (work or school account)</span></span>|<span data-ttu-id="91777-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91777-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="91777-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91777-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91777-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91777-114">Not supported.</span></span>|
|<span data-ttu-id="91777-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91777-115">Application</span></span>|<span data-ttu-id="91777-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91777-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91777-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91777-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="91777-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91777-118">Request headers</span></span>
|<span data-ttu-id="91777-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91777-119">Header</span></span>|<span data-ttu-id="91777-120">値</span><span class="sxs-lookup"><span data-stu-id="91777-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91777-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91777-121">Authorization</span></span>|<span data-ttu-id="91777-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="91777-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91777-123">承諾</span><span class="sxs-lookup"><span data-stu-id="91777-123">Accept</span></span>|<span data-ttu-id="91777-124">application/json</span><span class="sxs-lookup"><span data-stu-id="91777-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91777-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="91777-125">Request body</span></span>
<span data-ttu-id="91777-126">要求本文で、iosVppApp オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="91777-126">In the request body, supply a JSON representation for the iosVppApp object.</span></span>

<span data-ttu-id="91777-127">次の表に、iosVppApp 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="91777-127">The following table shows the properties that are required when you create the iosVppApp.</span></span>

|<span data-ttu-id="91777-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91777-128">Property</span></span>|<span data-ttu-id="91777-129">型</span><span class="sxs-lookup"><span data-stu-id="91777-129">Type</span></span>|<span data-ttu-id="91777-130">説明</span><span class="sxs-lookup"><span data-stu-id="91777-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91777-131">id</span><span class="sxs-lookup"><span data-stu-id="91777-131">id</span></span>|<span data-ttu-id="91777-132">文字列</span><span class="sxs-lookup"><span data-stu-id="91777-132">String</span></span>|<span data-ttu-id="91777-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="91777-133">Key of the entity.</span></span> <span data-ttu-id="91777-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-135">displayName</span><span class="sxs-lookup"><span data-stu-id="91777-135">displayName</span></span>|<span data-ttu-id="91777-136">文字列</span><span class="sxs-lookup"><span data-stu-id="91777-136">String</span></span>|<span data-ttu-id="91777-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="91777-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="91777-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-139">description</span><span class="sxs-lookup"><span data-stu-id="91777-139">description</span></span>|<span data-ttu-id="91777-140">String</span><span class="sxs-lookup"><span data-stu-id="91777-140">String</span></span>|<span data-ttu-id="91777-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="91777-141">The description of the app.</span></span> <span data-ttu-id="91777-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-143">publisher</span><span class="sxs-lookup"><span data-stu-id="91777-143">publisher</span></span>|<span data-ttu-id="91777-144">String</span><span class="sxs-lookup"><span data-stu-id="91777-144">String</span></span>|<span data-ttu-id="91777-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="91777-145">The publisher of the app.</span></span> <span data-ttu-id="91777-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="91777-147">largeIcon</span></span>|[<span data-ttu-id="91777-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="91777-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="91777-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="91777-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="91777-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="91777-151">createdDateTime</span></span>|<span data-ttu-id="91777-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91777-152">DateTimeOffset</span></span>|<span data-ttu-id="91777-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="91777-153">The date and time the app was created.</span></span> <span data-ttu-id="91777-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="91777-155">lastModifiedDateTime</span></span>|<span data-ttu-id="91777-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91777-156">DateTimeOffset</span></span>|<span data-ttu-id="91777-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="91777-157">The date and time the app was last modified.</span></span> <span data-ttu-id="91777-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="91777-159">isFeatured</span></span>|<span data-ttu-id="91777-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="91777-160">Boolean</span></span>|<span data-ttu-id="91777-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="91777-162">privacyInformationUrl</span></span>|<span data-ttu-id="91777-163">String</span><span class="sxs-lookup"><span data-stu-id="91777-163">String</span></span>|<span data-ttu-id="91777-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="91777-164">The privacy statement Url.</span></span> <span data-ttu-id="91777-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="91777-166">informationUrl</span></span>|<span data-ttu-id="91777-167">String</span><span class="sxs-lookup"><span data-stu-id="91777-167">String</span></span>|<span data-ttu-id="91777-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="91777-168">The more information Url.</span></span> <span data-ttu-id="91777-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-170">owner</span><span class="sxs-lookup"><span data-stu-id="91777-170">owner</span></span>|<span data-ttu-id="91777-171">String</span><span class="sxs-lookup"><span data-stu-id="91777-171">String</span></span>|<span data-ttu-id="91777-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="91777-172">The owner of the app.</span></span> <span data-ttu-id="91777-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-174">developer</span><span class="sxs-lookup"><span data-stu-id="91777-174">developer</span></span>|<span data-ttu-id="91777-175">String</span><span class="sxs-lookup"><span data-stu-id="91777-175">String</span></span>|<span data-ttu-id="91777-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="91777-176">The developer of the app.</span></span> <span data-ttu-id="91777-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-178">notes</span><span class="sxs-lookup"><span data-stu-id="91777-178">notes</span></span>|<span data-ttu-id="91777-179">String</span><span class="sxs-lookup"><span data-stu-id="91777-179">String</span></span>|<span data-ttu-id="91777-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="91777-180">Notes for the app.</span></span> <span data-ttu-id="91777-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="91777-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="91777-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="91777-182">publishingState</span></span>|[<span data-ttu-id="91777-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="91777-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="91777-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="91777-184">The publishing state for the app.</span></span> <span data-ttu-id="91777-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="91777-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="91777-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="91777-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="91777-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="91777-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="91777-188">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="91777-188">usedLicenseCount</span></span>|<span data-ttu-id="91777-189">Int32</span><span class="sxs-lookup"><span data-stu-id="91777-189">Int32</span></span>|<span data-ttu-id="91777-190">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="91777-190">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="91777-191">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="91777-191">totalLicenseCount</span></span>|<span data-ttu-id="91777-192">Int32</span><span class="sxs-lookup"><span data-stu-id="91777-192">Int32</span></span>|<span data-ttu-id="91777-193">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="91777-193">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="91777-194">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="91777-194">releaseDateTime</span></span>|<span data-ttu-id="91777-195">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="91777-195">DateTimeOffset</span></span>|<span data-ttu-id="91777-196">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="91777-196">The VPP application release date and time.</span></span>|
|<span data-ttu-id="91777-197">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="91777-197">appStoreUrl</span></span>|<span data-ttu-id="91777-198">String</span><span class="sxs-lookup"><span data-stu-id="91777-198">String</span></span>|<span data-ttu-id="91777-199">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="91777-199">The store URL.</span></span>|
|<span data-ttu-id="91777-200">licensingType</span><span class="sxs-lookup"><span data-stu-id="91777-200">licensingType</span></span>|[<span data-ttu-id="91777-201">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="91777-201">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="91777-202">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="91777-202">The supported License Type.</span></span>|
|<span data-ttu-id="91777-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="91777-203">applicableDeviceType</span></span>|[<span data-ttu-id="91777-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="91777-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="91777-205">該当する iOS デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="91777-205">The applicable iOS Device Type.</span></span>|
|<span data-ttu-id="91777-206">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="91777-206">vppTokenOrganizationName</span></span>|<span data-ttu-id="91777-207">文字列</span><span class="sxs-lookup"><span data-stu-id="91777-207">String</span></span>|<span data-ttu-id="91777-208">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="91777-208">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="91777-209">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="91777-209">vppTokenAccountType</span></span>|[<span data-ttu-id="91777-210">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="91777-210">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="91777-211">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="91777-211">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="91777-212">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="91777-212">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="91777-213">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="91777-213">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="91777-214">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="91777-214">vppTokenAppleId</span></span>|<span data-ttu-id="91777-215">String</span><span class="sxs-lookup"><span data-stu-id="91777-215">String</span></span>|<span data-ttu-id="91777-216">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="91777-216">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="91777-217">bundleId</span><span class="sxs-lookup"><span data-stu-id="91777-217">bundleId</span></span>|<span data-ttu-id="91777-218">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="91777-218">String</span></span>|<span data-ttu-id="91777-219">ID 名。</span><span class="sxs-lookup"><span data-stu-id="91777-219">The Identity Name.</span></span>|



## <a name="response"></a><span data-ttu-id="91777-220">応答</span><span class="sxs-lookup"><span data-stu-id="91777-220">Response</span></span>
<span data-ttu-id="91777-221">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosVppApp](../resources/intune-apps-iosvppapp.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="91777-221">If successful, this method returns a `201 Created` response code and a [iosVppApp](../resources/intune-apps-iosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91777-222">例</span><span class="sxs-lookup"><span data-stu-id="91777-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="91777-223">要求</span><span class="sxs-lookup"><span data-stu-id="91777-223">Request</span></span>
<span data-ttu-id="91777-224">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91777-224">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="91777-225">応答</span><span class="sxs-lookup"><span data-stu-id="91777-225">Response</span></span>
<span data-ttu-id="91777-p116">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="91777-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



