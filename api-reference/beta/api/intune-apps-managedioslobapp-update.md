---
title: managedIOSLobApp の更新
description: managedIOSLobApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: aa276827960b0ac0b73489402ac7ba309c58c098
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412927"
---
# <a name="update-managedioslobapp"></a><span data-ttu-id="ac86e-103">managedIOSLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="ac86e-103">Update managedIOSLobApp</span></span>

> <span data-ttu-id="ac86e-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ac86e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ac86e-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac86e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ac86e-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ac86e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac86e-107">[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ac86e-107">Update the properties of a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac86e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ac86e-108">Prerequisites</span></span>
<span data-ttu-id="ac86e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ac86e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ac86e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ac86e-111">Permission type</span></span>|<span data-ttu-id="ac86e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ac86e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac86e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ac86e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ac86e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac86e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ac86e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ac86e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac86e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac86e-116">Not supported.</span></span>|
|<span data-ttu-id="ac86e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ac86e-117">Application</span></span>|<span data-ttu-id="ac86e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ac86e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac86e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ac86e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="ac86e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac86e-120">Request headers</span></span>
|<span data-ttu-id="ac86e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ac86e-121">Header</span></span>|<span data-ttu-id="ac86e-122">値</span><span class="sxs-lookup"><span data-stu-id="ac86e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac86e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac86e-123">Authorization</span></span>|<span data-ttu-id="ac86e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ac86e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac86e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ac86e-125">Accept</span></span>|<span data-ttu-id="ac86e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ac86e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac86e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ac86e-127">Request body</span></span>
<span data-ttu-id="ac86e-128">要求本文で、[managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ac86e-128">In the request body, supply a JSON representation for the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

<span data-ttu-id="ac86e-129">次の表に、[managedDeviceOverview](../resources/intune-apps-managedioslobapp.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ac86e-129">The following table shows the properties that are required when you create the [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span></span>

|<span data-ttu-id="ac86e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac86e-130">Property</span></span>|<span data-ttu-id="ac86e-131">型</span><span class="sxs-lookup"><span data-stu-id="ac86e-131">Type</span></span>|<span data-ttu-id="ac86e-132">説明</span><span class="sxs-lookup"><span data-stu-id="ac86e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac86e-133">id</span><span class="sxs-lookup"><span data-stu-id="ac86e-133">id</span></span>|<span data-ttu-id="ac86e-134">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-134">String</span></span>|<span data-ttu-id="ac86e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ac86e-135">Key of the entity.</span></span> <span data-ttu-id="ac86e-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ac86e-137">displayName</span></span>|<span data-ttu-id="ac86e-138">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-138">String</span></span>|<span data-ttu-id="ac86e-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="ac86e-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ac86e-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-141">説明</span><span class="sxs-lookup"><span data-stu-id="ac86e-141">description</span></span>|<span data-ttu-id="ac86e-142">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-142">String</span></span>|<span data-ttu-id="ac86e-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="ac86e-143">The description of the app.</span></span> <span data-ttu-id="ac86e-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ac86e-145">publisher</span></span>|<span data-ttu-id="ac86e-146">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-146">String</span></span>|<span data-ttu-id="ac86e-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="ac86e-147">The publisher of the app.</span></span> <span data-ttu-id="ac86e-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ac86e-149">largeIcon</span></span>|[<span data-ttu-id="ac86e-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ac86e-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ac86e-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="ac86e-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ac86e-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ac86e-153">createdDateTime</span></span>|<span data-ttu-id="ac86e-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac86e-154">DateTimeOffset</span></span>|<span data-ttu-id="ac86e-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ac86e-155">The date and time the app was created.</span></span> <span data-ttu-id="ac86e-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ac86e-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ac86e-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac86e-158">DateTimeOffset</span></span>|<span data-ttu-id="ac86e-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ac86e-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ac86e-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ac86e-161">isFeatured</span></span>|<span data-ttu-id="ac86e-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac86e-162">Boolean</span></span>|<span data-ttu-id="ac86e-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ac86e-164">privacyInformationUrl</span></span>|<span data-ttu-id="ac86e-165">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-165">String</span></span>|<span data-ttu-id="ac86e-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="ac86e-166">The privacy statement Url.</span></span> <span data-ttu-id="ac86e-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ac86e-168">informationUrl</span></span>|<span data-ttu-id="ac86e-169">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-169">String</span></span>|<span data-ttu-id="ac86e-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="ac86e-170">The more information Url.</span></span> <span data-ttu-id="ac86e-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-172">owner</span><span class="sxs-lookup"><span data-stu-id="ac86e-172">owner</span></span>|<span data-ttu-id="ac86e-173">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-173">String</span></span>|<span data-ttu-id="ac86e-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="ac86e-174">The owner of the app.</span></span> <span data-ttu-id="ac86e-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-176">developer</span><span class="sxs-lookup"><span data-stu-id="ac86e-176">developer</span></span>|<span data-ttu-id="ac86e-177">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-177">String</span></span>|<span data-ttu-id="ac86e-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="ac86e-178">The developer of the app.</span></span> <span data-ttu-id="ac86e-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-180">notes</span><span class="sxs-lookup"><span data-stu-id="ac86e-180">notes</span></span>|<span data-ttu-id="ac86e-181">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-181">String</span></span>|<span data-ttu-id="ac86e-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="ac86e-182">Notes for the app.</span></span> <span data-ttu-id="ac86e-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ac86e-184">uploadState</span></span>|<span data-ttu-id="ac86e-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ac86e-185">Int32</span></span>|<span data-ttu-id="ac86e-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="ac86e-186">The upload state.</span></span> <span data-ttu-id="ac86e-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ac86e-188">publishingState</span></span>|[<span data-ttu-id="ac86e-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ac86e-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ac86e-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="ac86e-190">The publishing state for the app.</span></span> <span data-ttu-id="ac86e-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="ac86e-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ac86e-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ac86e-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ac86e-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="ac86e-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ac86e-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ac86e-194">isAssigned</span></span>|<span data-ttu-id="ac86e-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ac86e-195">Boolean</span></span>|<span data-ttu-id="ac86e-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="ac86e-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ac86e-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ac86e-198">roleScopeTagIds</span></span>|<span data-ttu-id="ac86e-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ac86e-199">String collection</span></span>|<span data-ttu-id="ac86e-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="ac86e-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ac86e-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ac86e-202">appAvailability</span><span class="sxs-lookup"><span data-stu-id="ac86e-202">appAvailability</span></span>|[<span data-ttu-id="ac86e-203">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="ac86e-203">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="ac86e-204">アプリケーションの可用性。</span><span class="sxs-lookup"><span data-stu-id="ac86e-204">The Application's availability.</span></span> <span data-ttu-id="ac86e-205">[ManagedApp](../resources/intune-apps-managedapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ac86e-205">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="ac86e-206">可能な値は、`global`、`lineOfBusiness` です。</span><span class="sxs-lookup"><span data-stu-id="ac86e-206">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="ac86e-207">version</span><span class="sxs-lookup"><span data-stu-id="ac86e-207">version</span></span>|<span data-ttu-id="ac86e-208">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-208">String</span></span>|<span data-ttu-id="ac86e-209">アプリケーションのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ac86e-209">The Application's version.</span></span> <span data-ttu-id="ac86e-210">[managedApp](../resources/intune-apps-managedapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-210">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="ac86e-211">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ac86e-211">committedContentVersion</span></span>|<span data-ttu-id="ac86e-212">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-212">String</span></span>|<span data-ttu-id="ac86e-213">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ac86e-213">The internal committed content version.</span></span> <span data-ttu-id="ac86e-214">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ac86e-215">fileName</span><span class="sxs-lookup"><span data-stu-id="ac86e-215">fileName</span></span>|<span data-ttu-id="ac86e-216">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-216">String</span></span>|<span data-ttu-id="ac86e-217">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="ac86e-217">The name of the main Lob application file.</span></span> <span data-ttu-id="ac86e-218">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-218">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ac86e-219">size</span><span class="sxs-lookup"><span data-stu-id="ac86e-219">size</span></span>|<span data-ttu-id="ac86e-220">Int64</span><span class="sxs-lookup"><span data-stu-id="ac86e-220">Int64</span></span>|<span data-ttu-id="ac86e-221">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="ac86e-221">The total size, including all uploaded files.</span></span> <span data-ttu-id="ac86e-222">[managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ac86e-222">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="ac86e-223">bundleId</span><span class="sxs-lookup"><span data-stu-id="ac86e-223">bundleId</span></span>|<span data-ttu-id="ac86e-224">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-224">String</span></span>|<span data-ttu-id="ac86e-225">ID 名。</span><span class="sxs-lookup"><span data-stu-id="ac86e-225">The Identity Name.</span></span>|
|<span data-ttu-id="ac86e-226">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="ac86e-226">applicableDeviceType</span></span>|[<span data-ttu-id="ac86e-227">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="ac86e-227">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="ac86e-228">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="ac86e-228">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="ac86e-229">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ac86e-229">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ac86e-230">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ac86e-230">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="ac86e-231">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="ac86e-231">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ac86e-232">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ac86e-232">expirationDateTime</span></span>|<span data-ttu-id="ac86e-233">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac86e-233">DateTimeOffset</span></span>|<span data-ttu-id="ac86e-234">有効期限。</span><span class="sxs-lookup"><span data-stu-id="ac86e-234">The expiration time.</span></span>|
|<span data-ttu-id="ac86e-235">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="ac86e-235">versionNumber</span></span>|<span data-ttu-id="ac86e-236">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-236">String</span></span>|<span data-ttu-id="ac86e-237">管理対象 iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="ac86e-237">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ac86e-238">buildNumber</span><span class="sxs-lookup"><span data-stu-id="ac86e-238">buildNumber</span></span>|<span data-ttu-id="ac86e-239">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-239">String</span></span>|<span data-ttu-id="ac86e-240">管理対象 iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="ac86e-240">The build number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="ac86e-241">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ac86e-241">identityVersion</span></span>|<span data-ttu-id="ac86e-242">String</span><span class="sxs-lookup"><span data-stu-id="ac86e-242">String</span></span>|<span data-ttu-id="ac86e-243">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ac86e-243">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ac86e-244">応答</span><span class="sxs-lookup"><span data-stu-id="ac86e-244">Response</span></span>
<span data-ttu-id="ac86e-245">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="ac86e-245">If successful, this method returns a `200 OK` response code and an updated [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac86e-246">例</span><span class="sxs-lookup"><span data-stu-id="ac86e-246">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac86e-247">要求</span><span class="sxs-lookup"><span data-stu-id="ac86e-247">Request</span></span>
<span data-ttu-id="ac86e-248">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ac86e-248">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1442

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ac86e-249">応答</span><span class="sxs-lookup"><span data-stu-id="ac86e-249">Response</span></span>
<span data-ttu-id="ac86e-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ac86e-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1614

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value",
  "identityVersion": "Identity Version value"
}
```




