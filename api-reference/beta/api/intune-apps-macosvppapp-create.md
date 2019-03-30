---
title: macOsVppApp を作成する
description: 新しい macOsVppApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69507bf37e0f06a952ff56eb808c0e4f85cc647e
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30987231"
---
# <a name="create-macosvppapp"></a><span data-ttu-id="31aa7-103">macOsVppApp を作成する</span><span class="sxs-lookup"><span data-stu-id="31aa7-103">Create macOsVppApp</span></span>

> <span data-ttu-id="31aa7-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31aa7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="31aa7-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="31aa7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="31aa7-106">新しい[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="31aa7-106">Create a new [macOsVppApp](../resources/intune-apps-macosvppapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="31aa7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="31aa7-107">Prerequisites</span></span>
<span data-ttu-id="31aa7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31aa7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="31aa7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="31aa7-110">Permission type</span></span>|<span data-ttu-id="31aa7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="31aa7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="31aa7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="31aa7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="31aa7-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="31aa7-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="31aa7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="31aa7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="31aa7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31aa7-115">Not supported.</span></span>|
|<span data-ttu-id="31aa7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="31aa7-116">Application</span></span>|<span data-ttu-id="31aa7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31aa7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="31aa7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="31aa7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="31aa7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31aa7-119">Request headers</span></span>
|<span data-ttu-id="31aa7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="31aa7-120">Header</span></span>|<span data-ttu-id="31aa7-121">値</span><span class="sxs-lookup"><span data-stu-id="31aa7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="31aa7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="31aa7-122">Authorization</span></span>|<span data-ttu-id="31aa7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="31aa7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="31aa7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="31aa7-124">Accept</span></span>|<span data-ttu-id="31aa7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="31aa7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="31aa7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="31aa7-126">Request body</span></span>
<span data-ttu-id="31aa7-127">要求本文で、macOsVppApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="31aa7-127">In the request body, supply a JSON representation for the macOsVppApp object.</span></span>

<span data-ttu-id="31aa7-128">次の表に、macOsVppApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="31aa7-128">The following table shows the properties that are required when you create the macOsVppApp.</span></span>

|<span data-ttu-id="31aa7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31aa7-129">Property</span></span>|<span data-ttu-id="31aa7-130">型</span><span class="sxs-lookup"><span data-stu-id="31aa7-130">Type</span></span>|<span data-ttu-id="31aa7-131">説明</span><span class="sxs-lookup"><span data-stu-id="31aa7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="31aa7-132">id</span><span class="sxs-lookup"><span data-stu-id="31aa7-132">id</span></span>|<span data-ttu-id="31aa7-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="31aa7-133">String</span></span>|<span data-ttu-id="31aa7-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="31aa7-134">Key of the entity.</span></span> <span data-ttu-id="31aa7-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-136">displayName</span><span class="sxs-lookup"><span data-stu-id="31aa7-136">displayName</span></span>|<span data-ttu-id="31aa7-137">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-137">String</span></span>|<span data-ttu-id="31aa7-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="31aa7-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="31aa7-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-140">description</span><span class="sxs-lookup"><span data-stu-id="31aa7-140">description</span></span>|<span data-ttu-id="31aa7-141">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-141">String</span></span>|<span data-ttu-id="31aa7-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="31aa7-142">The description of the app.</span></span> <span data-ttu-id="31aa7-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-144">publisher</span><span class="sxs-lookup"><span data-stu-id="31aa7-144">publisher</span></span>|<span data-ttu-id="31aa7-145">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-145">String</span></span>|<span data-ttu-id="31aa7-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="31aa7-146">The publisher of the app.</span></span> <span data-ttu-id="31aa7-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="31aa7-148">largeIcon</span></span>|[<span data-ttu-id="31aa7-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="31aa7-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="31aa7-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="31aa7-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="31aa7-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="31aa7-152">createdDateTime</span></span>|<span data-ttu-id="31aa7-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31aa7-153">DateTimeOffset</span></span>|<span data-ttu-id="31aa7-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="31aa7-154">The date and time the app was created.</span></span> <span data-ttu-id="31aa7-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="31aa7-156">lastModifiedDateTime</span></span>|<span data-ttu-id="31aa7-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31aa7-157">DateTimeOffset</span></span>|<span data-ttu-id="31aa7-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="31aa7-158">The date and time the app was last modified.</span></span> <span data-ttu-id="31aa7-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="31aa7-160">isFeatured</span></span>|<span data-ttu-id="31aa7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="31aa7-161">Boolean</span></span>|<span data-ttu-id="31aa7-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="31aa7-163">privacyInformationUrl</span></span>|<span data-ttu-id="31aa7-164">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-164">String</span></span>|<span data-ttu-id="31aa7-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="31aa7-165">The privacy statement Url.</span></span> <span data-ttu-id="31aa7-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="31aa7-167">informationUrl</span></span>|<span data-ttu-id="31aa7-168">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-168">String</span></span>|<span data-ttu-id="31aa7-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="31aa7-169">The more information Url.</span></span> <span data-ttu-id="31aa7-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-171">owner</span><span class="sxs-lookup"><span data-stu-id="31aa7-171">owner</span></span>|<span data-ttu-id="31aa7-172">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-172">String</span></span>|<span data-ttu-id="31aa7-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="31aa7-173">The owner of the app.</span></span> <span data-ttu-id="31aa7-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-175">developer</span><span class="sxs-lookup"><span data-stu-id="31aa7-175">developer</span></span>|<span data-ttu-id="31aa7-176">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-176">String</span></span>|<span data-ttu-id="31aa7-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="31aa7-177">The developer of the app.</span></span> <span data-ttu-id="31aa7-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-179">notes</span><span class="sxs-lookup"><span data-stu-id="31aa7-179">notes</span></span>|<span data-ttu-id="31aa7-180">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-180">String</span></span>|<span data-ttu-id="31aa7-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="31aa7-181">Notes for the app.</span></span> <span data-ttu-id="31aa7-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="31aa7-183">uploadState</span></span>|<span data-ttu-id="31aa7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="31aa7-184">Int32</span></span>|<span data-ttu-id="31aa7-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="31aa7-185">The upload state.</span></span> <span data-ttu-id="31aa7-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="31aa7-187">publishingState</span></span>|[<span data-ttu-id="31aa7-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="31aa7-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="31aa7-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="31aa7-189">The publishing state for the app.</span></span> <span data-ttu-id="31aa7-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="31aa7-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="31aa7-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="31aa7-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="31aa7-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="31aa7-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="31aa7-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="31aa7-193">isAssigned</span></span>|<span data-ttu-id="31aa7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="31aa7-194">Boolean</span></span>|<span data-ttu-id="31aa7-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="31aa7-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="31aa7-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="31aa7-197">roleScopeTagIds</span></span>|<span data-ttu-id="31aa7-198">String collection</span><span class="sxs-lookup"><span data-stu-id="31aa7-198">String collection</span></span>|<span data-ttu-id="31aa7-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="31aa7-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="31aa7-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="31aa7-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="31aa7-201">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="31aa7-201">usedLicenseCount</span></span>|<span data-ttu-id="31aa7-202">Int32</span><span class="sxs-lookup"><span data-stu-id="31aa7-202">Int32</span></span>|<span data-ttu-id="31aa7-203">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="31aa7-203">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="31aa7-204">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="31aa7-204">totalLicenseCount</span></span>|<span data-ttu-id="31aa7-205">Int32</span><span class="sxs-lookup"><span data-stu-id="31aa7-205">Int32</span></span>|<span data-ttu-id="31aa7-206">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="31aa7-206">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="31aa7-207">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="31aa7-207">releaseDateTime</span></span>|<span data-ttu-id="31aa7-208">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31aa7-208">DateTimeOffset</span></span>|<span data-ttu-id="31aa7-209">VPP アプリケーションのリリースの日時。</span><span class="sxs-lookup"><span data-stu-id="31aa7-209">The VPP application release date and time.</span></span>|
|<span data-ttu-id="31aa7-210">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="31aa7-210">appStoreUrl</span></span>|<span data-ttu-id="31aa7-211">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-211">String</span></span>|<span data-ttu-id="31aa7-212">ストアの URL。</span><span class="sxs-lookup"><span data-stu-id="31aa7-212">The store URL.</span></span>|
|<span data-ttu-id="31aa7-213">licensingType</span><span class="sxs-lookup"><span data-stu-id="31aa7-213">licensingType</span></span>|[<span data-ttu-id="31aa7-214">vppLicensingType</span><span class="sxs-lookup"><span data-stu-id="31aa7-214">vppLicensingType</span></span>](../resources/intune-apps-vpplicensingtype.md)|<span data-ttu-id="31aa7-215">サポートされているライセンスの種類。</span><span class="sxs-lookup"><span data-stu-id="31aa7-215">The supported License Type.</span></span>|
|<span data-ttu-id="31aa7-216">vppTokenOrganizationName</span><span class="sxs-lookup"><span data-stu-id="31aa7-216">vppTokenOrganizationName</span></span>|<span data-ttu-id="31aa7-217">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-217">String</span></span>|<span data-ttu-id="31aa7-218">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="31aa7-218">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="31aa7-219">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="31aa7-219">vppTokenAccountType</span></span>|[<span data-ttu-id="31aa7-220">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="31aa7-220">vppTokenAccountType</span></span>](../resources/intune-shared-vpptokenaccounttype.md)|<span data-ttu-id="31aa7-221">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="31aa7-221">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="31aa7-222">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="31aa7-222">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="31aa7-223">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="31aa7-223">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="31aa7-224">vppTokenAppleId</span><span class="sxs-lookup"><span data-stu-id="31aa7-224">vppTokenAppleId</span></span>|<span data-ttu-id="31aa7-225">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-225">String</span></span>|<span data-ttu-id="31aa7-226">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="31aa7-226">The Apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="31aa7-227">bundleId</span><span class="sxs-lookup"><span data-stu-id="31aa7-227">bundleId</span></span>|<span data-ttu-id="31aa7-228">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="31aa7-228">String</span></span>|<span data-ttu-id="31aa7-229">ID 名。</span><span class="sxs-lookup"><span data-stu-id="31aa7-229">The Identity Name.</span></span>|
|<span data-ttu-id="31aa7-230">vppTokenId</span><span class="sxs-lookup"><span data-stu-id="31aa7-230">vppTokenId</span></span>|<span data-ttu-id="31aa7-231">String</span><span class="sxs-lookup"><span data-stu-id="31aa7-231">String</span></span>|<span data-ttu-id="31aa7-232">このアプリに関連付けられている VPP トークンの識別子。</span><span class="sxs-lookup"><span data-stu-id="31aa7-232">Identifier of the VPP token associated with this app.</span></span>|
|<span data-ttu-id="31aa7-233">revokeLicenseActionResults</span><span class="sxs-lookup"><span data-stu-id="31aa7-233">revokeLicenseActionResults</span></span>|<span data-ttu-id="31aa7-234">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="31aa7-234">[macOsVppAppRevokeLicensesActionResult](../resources/intune-apps-macosvppapprevokelicensesactionresult.md) collection</span></span>|<span data-ttu-id="31aa7-235">このアプリでのライセンスの取り消しアクションの結果。</span><span class="sxs-lookup"><span data-stu-id="31aa7-235">Results of revoke license actions on this app.</span></span>|



## <a name="response"></a><span data-ttu-id="31aa7-236">応答</span><span class="sxs-lookup"><span data-stu-id="31aa7-236">Response</span></span>
<span data-ttu-id="31aa7-237">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[macOsVppApp](../resources/intune-apps-macosvppapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="31aa7-237">If successful, this method returns a `201 Created` response code and a [macOsVppApp](../resources/intune-apps-macosvppapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="31aa7-238">例</span><span class="sxs-lookup"><span data-stu-id="31aa7-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="31aa7-239">要求</span><span class="sxs-lookup"><span data-stu-id="31aa7-239">Request</span></span>
<span data-ttu-id="31aa7-240">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="31aa7-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1842

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
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
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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

### <a name="response"></a><span data-ttu-id="31aa7-241">応答</span><span class="sxs-lookup"><span data-stu-id="31aa7-241">Response</span></span>
<span data-ttu-id="31aa7-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="31aa7-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2014

{
  "@odata.type": "#microsoft.graph.macOsVppApp",
  "id": "10b95265-5265-10b9-6552-b9106552b910",
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
  "vppTokenOrganizationName": "Vpp Token Organization Name value",
  "vppTokenAccountType": "education",
  "vppTokenAppleId": "Vpp Token Apple Id value",
  "bundleId": "Bundle Id value",
  "vppTokenId": "Vpp Token Id value",
  "revokeLicenseActionResults": [
    {
      "@odata.type": "microsoft.graph.macOsVppAppRevokeLicensesActionResult",
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




