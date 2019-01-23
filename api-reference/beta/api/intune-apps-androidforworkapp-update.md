---
title: AndroidForWorkApp を更新します。
description: AndroidForWorkApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 09b5f502ca8b666a687e2b0df99fed52b1c4ff12
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398346"
---
# <a name="update-androidforworkapp"></a><span data-ttu-id="a5fe2-103">AndroidForWorkApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-103">Update androidForWorkApp</span></span>

> <span data-ttu-id="a5fe2-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a5fe2-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5fe2-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5fe2-107">[AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-107">Update the properties of a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5fe2-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a5fe2-108">Prerequisites</span></span>
<span data-ttu-id="a5fe2-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a5fe2-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5fe2-111">Permission type</span></span>|<span data-ttu-id="a5fe2-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5fe2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5fe2-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5fe2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5fe2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5fe2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5fe2-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5fe2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5fe2-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-116">Not supported.</span></span>|
|<span data-ttu-id="a5fe2-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5fe2-117">Application</span></span>|<span data-ttu-id="a5fe2-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5fe2-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5fe2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="a5fe2-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5fe2-120">Request headers</span></span>
|<span data-ttu-id="a5fe2-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5fe2-121">Header</span></span>|<span data-ttu-id="a5fe2-122">値</span><span class="sxs-lookup"><span data-stu-id="a5fe2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5fe2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5fe2-123">Authorization</span></span>|<span data-ttu-id="a5fe2-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5fe2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5fe2-125">Accept</span></span>|<span data-ttu-id="a5fe2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5fe2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5fe2-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5fe2-127">Request body</span></span>
<span data-ttu-id="a5fe2-128">要求の本文に[androidForWorkApp](../resources/intune-apps-androidforworkapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-128">In the request body, supply a JSON representation for the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

<span data-ttu-id="a5fe2-129">[AndroidForWorkApp](../resources/intune-apps-androidforworkapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-129">The following table shows the properties that are required when you create the [androidForWorkApp](../resources/intune-apps-androidforworkapp.md).</span></span>

|<span data-ttu-id="a5fe2-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5fe2-130">Property</span></span>|<span data-ttu-id="a5fe2-131">型</span><span class="sxs-lookup"><span data-stu-id="a5fe2-131">Type</span></span>|<span data-ttu-id="a5fe2-132">説明</span><span class="sxs-lookup"><span data-stu-id="a5fe2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5fe2-133">id</span><span class="sxs-lookup"><span data-stu-id="a5fe2-133">id</span></span>|<span data-ttu-id="a5fe2-134">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-134">String</span></span>|<span data-ttu-id="a5fe2-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-135">Key of the entity.</span></span> <span data-ttu-id="a5fe2-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a5fe2-137">displayName</span></span>|<span data-ttu-id="a5fe2-138">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-138">String</span></span>|<span data-ttu-id="a5fe2-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a5fe2-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-141">説明</span><span class="sxs-lookup"><span data-stu-id="a5fe2-141">description</span></span>|<span data-ttu-id="a5fe2-142">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-142">String</span></span>|<span data-ttu-id="a5fe2-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-143">The description of the app.</span></span> <span data-ttu-id="a5fe2-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="a5fe2-145">publisher</span></span>|<span data-ttu-id="a5fe2-146">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-146">String</span></span>|<span data-ttu-id="a5fe2-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-147">The publisher of the app.</span></span> <span data-ttu-id="a5fe2-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a5fe2-149">largeIcon</span></span>|[<span data-ttu-id="a5fe2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a5fe2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a5fe2-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a5fe2-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a5fe2-153">createdDateTime</span></span>|<span data-ttu-id="a5fe2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5fe2-154">DateTimeOffset</span></span>|<span data-ttu-id="a5fe2-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-155">The date and time the app was created.</span></span> <span data-ttu-id="a5fe2-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a5fe2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="a5fe2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a5fe2-158">DateTimeOffset</span></span>|<span data-ttu-id="a5fe2-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="a5fe2-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a5fe2-161">isFeatured</span></span>|<span data-ttu-id="a5fe2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5fe2-162">Boolean</span></span>|<span data-ttu-id="a5fe2-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a5fe2-164">privacyInformationUrl</span></span>|<span data-ttu-id="a5fe2-165">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-165">String</span></span>|<span data-ttu-id="a5fe2-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-166">The privacy statement Url.</span></span> <span data-ttu-id="a5fe2-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a5fe2-168">informationUrl</span></span>|<span data-ttu-id="a5fe2-169">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-169">String</span></span>|<span data-ttu-id="a5fe2-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-170">The more information Url.</span></span> <span data-ttu-id="a5fe2-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-172">owner</span><span class="sxs-lookup"><span data-stu-id="a5fe2-172">owner</span></span>|<span data-ttu-id="a5fe2-173">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-173">String</span></span>|<span data-ttu-id="a5fe2-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-174">The owner of the app.</span></span> <span data-ttu-id="a5fe2-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-176">developer</span><span class="sxs-lookup"><span data-stu-id="a5fe2-176">developer</span></span>|<span data-ttu-id="a5fe2-177">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-177">String</span></span>|<span data-ttu-id="a5fe2-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-178">The developer of the app.</span></span> <span data-ttu-id="a5fe2-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-180">notes</span><span class="sxs-lookup"><span data-stu-id="a5fe2-180">notes</span></span>|<span data-ttu-id="a5fe2-181">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-181">String</span></span>|<span data-ttu-id="a5fe2-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-182">Notes for the app.</span></span> <span data-ttu-id="a5fe2-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="a5fe2-184">uploadState</span></span>|<span data-ttu-id="a5fe2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a5fe2-185">Int32</span></span>|<span data-ttu-id="a5fe2-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-186">The upload state.</span></span> <span data-ttu-id="a5fe2-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="a5fe2-188">publishingState</span></span>|[<span data-ttu-id="a5fe2-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a5fe2-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a5fe2-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-190">The publishing state for the app.</span></span> <span data-ttu-id="a5fe2-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a5fe2-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a5fe2-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a5fe2-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="a5fe2-194">isAssigned</span></span>|<span data-ttu-id="a5fe2-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="a5fe2-195">Boolean</span></span>|<span data-ttu-id="a5fe2-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="a5fe2-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a5fe2-198">roleScopeTagIds</span></span>|<span data-ttu-id="a5fe2-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a5fe2-199">String collection</span></span>|<span data-ttu-id="a5fe2-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="a5fe2-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a5fe2-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a5fe2-202">packageId</span><span class="sxs-lookup"><span data-stu-id="a5fe2-202">packageId</span></span>|<span data-ttu-id="a5fe2-203">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-203">String</span></span>|<span data-ttu-id="a5fe2-204">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-204">The package identifier.</span></span>|
|<span data-ttu-id="a5fe2-205">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="a5fe2-205">appIdentifier</span></span>|<span data-ttu-id="a5fe2-206">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-206">String</span></span>|<span data-ttu-id="a5fe2-207">ID 名。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-207">The Identity Name.</span></span>|
|<span data-ttu-id="a5fe2-208">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a5fe2-208">usedLicenseCount</span></span>|<span data-ttu-id="a5fe2-209">Int32</span><span class="sxs-lookup"><span data-stu-id="a5fe2-209">Int32</span></span>|<span data-ttu-id="a5fe2-210">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-210">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="a5fe2-211">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="a5fe2-211">totalLicenseCount</span></span>|<span data-ttu-id="a5fe2-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a5fe2-212">Int32</span></span>|<span data-ttu-id="a5fe2-213">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-213">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="a5fe2-214">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="a5fe2-214">appStoreUrl</span></span>|<span data-ttu-id="a5fe2-215">String</span><span class="sxs-lookup"><span data-stu-id="a5fe2-215">String</span></span>|<span data-ttu-id="a5fe2-216">作業ストア アプリケーションの URL を再生します。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-216">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="a5fe2-217">応答</span><span class="sxs-lookup"><span data-stu-id="a5fe2-217">Response</span></span>
<span data-ttu-id="a5fe2-218">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[androidForWorkApp](../resources/intune-apps-androidforworkapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-218">If successful, this method returns a `200 OK` response code and an updated [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5fe2-219">例</span><span class="sxs-lookup"><span data-stu-id="a5fe2-219">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5fe2-220">要求</span><span class="sxs-lookup"><span data-stu-id="a5fe2-220">Request</span></span>
<span data-ttu-id="a5fe2-221">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-221">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 876

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```

### <a name="response"></a><span data-ttu-id="a5fe2-222">応答</span><span class="sxs-lookup"><span data-stu-id="a5fe2-222">Response</span></span>
<span data-ttu-id="a5fe2-p119">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5fe2-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1048

{
  "@odata.type": "#microsoft.graph.androidForWorkApp",
  "id": "c5010785-0785-c501-8507-01c5850701c5",
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
  "packageId": "Package Id value",
  "appIdentifier": "App Identifier value",
  "usedLicenseCount": 0,
  "totalLicenseCount": 1,
  "appStoreUrl": "https://example.com/appStoreUrl/"
}
```




