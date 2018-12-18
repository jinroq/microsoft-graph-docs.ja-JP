---
title: OfficeSuiteApp を更新します。
description: OfficeSuiteApp オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 444bf90622d47d803a311e29d504dd8517369768
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337941"
---
# <a name="update-officesuiteapp"></a><span data-ttu-id="8e9af-103">OfficeSuiteApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="8e9af-103">Update officeSuiteApp</span></span>

> <span data-ttu-id="8e9af-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8e9af-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8e9af-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e9af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8e9af-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8e9af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8e9af-107">[OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8e9af-107">Update the properties of a [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8e9af-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8e9af-108">Prerequisites</span></span>
<span data-ttu-id="8e9af-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8e9af-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8e9af-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8e9af-111">Permission type</span></span>|<span data-ttu-id="8e9af-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8e9af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8e9af-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8e9af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8e9af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8e9af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8e9af-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8e9af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8e9af-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e9af-116">Not supported.</span></span>|
|<span data-ttu-id="8e9af-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8e9af-117">Application</span></span>|<span data-ttu-id="8e9af-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8e9af-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8e9af-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8e9af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="8e9af-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e9af-120">Request headers</span></span>
|<span data-ttu-id="8e9af-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8e9af-121">Header</span></span>|<span data-ttu-id="8e9af-122">値</span><span class="sxs-lookup"><span data-stu-id="8e9af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8e9af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="8e9af-123">Authorization</span></span>|<span data-ttu-id="8e9af-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8e9af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8e9af-125">Accept</span><span class="sxs-lookup"><span data-stu-id="8e9af-125">Accept</span></span>|<span data-ttu-id="8e9af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8e9af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8e9af-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="8e9af-127">Request body</span></span>
<span data-ttu-id="8e9af-128">要求の本文に[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="8e9af-128">In the request body, supply a JSON representation for the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object.</span></span>

<span data-ttu-id="8e9af-129">[OfficeSuiteApp](../resources/intune-apps-officesuiteapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="8e9af-129">The following table shows the properties that are required when you create the [officeSuiteApp](../resources/intune-apps-officesuiteapp.md).</span></span>

|<span data-ttu-id="8e9af-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8e9af-130">Property</span></span>|<span data-ttu-id="8e9af-131">種類</span><span class="sxs-lookup"><span data-stu-id="8e9af-131">Type</span></span>|<span data-ttu-id="8e9af-132">説明</span><span class="sxs-lookup"><span data-stu-id="8e9af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e9af-133">ID</span><span class="sxs-lookup"><span data-stu-id="8e9af-133">id</span></span>|<span data-ttu-id="8e9af-134">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-134">String</span></span>|<span data-ttu-id="8e9af-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8e9af-135">Key of the entity.</span></span> <span data-ttu-id="8e9af-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-137">displayName</span><span class="sxs-lookup"><span data-stu-id="8e9af-137">displayName</span></span>|<span data-ttu-id="8e9af-138">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-138">String</span></span>|<span data-ttu-id="8e9af-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="8e9af-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="8e9af-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-141">説明</span><span class="sxs-lookup"><span data-stu-id="8e9af-141">description</span></span>|<span data-ttu-id="8e9af-142">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-142">String</span></span>|<span data-ttu-id="8e9af-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="8e9af-143">The description of the app.</span></span> <span data-ttu-id="8e9af-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-145">publisher</span><span class="sxs-lookup"><span data-stu-id="8e9af-145">publisher</span></span>|<span data-ttu-id="8e9af-146">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-146">String</span></span>|<span data-ttu-id="8e9af-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="8e9af-147">The publisher of the app.</span></span> <span data-ttu-id="8e9af-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="8e9af-149">largeIcon</span></span>|[<span data-ttu-id="8e9af-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8e9af-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="8e9af-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="8e9af-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="8e9af-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8e9af-153">createdDateTime</span></span>|<span data-ttu-id="8e9af-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e9af-154">DateTimeOffset</span></span>|<span data-ttu-id="8e9af-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8e9af-155">The date and time the app was created.</span></span> <span data-ttu-id="8e9af-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8e9af-157">lastModifiedDateTime</span></span>|<span data-ttu-id="8e9af-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8e9af-158">DateTimeOffset</span></span>|<span data-ttu-id="8e9af-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8e9af-159">The date and time the app was last modified.</span></span> <span data-ttu-id="8e9af-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="8e9af-161">isFeatured</span></span>|<span data-ttu-id="8e9af-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="8e9af-162">Boolean</span></span>|<span data-ttu-id="8e9af-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="8e9af-164">privacyInformationUrl</span></span>|<span data-ttu-id="8e9af-165">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-165">String</span></span>|<span data-ttu-id="8e9af-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="8e9af-166">The privacy statement Url.</span></span> <span data-ttu-id="8e9af-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="8e9af-168">informationUrl</span></span>|<span data-ttu-id="8e9af-169">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-169">String</span></span>|<span data-ttu-id="8e9af-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="8e9af-170">The more information Url.</span></span> <span data-ttu-id="8e9af-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-172">owner</span><span class="sxs-lookup"><span data-stu-id="8e9af-172">owner</span></span>|<span data-ttu-id="8e9af-173">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-173">String</span></span>|<span data-ttu-id="8e9af-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="8e9af-174">The owner of the app.</span></span> <span data-ttu-id="8e9af-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-176">developer</span><span class="sxs-lookup"><span data-stu-id="8e9af-176">developer</span></span>|<span data-ttu-id="8e9af-177">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-177">String</span></span>|<span data-ttu-id="8e9af-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="8e9af-178">The developer of the app.</span></span> <span data-ttu-id="8e9af-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-180">notes</span><span class="sxs-lookup"><span data-stu-id="8e9af-180">notes</span></span>|<span data-ttu-id="8e9af-181">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-181">String</span></span>|<span data-ttu-id="8e9af-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="8e9af-182">Notes for the app.</span></span> <span data-ttu-id="8e9af-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="8e9af-184">uploadState</span></span>|<span data-ttu-id="8e9af-185">Int32</span><span class="sxs-lookup"><span data-stu-id="8e9af-185">Int32</span></span>|<span data-ttu-id="8e9af-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="8e9af-186">The upload state.</span></span> <span data-ttu-id="8e9af-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8e9af-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="8e9af-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="8e9af-188">publishingState</span></span>|[<span data-ttu-id="8e9af-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="8e9af-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="8e9af-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="8e9af-190">The publishing state for the app.</span></span> <span data-ttu-id="8e9af-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="8e9af-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="8e9af-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="8e9af-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="8e9af-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="8e9af-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="8e9af-194">autoAcceptEula</span><span class="sxs-lookup"><span data-stu-id="8e9af-194">autoAcceptEula</span></span>|<span data-ttu-id="8e9af-195">ブール型</span><span class="sxs-lookup"><span data-stu-id="8e9af-195">Boolean</span></span>|<span data-ttu-id="8e9af-196">エンド ・ ユーザーのデバイスに自動的に使用許諾契約書をそのまま使用する値。</span><span class="sxs-lookup"><span data-stu-id="8e9af-196">The value to accept the EULA automatically on the enduser's device.</span></span>|
|<span data-ttu-id="8e9af-197">productIds</span><span class="sxs-lookup"><span data-stu-id="8e9af-197">productIds</span></span>|<span data-ttu-id="8e9af-198">[officeProductId](../resources/intune-apps-officeproductid.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="8e9af-198">[officeProductId](../resources/intune-apps-officeproductid.md) collection</span></span>|<span data-ttu-id="8e9af-199">Office365 スイート SKU を表すプロダクト Id です。</span><span class="sxs-lookup"><span data-stu-id="8e9af-199">The Product Ids that represent the Office365 Suite SKU.</span></span> <span data-ttu-id="8e9af-200">可能な値は、`o365ProPlusRetail`、`o365BusinessRetail`、`visioProRetail`、`projectProRetail` です。</span><span class="sxs-lookup"><span data-stu-id="8e9af-200">Possible values are: `o365ProPlusRetail`, `o365BusinessRetail`, `visioProRetail`, `projectProRetail`.</span></span>|
|<span data-ttu-id="8e9af-201">excludedApps</span><span class="sxs-lookup"><span data-stu-id="8e9af-201">excludedApps</span></span>|[<span data-ttu-id="8e9af-202">excludedApps</span><span class="sxs-lookup"><span data-stu-id="8e9af-202">excludedApps</span></span>](../resources/intune-apps-excludedapps.md)|<span data-ttu-id="8e9af-203">選択した Office365 製品 id。 から除外されている場合、アプリケーションを表すためのプロパティ</span><span class="sxs-lookup"><span data-stu-id="8e9af-203">The property to represent the apps which are excluded from the selected Office365 Product Id.</span></span>|
|<span data-ttu-id="8e9af-204">useSharedComputerActivation</span><span class="sxs-lookup"><span data-stu-id="8e9af-204">useSharedComputerActivation</span></span>|<span data-ttu-id="8e9af-205">ブール型</span><span class="sxs-lookup"><span data-stu-id="8e9af-205">Boolean</span></span>|<span data-ttu-id="8e9af-206">Office365 アプリケーション スイートではなく、共有のコンピューターのライセンス認証が使用されるかどうかを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="8e9af-206">The property to represent that whether the shared computer activation is used not for Office365 app suite.</span></span>|
|<span data-ttu-id="8e9af-207">updateChannel</span><span class="sxs-lookup"><span data-stu-id="8e9af-207">updateChannel</span></span>|[<span data-ttu-id="8e9af-208">officeUpdateChannel</span><span class="sxs-lookup"><span data-stu-id="8e9af-208">officeUpdateChannel</span></span>](../resources/intune-apps-officeupdatechannel.md)|<span data-ttu-id="8e9af-209">Office365 更新チャネルを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="8e9af-209">The property to represent the Office365 Update Channel.</span></span> <span data-ttu-id="8e9af-210">可能な値は、`none`、`current`、`deferred`、`firstReleaseCurrent`、`firstReleaseDeferred` です。</span><span class="sxs-lookup"><span data-stu-id="8e9af-210">Possible values are: `none`, `current`, `deferred`, `firstReleaseCurrent`, `firstReleaseDeferred`.</span></span>|
|<span data-ttu-id="8e9af-211">officePlatformArchitecture</span><span class="sxs-lookup"><span data-stu-id="8e9af-211">officePlatformArchitecture</span></span>|[<span data-ttu-id="8e9af-212">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="8e9af-212">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="8e9af-213">Office365 アプリケーション スイートのバージョンを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="8e9af-213">The property to represent the Office365 app suite version.</span></span> <span data-ttu-id="8e9af-214">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="8e9af-214">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="8e9af-215">localesToInstall</span><span class="sxs-lookup"><span data-stu-id="8e9af-215">localesToInstall</span></span>|<span data-ttu-id="8e9af-216">String コレクション</span><span class="sxs-lookup"><span data-stu-id="8e9af-216">String collection</span></span>|<span data-ttu-id="8e9af-217">インストールされているロケールを表すプロパティ Office365 からアプリケーションがインストールされています。</span><span class="sxs-lookup"><span data-stu-id="8e9af-217">The property to represent the locales which are installed when the apps from Office365 is installed.</span></span> <span data-ttu-id="8e9af-218">標準の RFC 6033 を使用します。</span><span class="sxs-lookup"><span data-stu-id="8e9af-218">It uses standard RFC 6033.</span></span> <span data-ttu-id="8e9af-219">Ref。https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span><span class="sxs-lookup"><span data-stu-id="8e9af-219">Ref: https://technet.microsoft.com/en-us/library/cc179219(v=office.16).aspx</span></span>|
|<span data-ttu-id="8e9af-220">installProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="8e9af-220">installProgressDisplayLevel</span></span>|[<span data-ttu-id="8e9af-221">officeSuiteInstallProgressDisplayLevel</span><span class="sxs-lookup"><span data-stu-id="8e9af-221">officeSuiteInstallProgressDisplayLevel</span></span>](../resources/intune-apps-officesuiteinstallprogressdisplaylevel.md)|<span data-ttu-id="8e9af-222">デバイスのインストール中のセットアップの UI の表示のレベルを指定します。</span><span class="sxs-lookup"><span data-stu-id="8e9af-222">To specify the level of display for the Installation Progress Setup UI on the Device.</span></span> <span data-ttu-id="8e9af-223">使用可能な値は、`none`、`full` です。</span><span class="sxs-lookup"><span data-stu-id="8e9af-223">Possible values are: `none`, `full`.</span></span>|
|<span data-ttu-id="8e9af-224">shouldUninstallOlderVersionsOfOffice</span><span class="sxs-lookup"><span data-stu-id="8e9af-224">shouldUninstallOlderVersionsOfOffice</span></span>|<span data-ttu-id="8e9af-225">ブール型</span><span class="sxs-lookup"><span data-stu-id="8e9af-225">Boolean</span></span>|<span data-ttu-id="8e9af-226">Office365 のアプリケーション スイートをかデバイスに配置する場合は、既存の Office MSI をアンインストールするかどうかを決定するプロパティ。</span><span class="sxs-lookup"><span data-stu-id="8e9af-226">The property to determine whether to uninstall existing Office MSI if an Office365 app suite is deployed to the device or not.</span></span>|
|<span data-ttu-id="8e9af-227">targetVersion</span><span class="sxs-lookup"><span data-stu-id="8e9af-227">targetVersion</span></span>|<span data-ttu-id="8e9af-228">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-228">String</span></span>|<span data-ttu-id="8e9af-229">デバイス上に配置されたままする必要があります Office365 アプリケーション スイートの特定のターゲットのバージョンを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="8e9af-229">The property to represent the specific target version for the Office365 app suite that should be remained deployed on the devices.</span></span>|
|<span data-ttu-id="8e9af-230">updateVersion</span><span class="sxs-lookup"><span data-stu-id="8e9af-230">updateVersion</span></span>|<span data-ttu-id="8e9af-231">String</span><span class="sxs-lookup"><span data-stu-id="8e9af-231">String</span></span>|<span data-ttu-id="8e9af-232">ターゲットの特定のバージョンで Office365 アプリケーション スイートの利用可能な更新プログラムのバージョンを表すプロパティです。</span><span class="sxs-lookup"><span data-stu-id="8e9af-232">The property to represent the update version in which the specific target version is available for the Office365 app suite.</span></span>|



## <a name="response"></a><span data-ttu-id="8e9af-233">応答</span><span class="sxs-lookup"><span data-stu-id="8e9af-233">Response</span></span>
<span data-ttu-id="8e9af-234">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[officeSuiteApp](../resources/intune-apps-officesuiteapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8e9af-234">If successful, this method returns a `200 OK` response code and an updated [officeSuiteApp](../resources/intune-apps-officesuiteapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8e9af-235">例</span><span class="sxs-lookup"><span data-stu-id="8e9af-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="8e9af-236">要求</span><span class="sxs-lookup"><span data-stu-id="8e9af-236">Request</span></span>
<span data-ttu-id="8e9af-237">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8e9af-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1413

{
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
  "updateVersion": "Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="8e9af-238">応答</span><span class="sxs-lookup"><span data-stu-id="8e9af-238">Response</span></span>
<span data-ttu-id="8e9af-p122">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8e9af-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1574

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
  "updateVersion": "Update Version value"
}
```





