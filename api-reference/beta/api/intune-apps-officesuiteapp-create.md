---
title: OfficeSuiteApp を作成する
description: 新しい officeSuiteApp オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 664fc19eb20079c10352571e9d9d1cdb754bb7d8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960511"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="a8d05-103">OfficeSuiteApp を作成する</span><span class="sxs-lookup"><span data-stu-id="a8d05-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="a8d05-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8d05-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8d05-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8d05-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8d05-106">新しい[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a8d05-106">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8d05-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="a8d05-107">Prerequisites</span></span>
<span data-ttu-id="a8d05-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a8d05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8d05-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a8d05-110">Permission type</span></span>|<span data-ttu-id="a8d05-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a8d05-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8d05-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a8d05-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8d05-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8d05-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8d05-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a8d05-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8d05-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8d05-115">Not supported.</span></span>|
|<span data-ttu-id="a8d05-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a8d05-116">Application</span></span>|<span data-ttu-id="a8d05-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a8d05-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8d05-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a8d05-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="a8d05-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8d05-119">Request headers</span></span>
|<span data-ttu-id="a8d05-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a8d05-120">Header</span></span>|<span data-ttu-id="a8d05-121">値</span><span class="sxs-lookup"><span data-stu-id="a8d05-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8d05-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8d05-122">Authorization</span></span>|<span data-ttu-id="a8d05-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a8d05-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8d05-124">承諾</span><span class="sxs-lookup"><span data-stu-id="a8d05-124">Accept</span></span>|<span data-ttu-id="a8d05-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8d05-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8d05-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="a8d05-126">Request body</span></span>
<span data-ttu-id="a8d05-127">要求本文で、officeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a8d05-127">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="a8d05-128">次の表に、officeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a8d05-128">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="a8d05-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a8d05-129">Property</span></span>|<span data-ttu-id="a8d05-130">型</span><span class="sxs-lookup"><span data-stu-id="a8d05-130">Type</span></span>|<span data-ttu-id="a8d05-131">説明</span><span class="sxs-lookup"><span data-stu-id="a8d05-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8d05-132">id</span><span class="sxs-lookup"><span data-stu-id="a8d05-132">id</span></span>|<span data-ttu-id="a8d05-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a8d05-133">String</span></span>|<span data-ttu-id="a8d05-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a8d05-134">Key of the entity.</span></span> <span data-ttu-id="a8d05-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a8d05-136">displayName</span></span>|<span data-ttu-id="a8d05-137">文字列</span><span class="sxs-lookup"><span data-stu-id="a8d05-137">String</span></span>|<span data-ttu-id="a8d05-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="a8d05-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a8d05-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-140">description</span><span class="sxs-lookup"><span data-stu-id="a8d05-140">description</span></span>|<span data-ttu-id="a8d05-141">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-141">String</span></span>|<span data-ttu-id="a8d05-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="a8d05-142">The description of the app.</span></span> <span data-ttu-id="a8d05-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-144">publisher</span><span class="sxs-lookup"><span data-stu-id="a8d05-144">publisher</span></span>|<span data-ttu-id="a8d05-145">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-145">String</span></span>|<span data-ttu-id="a8d05-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="a8d05-146">The publisher of the app.</span></span> <span data-ttu-id="a8d05-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a8d05-148">largeIcon</span></span>|[<span data-ttu-id="a8d05-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a8d05-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a8d05-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="a8d05-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a8d05-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8d05-152">createdDateTime</span></span>|<span data-ttu-id="a8d05-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8d05-153">DateTimeOffset</span></span>|<span data-ttu-id="a8d05-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="a8d05-154">The date and time the app was created.</span></span> <span data-ttu-id="a8d05-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8d05-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a8d05-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8d05-157">DateTimeOffset</span></span>|<span data-ttu-id="a8d05-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="a8d05-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a8d05-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a8d05-160">isFeatured</span></span>|<span data-ttu-id="a8d05-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8d05-161">Boolean</span></span>|<span data-ttu-id="a8d05-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a8d05-163">privacyInformationUrl</span></span>|<span data-ttu-id="a8d05-164">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-164">String</span></span>|<span data-ttu-id="a8d05-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="a8d05-165">The privacy statement Url.</span></span> <span data-ttu-id="a8d05-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a8d05-167">informationUrl</span></span>|<span data-ttu-id="a8d05-168">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-168">String</span></span>|<span data-ttu-id="a8d05-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="a8d05-169">The more information Url.</span></span> <span data-ttu-id="a8d05-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-171">owner</span><span class="sxs-lookup"><span data-stu-id="a8d05-171">owner</span></span>|<span data-ttu-id="a8d05-172">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-172">String</span></span>|<span data-ttu-id="a8d05-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="a8d05-173">The owner of the app.</span></span> <span data-ttu-id="a8d05-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-175">developer</span><span class="sxs-lookup"><span data-stu-id="a8d05-175">developer</span></span>|<span data-ttu-id="a8d05-176">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-176">String</span></span>|<span data-ttu-id="a8d05-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="a8d05-177">The developer of the app.</span></span> <span data-ttu-id="a8d05-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-179">notes</span><span class="sxs-lookup"><span data-stu-id="a8d05-179">notes</span></span>|<span data-ttu-id="a8d05-180">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-180">String</span></span>|<span data-ttu-id="a8d05-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-181">Notes for the app.</span></span> <span data-ttu-id="a8d05-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="a8d05-183">uploadState</span></span>|<span data-ttu-id="a8d05-184">Int32</span><span class="sxs-lookup"><span data-stu-id="a8d05-184">Int32</span></span>|<span data-ttu-id="a8d05-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="a8d05-185">The upload state.</span></span> <span data-ttu-id="a8d05-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="a8d05-187">publishingState</span></span>|[<span data-ttu-id="a8d05-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a8d05-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a8d05-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="a8d05-189">The publishing state for the app.</span></span> <span data-ttu-id="a8d05-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="a8d05-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a8d05-191">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a8d05-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a8d05-192">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="a8d05-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a8d05-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a8d05-193">isAssigned</span></span>|<span data-ttu-id="a8d05-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8d05-194">Boolean</span></span>|<span data-ttu-id="a8d05-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="a8d05-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a8d05-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8d05-197">roleScopeTagIds</span></span>|<span data-ttu-id="a8d05-198">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a8d05-198">String collection</span></span>|<span data-ttu-id="a8d05-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="a8d05-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a8d05-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-201">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="a8d05-201">dependentAppCount</span></span>|<span data-ttu-id="a8d05-202">Int32</span><span class="sxs-lookup"><span data-stu-id="a8d05-202">Int32</span></span>|<span data-ttu-id="a8d05-203">子アプリが持つ依存関係の合計数。</span><span class="sxs-lookup"><span data-stu-id="a8d05-203">The total number of dependencies the child app has.</span></span> <span data-ttu-id="a8d05-204">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a8d05-204">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a8d05-205">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="a8d05-205">autoAcceptEula</span></span>|<span data-ttu-id="a8d05-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8d05-206">Boolean</span></span>|<span data-ttu-id="a8d05-207">Enduser のデバイスで EULA に自動的に同意する値。</span><span class="sxs-lookup"><span data-stu-id="a8d05-207">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="a8d05-208">productIds</span><span class="sxs-lookup"><span data-stu-id="a8d05-208">productIds</span></span>|<span data-ttu-id="a8d05-209">[Officeproductid](../resources/intune-apps-officeproductid.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="a8d05-209">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="a8d05-210">Office365 スイート SKU を表す製品 Id。</span><span class="sxs-lookup"><span data-stu-id="a8d05-210">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="a8d05-211">使用可能な値は、`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail` です。</span><span class="sxs-lookup"><span data-stu-id="a8d05-211">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="a8d05-212">excludedApps</span><span class="sxs-lookup"><span data-stu-id="a8d05-212">excludedApps</span></span>|[<span data-ttu-id="a8d05-213">excludedApps</span><span class="sxs-lookup"><span data-stu-id="a8d05-213">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="a8d05-214">選択した Office365 製品 Id から除外されるアプリを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-214">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="a8d05-215">。 Usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="a8d05-215">useSharedComputerActivation</span></span>|<span data-ttu-id="a8d05-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8d05-216">Boolean</span></span>|<span data-ttu-id="a8d05-217">Office 365 アプリスイートに対して共有コンピューターのライセンス認証が使用されていないかどうかを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-217">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="a8d05-218">updateChannel</span><span class="sxs-lookup"><span data-stu-id="a8d05-218">updateChannel</span></span>|[<span data-ttu-id="a8d05-219">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="a8d05-219">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="a8d05-220">Office365 更新チャネルを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-220">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="a8d05-221">可能な値は、`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred` です。</span><span class="sxs-lookup"><span data-stu-id="a8d05-221">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="a8d05-222">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="a8d05-222">officePlatformArchitecture</span></span>|[<span data-ttu-id="a8d05-223">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a8d05-223">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a8d05-224">Office365 アプリスイートのバージョンを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-224">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="a8d05-225">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="a8d05-225">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="a8d05-226">次</span><span class="sxs-lookup"><span data-stu-id="a8d05-226">localesToInstall</span></span>|<span data-ttu-id="a8d05-227">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="a8d05-227">String collection</span></span>|<span data-ttu-id="a8d05-228">Office365 のアプリをインストールするときにインストールされるロケールを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-228">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="a8d05-229">標準の RFC 6033 を使用します。</span><span class="sxs-lookup"><span data-stu-id="a8d05-229">It uses standard RFC 6033.</span></span> <span data-ttu-id="a8d05-230">Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="a8d05-230">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="a8d05-231">Install進捗 Displaylevel</span><span class="sxs-lookup"><span data-stu-id="a8d05-231">installProgressDisplayLevel</span></span>|[<span data-ttu-id="a8d05-232">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="a8d05-232">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="a8d05-233">デバイス上のインストールの進行状況のセットアップ UI の表示レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="a8d05-233">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="a8d05-234">可能な値は、`none`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="a8d05-234">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="a8d05-235">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="a8d05-235">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="a8d05-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8d05-236">Boolean</span></span>|<span data-ttu-id="a8d05-237">Office365 アプリスイートがデバイスに展開されている場合に、既存の Office MSI をアンインストールするかどうかを決定するプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-237">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="a8d05-238">targetVersion</span><span class="sxs-lookup"><span data-stu-id="a8d05-238">targetVersion</span></span>|<span data-ttu-id="a8d05-239">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-239">String</span></span>|<span data-ttu-id="a8d05-240">デバイスに展開されたままにする必要がある、Office365 アプリスイートの特定のターゲットバージョンを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-240">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="a8d05-241">updateVersion</span><span class="sxs-lookup"><span data-stu-id="a8d05-241">updateVersion</span></span>|<span data-ttu-id="a8d05-242">String</span><span class="sxs-lookup"><span data-stu-id="a8d05-242">String</span></span>|<span data-ttu-id="a8d05-243">Office365 アプリスイートで特定のターゲットバージョンが利用可能な更新バージョンを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-243">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="a8d05-244">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="a8d05-244">officeConfigurationXml</span></span>|<span data-ttu-id="a8d05-245">Binary</span><span class="sxs-lookup"><span data-stu-id="a8d05-245">Binary</span></span>|<span data-ttu-id="a8d05-246">Office ProPlus アプリに指定できる XML 構成ファイルを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="a8d05-246">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="a8d05-247">他のすべてのプロパティより優先されます。</span><span class="sxs-lookup"><span data-stu-id="a8d05-247">Takes precedence over all other properties.</span></span> <span data-ttu-id="a8d05-248">指定した場合、XML 構成ファイルを使用してアプリが作成されます。</span><span class="sxs-lookup"><span data-stu-id="a8d05-248">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="a8d05-249">応答</span><span class="sxs-lookup"><span data-stu-id="a8d05-249">Response</span></span>
<span data-ttu-id="a8d05-250">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a8d05-250">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8d05-251">例</span><span class="sxs-lookup"><span data-stu-id="a8d05-251">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8d05-252">要求</span><span class="sxs-lookup"><span data-stu-id="a8d05-252">Request</span></span>
<span data-ttu-id="a8d05-253">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a8d05-253">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1599

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
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
  "dependentAppCount": 1,
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="a8d05-254">応答</span><span class="sxs-lookup"><span data-stu-id="a8d05-254">Response</span></span>
<span data-ttu-id="a8d05-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a8d05-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1771

{
  "@odata.type": "#microsoft.graph.officeSuiteApp",
  "id": "9b263b46-3b46-9b26-463b-269b463b269b",
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
  "dependentAppCount": 1,
  "autoAcceptEula": true,
  "productIds": [
    "o365BusinessRetail"
  ],
  "excludedApps": {
    "@odata.type": "microsoft.graph.excludedApps",
    "access": true,
    "excel": true,
    "groove": true,
    "infoPath": true,
    "lync": true,
    "oneDrive": true,
    "oneNote": true,
    "outlook": true,
    "powerPoint": true,
    "publisher": true,
    "sharePointDesigner": true,
    "teams": true,
    "visio": true,
    "word": true
  },
  "useSharedComputerActivation": true,
  "updateChannel": "current",
  "officePlatformArchitecture": "x86",
  "localesToInstall": [
    "Locales To Install value"
  ],
  "installProgressDisplayLevel": "full",
  "shouldUninstallOlderVersionsOfOffice": true,
  "targetVersion": "Target Version value",
  "updateVersion": "Update Version value",
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```





