---
title: androidforwork アプリの作成
description: 新しい androidforwork app オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1b96fbe67fac0a6c5c3bca7becb84f84538a056f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142085"
---
# <a name="create-androidforworkapp"></a><span data-ttu-id="67a67-103">androidforwork アプリの作成</span><span class="sxs-lookup"><span data-stu-id="67a67-103">Create androidForWorkApp</span></span>

> <span data-ttu-id="67a67-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67a67-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67a67-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67a67-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67a67-106">新しい[androidforwork app](../resources/intune-apps-androidforworkapp.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="67a67-106">Create a new [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67a67-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="67a67-107">Prerequisites</span></span>
<span data-ttu-id="67a67-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67a67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67a67-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67a67-110">Permission type</span></span>|<span data-ttu-id="67a67-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67a67-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67a67-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67a67-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67a67-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67a67-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67a67-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67a67-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67a67-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67a67-115">Not supported.</span></span>|
|<span data-ttu-id="67a67-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67a67-116">Application</span></span>|<span data-ttu-id="67a67-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67a67-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67a67-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67a67-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="67a67-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67a67-119">Request headers</span></span>
|<span data-ttu-id="67a67-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67a67-120">Header</span></span>|<span data-ttu-id="67a67-121">値</span><span class="sxs-lookup"><span data-stu-id="67a67-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67a67-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67a67-122">Authorization</span></span>|<span data-ttu-id="67a67-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="67a67-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67a67-124">承諾</span><span class="sxs-lookup"><span data-stu-id="67a67-124">Accept</span></span>|<span data-ttu-id="67a67-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67a67-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67a67-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="67a67-126">Request body</span></span>
<span data-ttu-id="67a67-127">要求本文で、androidforwork app オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67a67-127">In the request body, supply a JSON representation for the androidForWorkApp object.</span></span>

<span data-ttu-id="67a67-128">次の表に、androidforwork アプリの作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="67a67-128">The following table shows the properties that are required when you create the androidForWorkApp.</span></span>

|<span data-ttu-id="67a67-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67a67-129">Property</span></span>|<span data-ttu-id="67a67-130">型</span><span class="sxs-lookup"><span data-stu-id="67a67-130">Type</span></span>|<span data-ttu-id="67a67-131">説明</span><span class="sxs-lookup"><span data-stu-id="67a67-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67a67-132">id</span><span class="sxs-lookup"><span data-stu-id="67a67-132">id</span></span>|<span data-ttu-id="67a67-133">文字列</span><span class="sxs-lookup"><span data-stu-id="67a67-133">String</span></span>|<span data-ttu-id="67a67-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="67a67-134">Key of the entity.</span></span> <span data-ttu-id="67a67-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-136">displayName</span><span class="sxs-lookup"><span data-stu-id="67a67-136">displayName</span></span>|<span data-ttu-id="67a67-137">String</span><span class="sxs-lookup"><span data-stu-id="67a67-137">String</span></span>|<span data-ttu-id="67a67-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="67a67-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="67a67-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-140">説明</span><span class="sxs-lookup"><span data-stu-id="67a67-140">description</span></span>|<span data-ttu-id="67a67-141">文字列</span><span class="sxs-lookup"><span data-stu-id="67a67-141">String</span></span>|<span data-ttu-id="67a67-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="67a67-142">The description of the app.</span></span> <span data-ttu-id="67a67-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-144">publisher</span><span class="sxs-lookup"><span data-stu-id="67a67-144">publisher</span></span>|<span data-ttu-id="67a67-145">String</span><span class="sxs-lookup"><span data-stu-id="67a67-145">String</span></span>|<span data-ttu-id="67a67-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="67a67-146">The publisher of the app.</span></span> <span data-ttu-id="67a67-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="67a67-148">largeIcon</span></span>|[<span data-ttu-id="67a67-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="67a67-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="67a67-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="67a67-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="67a67-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67a67-152">createdDateTime</span></span>|<span data-ttu-id="67a67-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a67-153">DateTimeOffset</span></span>|<span data-ttu-id="67a67-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="67a67-154">The date and time the app was created.</span></span> <span data-ttu-id="67a67-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67a67-156">lastModifiedDateTime</span></span>|<span data-ttu-id="67a67-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67a67-157">DateTimeOffset</span></span>|<span data-ttu-id="67a67-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="67a67-158">The date and time the app was last modified.</span></span> <span data-ttu-id="67a67-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="67a67-160">isFeatured</span></span>|<span data-ttu-id="67a67-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a67-161">Boolean</span></span>|<span data-ttu-id="67a67-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="67a67-163">privacyInformationUrl</span></span>|<span data-ttu-id="67a67-164">String</span><span class="sxs-lookup"><span data-stu-id="67a67-164">String</span></span>|<span data-ttu-id="67a67-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="67a67-165">The privacy statement Url.</span></span> <span data-ttu-id="67a67-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="67a67-167">informationUrl</span></span>|<span data-ttu-id="67a67-168">String</span><span class="sxs-lookup"><span data-stu-id="67a67-168">String</span></span>|<span data-ttu-id="67a67-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="67a67-169">The more information Url.</span></span> <span data-ttu-id="67a67-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-171">owner</span><span class="sxs-lookup"><span data-stu-id="67a67-171">owner</span></span>|<span data-ttu-id="67a67-172">String</span><span class="sxs-lookup"><span data-stu-id="67a67-172">String</span></span>|<span data-ttu-id="67a67-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="67a67-173">The owner of the app.</span></span> <span data-ttu-id="67a67-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-175">developer</span><span class="sxs-lookup"><span data-stu-id="67a67-175">developer</span></span>|<span data-ttu-id="67a67-176">String</span><span class="sxs-lookup"><span data-stu-id="67a67-176">String</span></span>|<span data-ttu-id="67a67-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="67a67-177">The developer of the app.</span></span> <span data-ttu-id="67a67-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-179">notes</span><span class="sxs-lookup"><span data-stu-id="67a67-179">notes</span></span>|<span data-ttu-id="67a67-180">String</span><span class="sxs-lookup"><span data-stu-id="67a67-180">String</span></span>|<span data-ttu-id="67a67-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="67a67-181">Notes for the app.</span></span> <span data-ttu-id="67a67-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="67a67-183">uploadState</span></span>|<span data-ttu-id="67a67-184">Int32</span><span class="sxs-lookup"><span data-stu-id="67a67-184">Int32</span></span>|<span data-ttu-id="67a67-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="67a67-185">The upload state.</span></span> <span data-ttu-id="67a67-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="67a67-187">publishingState</span></span>|[<span data-ttu-id="67a67-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="67a67-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="67a67-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="67a67-189">The publishing state for the app.</span></span> <span data-ttu-id="67a67-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="67a67-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="67a67-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="67a67-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="67a67-192">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="67a67-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="67a67-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="67a67-193">isAssigned</span></span>|<span data-ttu-id="67a67-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="67a67-194">Boolean</span></span>|<span data-ttu-id="67a67-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="67a67-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="67a67-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67a67-197">roleScopeTagIds</span></span>|<span data-ttu-id="67a67-198">String コレクション</span><span class="sxs-lookup"><span data-stu-id="67a67-198">String collection</span></span>|<span data-ttu-id="67a67-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="67a67-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="67a67-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67a67-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67a67-201">packageId</span><span class="sxs-lookup"><span data-stu-id="67a67-201">packageId</span></span>|<span data-ttu-id="67a67-202">String</span><span class="sxs-lookup"><span data-stu-id="67a67-202">String</span></span>|<span data-ttu-id="67a67-203">パッケージの識別子。</span><span class="sxs-lookup"><span data-stu-id="67a67-203">The package identifier.</span></span>|
|<span data-ttu-id="67a67-204">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="67a67-204">appIdentifier</span></span>|<span data-ttu-id="67a67-205">String</span><span class="sxs-lookup"><span data-stu-id="67a67-205">String</span></span>|<span data-ttu-id="67a67-206">ID 名。</span><span class="sxs-lookup"><span data-stu-id="67a67-206">The Identity Name.</span></span>|
|<span data-ttu-id="67a67-207">usedLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67a67-207">usedLicenseCount</span></span>|<span data-ttu-id="67a67-208">Int32</span><span class="sxs-lookup"><span data-stu-id="67a67-208">Int32</span></span>|<span data-ttu-id="67a67-209">使用中の VPP ライセンスの数。</span><span class="sxs-lookup"><span data-stu-id="67a67-209">The number of VPP licenses in use.</span></span>|
|<span data-ttu-id="67a67-210">totalLicenseCount</span><span class="sxs-lookup"><span data-stu-id="67a67-210">totalLicenseCount</span></span>|<span data-ttu-id="67a67-211">Int32</span><span class="sxs-lookup"><span data-stu-id="67a67-211">Int32</span></span>|<span data-ttu-id="67a67-212">VPP ライセンスの総数。</span><span class="sxs-lookup"><span data-stu-id="67a67-212">The total number of VPP licenses.</span></span>|
|<span data-ttu-id="67a67-213">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="67a67-213">appStoreUrl</span></span>|<span data-ttu-id="67a67-214">String</span><span class="sxs-lookup"><span data-stu-id="67a67-214">String</span></span>|<span data-ttu-id="67a67-215">ワークストアアプリの URL を再生します。</span><span class="sxs-lookup"><span data-stu-id="67a67-215">The Play for Work Store app URL.</span></span>|



## <a name="response"></a><span data-ttu-id="67a67-216">応答</span><span class="sxs-lookup"><span data-stu-id="67a67-216">Response</span></span>
<span data-ttu-id="67a67-217">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[androidforwork app](../resources/intune-apps-androidforworkapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="67a67-217">If successful, this method returns a `201 Created` response code and a [androidForWorkApp](../resources/intune-apps-androidforworkapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67a67-218">例</span><span class="sxs-lookup"><span data-stu-id="67a67-218">Example</span></span>

### <a name="request"></a><span data-ttu-id="67a67-219">要求</span><span class="sxs-lookup"><span data-stu-id="67a67-219">Request</span></span>
<span data-ttu-id="67a67-220">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67a67-220">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="67a67-221">応答</span><span class="sxs-lookup"><span data-stu-id="67a67-221">Response</span></span>
<span data-ttu-id="67a67-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67a67-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




