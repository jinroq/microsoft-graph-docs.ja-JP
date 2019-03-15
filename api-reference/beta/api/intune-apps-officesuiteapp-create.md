---
title: officeSuiteApp を作成する
description: 新しい officeSuiteApp オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e3fda805a19773351d791e4ae1f22b89ae0781a
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/14/2019
ms.locfileid: "30571789"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="b7c22-103">officeSuiteApp を作成する</span><span class="sxs-lookup"><span data-stu-id="b7c22-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="b7c22-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7c22-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7c22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7c22-106">新しい[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="b7c22-106">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7c22-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b7c22-107">Prerequisites</span></span>
<span data-ttu-id="b7c22-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7c22-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b7c22-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7c22-110">Permission type</span></span>|<span data-ttu-id="b7c22-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7c22-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7c22-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7c22-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7c22-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7c22-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b7c22-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7c22-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7c22-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c22-115">Not supported.</span></span>|
|<span data-ttu-id="b7c22-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7c22-116">Application</span></span>|<span data-ttu-id="b7c22-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7c22-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7c22-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7c22-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="b7c22-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7c22-119">Request headers</span></span>
|<span data-ttu-id="b7c22-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7c22-120">Header</span></span>|<span data-ttu-id="b7c22-121">値</span><span class="sxs-lookup"><span data-stu-id="b7c22-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7c22-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7c22-122">Authorization</span></span>|<span data-ttu-id="b7c22-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7c22-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7c22-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b7c22-124">Accept</span></span>|<span data-ttu-id="b7c22-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7c22-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7c22-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7c22-126">Request body</span></span>
<span data-ttu-id="b7c22-127">要求本文で、officeSuiteApp オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b7c22-127">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="b7c22-128">次の表に、officeSuiteApp の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b7c22-128">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="b7c22-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b7c22-129">Property</span></span>|<span data-ttu-id="b7c22-130">型</span><span class="sxs-lookup"><span data-stu-id="b7c22-130">Type</span></span>|<span data-ttu-id="b7c22-131">説明</span><span class="sxs-lookup"><span data-stu-id="b7c22-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7c22-132">id</span><span class="sxs-lookup"><span data-stu-id="b7c22-132">id</span></span>|<span data-ttu-id="b7c22-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="b7c22-133">String</span></span>|<span data-ttu-id="b7c22-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b7c22-134">Key of the entity.</span></span> <span data-ttu-id="b7c22-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b7c22-136">displayName</span></span>|<span data-ttu-id="b7c22-137">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-137">String</span></span>|<span data-ttu-id="b7c22-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="b7c22-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="b7c22-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-140">description</span><span class="sxs-lookup"><span data-stu-id="b7c22-140">description</span></span>|<span data-ttu-id="b7c22-141">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-141">String</span></span>|<span data-ttu-id="b7c22-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="b7c22-142">The description of the app.</span></span> <span data-ttu-id="b7c22-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-144">publisher</span><span class="sxs-lookup"><span data-stu-id="b7c22-144">publisher</span></span>|<span data-ttu-id="b7c22-145">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-145">String</span></span>|<span data-ttu-id="b7c22-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="b7c22-146">The publisher of the app.</span></span> <span data-ttu-id="b7c22-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="b7c22-148">largeIcon</span></span>|[<span data-ttu-id="b7c22-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="b7c22-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="b7c22-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="b7c22-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="b7c22-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7c22-152">createdDateTime</span></span>|<span data-ttu-id="b7c22-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7c22-153">DateTimeOffset</span></span>|<span data-ttu-id="b7c22-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b7c22-154">The date and time the app was created.</span></span> <span data-ttu-id="b7c22-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7c22-156">lastModifiedDateTime</span></span>|<span data-ttu-id="b7c22-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7c22-157">DateTimeOffset</span></span>|<span data-ttu-id="b7c22-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b7c22-158">The date and time the app was last modified.</span></span> <span data-ttu-id="b7c22-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="b7c22-160">isFeatured</span></span>|<span data-ttu-id="b7c22-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7c22-161">Boolean</span></span>|<span data-ttu-id="b7c22-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="b7c22-163">privacyInformationUrl</span></span>|<span data-ttu-id="b7c22-164">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-164">String</span></span>|<span data-ttu-id="b7c22-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="b7c22-165">The privacy statement Url.</span></span> <span data-ttu-id="b7c22-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="b7c22-167">informationUrl</span></span>|<span data-ttu-id="b7c22-168">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-168">String</span></span>|<span data-ttu-id="b7c22-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="b7c22-169">The more information Url.</span></span> <span data-ttu-id="b7c22-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-171">owner</span><span class="sxs-lookup"><span data-stu-id="b7c22-171">owner</span></span>|<span data-ttu-id="b7c22-172">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-172">String</span></span>|<span data-ttu-id="b7c22-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="b7c22-173">The owner of the app.</span></span> <span data-ttu-id="b7c22-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-175">developer</span><span class="sxs-lookup"><span data-stu-id="b7c22-175">developer</span></span>|<span data-ttu-id="b7c22-176">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-176">String</span></span>|<span data-ttu-id="b7c22-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="b7c22-177">The developer of the app.</span></span> <span data-ttu-id="b7c22-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-179">notes</span><span class="sxs-lookup"><span data-stu-id="b7c22-179">notes</span></span>|<span data-ttu-id="b7c22-180">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-180">String</span></span>|<span data-ttu-id="b7c22-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-181">Notes for the app.</span></span> <span data-ttu-id="b7c22-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="b7c22-183">uploadState</span></span>|<span data-ttu-id="b7c22-184">Int32</span><span class="sxs-lookup"><span data-stu-id="b7c22-184">Int32</span></span>|<span data-ttu-id="b7c22-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="b7c22-185">The upload state.</span></span> <span data-ttu-id="b7c22-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="b7c22-187">publishingState</span></span>|[<span data-ttu-id="b7c22-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="b7c22-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="b7c22-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="b7c22-189">The publishing state for the app.</span></span> <span data-ttu-id="b7c22-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="b7c22-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="b7c22-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="b7c22-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="b7c22-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="b7c22-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="b7c22-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b7c22-193">isAssigned</span></span>|<span data-ttu-id="b7c22-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7c22-194">Boolean</span></span>|<span data-ttu-id="b7c22-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="b7c22-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="b7c22-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b7c22-197">roleScopeTagIds</span></span>|<span data-ttu-id="b7c22-198">String collection</span><span class="sxs-lookup"><span data-stu-id="b7c22-198">String collection</span></span>|<span data-ttu-id="b7c22-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="b7c22-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="b7c22-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b7c22-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="b7c22-201">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="b7c22-201">autoAcceptEula</span></span>|<span data-ttu-id="b7c22-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7c22-202">Boolean</span></span>|<span data-ttu-id="b7c22-203">enduser のデバイスで EULA に自動的に同意する値。</span><span class="sxs-lookup"><span data-stu-id="b7c22-203">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="b7c22-204">productIds</span><span class="sxs-lookup"><span data-stu-id="b7c22-204">productIds</span></span>|<span data-ttu-id="b7c22-205">[officeproductid](../resources/intune-apps-officeproductid.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="b7c22-205">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="b7c22-206">Office365 スイート SKU を表す製品 id。</span><span class="sxs-lookup"><span data-stu-id="b7c22-206">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="b7c22-207">可能な値は、`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail` です。</span><span class="sxs-lookup"><span data-stu-id="b7c22-207">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="b7c22-208">excludedApps</span><span class="sxs-lookup"><span data-stu-id="b7c22-208">excludedApps</span></span>|[<span data-ttu-id="b7c22-209">excludedApps</span><span class="sxs-lookup"><span data-stu-id="b7c22-209">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="b7c22-210">選択した Office365 製品 Id から除外されるアプリを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-210">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="b7c22-211">。 usesharedcomputeractivation</span><span class="sxs-lookup"><span data-stu-id="b7c22-211">useSharedComputerActivation</span></span>|<span data-ttu-id="b7c22-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7c22-212">Boolean</span></span>|<span data-ttu-id="b7c22-213">office 365 アプリスイートに対して共有コンピューターのライセンス認証が使用されていないかどうかを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-213">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="b7c22-214">updateChannel</span><span class="sxs-lookup"><span data-stu-id="b7c22-214">updateChannel</span></span>|[<span data-ttu-id="b7c22-215">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="b7c22-215">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="b7c22-216">Office365 更新チャネルを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-216">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="b7c22-217">可能な値は、`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred` です。</span><span class="sxs-lookup"><span data-stu-id="b7c22-217">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="b7c22-218">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="b7c22-218">officePlatformArchitecture</span></span>|[<span data-ttu-id="b7c22-219">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="b7c22-219">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="b7c22-220">Office365 アプリスイートのバージョンを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-220">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="b7c22-221">可能な値は `none`、`x86`、`x64`、`arm`、`neutral`、`arm64` です。</span><span class="sxs-lookup"><span data-stu-id="b7c22-221">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="b7c22-222">次</span><span class="sxs-lookup"><span data-stu-id="b7c22-222">localesToInstall</span></span>|<span data-ttu-id="b7c22-223">String collection</span><span class="sxs-lookup"><span data-stu-id="b7c22-223">String collection</span></span>|<span data-ttu-id="b7c22-224">Office365 のアプリをインストールするときにインストールされるロケールを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-224">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="b7c22-225">標準の RFC 6033 を使用します。</span><span class="sxs-lookup"><span data-stu-id="b7c22-225">It uses standard RFC 6033.</span></span> <span data-ttu-id="b7c22-226">Refhttps://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="b7c22-226">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="b7c22-227">install進捗 displaylevel</span><span class="sxs-lookup"><span data-stu-id="b7c22-227">installProgressDisplayLevel</span></span>|[<span data-ttu-id="b7c22-228">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="b7c22-228">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="b7c22-229">デバイス上のインストールの進行状況のセットアップ UI の表示レベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="b7c22-229">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="b7c22-230">可能な値は、`none`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="b7c22-230">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="b7c22-231">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="b7c22-231">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="b7c22-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7c22-232">Boolean</span></span>|<span data-ttu-id="b7c22-233">Office365 アプリスイートがデバイスに展開されている場合に、既存の Office MSI をアンインストールするかどうかを決定するプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-233">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="b7c22-234">targetVersion</span><span class="sxs-lookup"><span data-stu-id="b7c22-234">targetVersion</span></span>|<span data-ttu-id="b7c22-235">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-235">String</span></span>|<span data-ttu-id="b7c22-236">デバイスに展開されたままにする必要がある、Office365 アプリスイートの特定のターゲットバージョンを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-236">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="b7c22-237">updateversion</span><span class="sxs-lookup"><span data-stu-id="b7c22-237">updateVersion</span></span>|<span data-ttu-id="b7c22-238">String</span><span class="sxs-lookup"><span data-stu-id="b7c22-238">String</span></span>|<span data-ttu-id="b7c22-239">Office365 アプリスイートで特定のターゲットバージョンが利用可能な更新バージョンを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-239">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="b7c22-240">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="b7c22-240">officeConfigurationXml</span></span>|<span data-ttu-id="b7c22-241">バイナリ</span><span class="sxs-lookup"><span data-stu-id="b7c22-241">Binary</span></span>|<span data-ttu-id="b7c22-242">Office ProPlus アプリに指定できる XML 構成ファイルを表すプロパティ。</span><span class="sxs-lookup"><span data-stu-id="b7c22-242">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="b7c22-243">他のすべてのプロパティより優先されます。</span><span class="sxs-lookup"><span data-stu-id="b7c22-243">Takes precedence over all other properties.</span></span> <span data-ttu-id="b7c22-244">指定した場合、XML 構成ファイルを使用してアプリが作成されます。</span><span class="sxs-lookup"><span data-stu-id="b7c22-244">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="b7c22-245">応答</span><span class="sxs-lookup"><span data-stu-id="b7c22-245">Response</span></span>
<span data-ttu-id="b7c22-246">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b7c22-246">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7c22-247">例</span><span class="sxs-lookup"><span data-stu-id="b7c22-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7c22-248">要求</span><span class="sxs-lookup"><span data-stu-id="b7c22-248">Request</span></span>
<span data-ttu-id="b7c22-249">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7c22-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1572

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

### <a name="response"></a><span data-ttu-id="b7c22-250">応答</span><span class="sxs-lookup"><span data-stu-id="b7c22-250">Response</span></span>
<span data-ttu-id="b7c22-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7c22-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1744

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




