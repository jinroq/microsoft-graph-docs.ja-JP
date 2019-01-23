---
title: OfficeSuiteApp を作成します。
description: 新しい officeSuiteApp オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c1821c88f974bf61fe23de6bb34cfeb06d9250f6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405843"
---
# <a name="create-officesuiteapp"></a><span data-ttu-id="51d9e-103">OfficeSuiteApp を作成します。</span><span class="sxs-lookup"><span data-stu-id="51d9e-103">Create officeSuiteApp</span></span>

> <span data-ttu-id="51d9e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="51d9e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="51d9e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51d9e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="51d9e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51d9e-107">新しい[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="51d9e-107">Create a new [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51d9e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="51d9e-108">Prerequisites</span></span>
<span data-ttu-id="51d9e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51d9e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51d9e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51d9e-111">Permission type</span></span>|<span data-ttu-id="51d9e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51d9e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51d9e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51d9e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51d9e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51d9e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51d9e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51d9e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51d9e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51d9e-116">Not supported.</span></span>|
|<span data-ttu-id="51d9e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51d9e-117">Application</span></span>|<span data-ttu-id="51d9e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51d9e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51d9e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51d9e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="51d9e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51d9e-120">Request headers</span></span>
|<span data-ttu-id="51d9e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51d9e-121">Header</span></span>|<span data-ttu-id="51d9e-122">値</span><span class="sxs-lookup"><span data-stu-id="51d9e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51d9e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="51d9e-123">Authorization</span></span>|<span data-ttu-id="51d9e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="51d9e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51d9e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="51d9e-125">Accept</span></span>|<span data-ttu-id="51d9e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51d9e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51d9e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="51d9e-127">Request body</span></span>
<span data-ttu-id="51d9e-128">要求の本文に officeSuiteApp オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="51d9e-128">In the request body, supply a JSON representation for the officeSuiteApp object.</span></span>

<span data-ttu-id="51d9e-129">次の表は、officeSuiteApp を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="51d9e-129">The following table shows the properties that are required when you create the officeSuiteApp.</span></span>

|<span data-ttu-id="51d9e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51d9e-130">Property</span></span>|<span data-ttu-id="51d9e-131">型</span><span class="sxs-lookup"><span data-stu-id="51d9e-131">Type</span></span>|<span data-ttu-id="51d9e-132">説明</span><span class="sxs-lookup"><span data-stu-id="51d9e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51d9e-133">id</span><span class="sxs-lookup"><span data-stu-id="51d9e-133">id</span></span>|<span data-ttu-id="51d9e-134">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-134">String</span></span>|<span data-ttu-id="51d9e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="51d9e-135">Key of the entity.</span></span> <span data-ttu-id="51d9e-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="51d9e-137">displayName</span></span>|<span data-ttu-id="51d9e-138">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-138">String</span></span>|<span data-ttu-id="51d9e-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="51d9e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="51d9e-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-141">説明</span><span class="sxs-lookup"><span data-stu-id="51d9e-141">description</span></span>|<span data-ttu-id="51d9e-142">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-142">String</span></span>|<span data-ttu-id="51d9e-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="51d9e-143">The description of the app.</span></span> <span data-ttu-id="51d9e-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="51d9e-145">publisher</span></span>|<span data-ttu-id="51d9e-146">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-146">String</span></span>|<span data-ttu-id="51d9e-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="51d9e-147">The publisher of the app.</span></span> <span data-ttu-id="51d9e-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="51d9e-149">largeIcon</span></span>|[<span data-ttu-id="51d9e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="51d9e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="51d9e-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="51d9e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="51d9e-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51d9e-153">createdDateTime</span></span>|<span data-ttu-id="51d9e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51d9e-154">DateTimeOffset</span></span>|<span data-ttu-id="51d9e-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="51d9e-155">The date and time the app was created.</span></span> <span data-ttu-id="51d9e-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51d9e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="51d9e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51d9e-158">DateTimeOffset</span></span>|<span data-ttu-id="51d9e-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="51d9e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="51d9e-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="51d9e-161">isFeatured</span></span>|<span data-ttu-id="51d9e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="51d9e-162">Boolean</span></span>|<span data-ttu-id="51d9e-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="51d9e-164">privacyInformationUrl</span></span>|<span data-ttu-id="51d9e-165">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-165">String</span></span>|<span data-ttu-id="51d9e-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="51d9e-166">The privacy statement Url.</span></span> <span data-ttu-id="51d9e-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="51d9e-168">informationUrl</span></span>|<span data-ttu-id="51d9e-169">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-169">String</span></span>|<span data-ttu-id="51d9e-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="51d9e-170">The more information Url.</span></span> <span data-ttu-id="51d9e-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-172">owner</span><span class="sxs-lookup"><span data-stu-id="51d9e-172">owner</span></span>|<span data-ttu-id="51d9e-173">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-173">String</span></span>|<span data-ttu-id="51d9e-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="51d9e-174">The owner of the app.</span></span> <span data-ttu-id="51d9e-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-176">developer</span><span class="sxs-lookup"><span data-stu-id="51d9e-176">developer</span></span>|<span data-ttu-id="51d9e-177">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-177">String</span></span>|<span data-ttu-id="51d9e-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="51d9e-178">The developer of the app.</span></span> <span data-ttu-id="51d9e-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-180">notes</span><span class="sxs-lookup"><span data-stu-id="51d9e-180">notes</span></span>|<span data-ttu-id="51d9e-181">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-181">String</span></span>|<span data-ttu-id="51d9e-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="51d9e-182">Notes for the app.</span></span> <span data-ttu-id="51d9e-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="51d9e-184">uploadState</span></span>|<span data-ttu-id="51d9e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="51d9e-185">Int32</span></span>|<span data-ttu-id="51d9e-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-186">The upload state.</span></span> <span data-ttu-id="51d9e-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="51d9e-188">publishingState</span></span>|[<span data-ttu-id="51d9e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="51d9e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="51d9e-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="51d9e-190">The publishing state for the app.</span></span> <span data-ttu-id="51d9e-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="51d9e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="51d9e-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="51d9e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="51d9e-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="51d9e-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="51d9e-194">isAssigned</span></span>|<span data-ttu-id="51d9e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="51d9e-195">Boolean</span></span>|<span data-ttu-id="51d9e-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="51d9e-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51d9e-198">roleScopeTagIds</span></span>|<span data-ttu-id="51d9e-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="51d9e-199">String collection</span></span>|<span data-ttu-id="51d9e-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="51d9e-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="51d9e-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="51d9e-202">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="51d9e-202">autoAcceptEula</span></span>|<span data-ttu-id="51d9e-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="51d9e-203">Boolean</span></span>|<span data-ttu-id="51d9e-204">エンド ・ ユーザーのデバイスに自動的に使用許諾契約書をそのまま使用する値。</span><span class="sxs-lookup"><span data-stu-id="51d9e-204">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="51d9e-205">productIds</span><span class="sxs-lookup"><span data-stu-id="51d9e-205">productIds</span></span>|<span data-ttu-id="51d9e-206">[officeProductId](../resources/intune-apps-officeproductid.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="51d9e-206">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="51d9e-207">Office365 スイート SKU を表すプロダクト Id です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-207">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="51d9e-208">可能な値は、`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail` です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-208">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="51d9e-209">excludedApps</span><span class="sxs-lookup"><span data-stu-id="51d9e-209">excludedApps</span></span>|[<span data-ttu-id="51d9e-210">excludedApps</span><span class="sxs-lookup"><span data-stu-id="51d9e-210">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="51d9e-211">選択した Office365 製品 id。 から除外されている場合、アプリケーションを表すためのプロパティ</span><span class="sxs-lookup"><span data-stu-id="51d9e-211">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="51d9e-212">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="51d9e-212">useSharedComputerActivation</span></span>|<span data-ttu-id="51d9e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="51d9e-213">Boolean</span></span>|<span data-ttu-id="51d9e-214">Office365 アプリケーション スイートではなく、共有のコンピューターのライセンス認証が使用されるかどうかを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="51d9e-214">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="51d9e-215">updateChannel</span><span class="sxs-lookup"><span data-stu-id="51d9e-215">updateChannel</span></span>|[<span data-ttu-id="51d9e-216">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="51d9e-216">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="51d9e-217">Office365 更新チャネルを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="51d9e-217">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="51d9e-218">可能な値は、`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred` です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-218">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="51d9e-219">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="51d9e-219">officePlatformArchitecture</span></span>|[<span data-ttu-id="51d9e-220">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="51d9e-220">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="51d9e-221">Office365 アプリケーション スイートのバージョンを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="51d9e-221">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="51d9e-222">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="51d9e-222">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="51d9e-223">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="51d9e-223">localesToInstall</span></span>|<span data-ttu-id="51d9e-224">String コレクション</span><span class="sxs-lookup"><span data-stu-id="51d9e-224">String collection</span></span>|<span data-ttu-id="51d9e-225">インストールされているロケールを表すプロパティ Office365 からアプリケーションがインストールされています。</span><span class="sxs-lookup"><span data-stu-id="51d9e-225">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="51d9e-226">標準の RFC 6033 を使用します。</span><span class="sxs-lookup"><span data-stu-id="51d9e-226">It uses standard RFC 6033.</span></span> <span data-ttu-id="51d9e-227">Ref。https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="51d9e-227">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="51d9e-228">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="51d9e-228">installProgressDisplayLevel</span></span>|[<span data-ttu-id="51d9e-229">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="51d9e-229">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="51d9e-230">デバイスのインストール中のセットアップの UI の表示のレベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="51d9e-230">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="51d9e-231">使用可能な値は、`none`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-231">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="51d9e-232">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="51d9e-232">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="51d9e-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="51d9e-233">Boolean</span></span>|<span data-ttu-id="51d9e-234">Office365 のアプリケーション スイートをかデバイスに配置する場合は、既存の Office MSI をアンインストールするかどうかを決定するプロパティ。</span><span class="sxs-lookup"><span data-stu-id="51d9e-234">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="51d9e-235">targetVersion</span><span class="sxs-lookup"><span data-stu-id="51d9e-235">targetVersion</span></span>|<span data-ttu-id="51d9e-236">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-236">String</span></span>|<span data-ttu-id="51d9e-237">デバイス上に配置されたままする必要があります Office365 アプリケーション スイートの特定のターゲットのバージョンを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="51d9e-237">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="51d9e-238">updateVersion</span><span class="sxs-lookup"><span data-stu-id="51d9e-238">updateVersion</span></span>|<span data-ttu-id="51d9e-239">String</span><span class="sxs-lookup"><span data-stu-id="51d9e-239">String</span></span>|<span data-ttu-id="51d9e-240">ターゲットの特定のバージョンで Office365 アプリケーション スイートの利用可能な更新プログラムのバージョンを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="51d9e-240">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|
|<span data-ttu-id="51d9e-241">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="51d9e-241">officeConfigurationXml</span></span>|<span data-ttu-id="51d9e-242">Binary</span><span class="sxs-lookup"><span data-stu-id="51d9e-242">Binary</span></span>|<span data-ttu-id="51d9e-243">Office 用リソースのアプリケーションに指定できる XML 構成ファイルを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="51d9e-243">The property to represent the XML configuration file that can be specified for Office ProPlus Apps.</span></span> <span data-ttu-id="51d9e-244">その他のすべてのプロパティに優先します。</span><span class="sxs-lookup"><span data-stu-id="51d9e-244">Takes precedence over all other properties.</span></span> <span data-ttu-id="51d9e-245">存在する場合、XML 構成ファイルを使用してアプリケーションを作成します。</span><span class="sxs-lookup"><span data-stu-id="51d9e-245">When present, the XML configuration file will be used to create the app.</span></span>|



## <a name="response"></a><span data-ttu-id="51d9e-246">応答</span><span class="sxs-lookup"><span data-stu-id="51d9e-246">Response</span></span>
<span data-ttu-id="51d9e-247">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="51d9e-247">If successful, this method returns a `201 Created` response code and a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51d9e-248">例</span><span class="sxs-lookup"><span data-stu-id="51d9e-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="51d9e-249">要求</span><span class="sxs-lookup"><span data-stu-id="51d9e-249">Request</span></span>
<span data-ttu-id="51d9e-250">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51d9e-250">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1552

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

### <a name="response"></a><span data-ttu-id="51d9e-251">応答</span><span class="sxs-lookup"><span data-stu-id="51d9e-251">Response</span></span>
<span data-ttu-id="51d9e-p125">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51d9e-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1724

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




