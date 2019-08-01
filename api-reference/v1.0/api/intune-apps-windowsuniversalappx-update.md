---
title: windowsUniversalAppX の更新
description: windowsUniversalAppX オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 21df53aa0f7cdcb9c239193851f7ea12d293c2b1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015907"
---
# <a name="update-windowsuniversalappx"></a><span data-ttu-id="2d138-103">windowsUniversalAppX の更新</span><span class="sxs-lookup"><span data-stu-id="2d138-103">Update windowsUniversalAppX</span></span>

> <span data-ttu-id="2d138-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d138-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d138-105">[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2d138-105">Update the properties of a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d138-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d138-106">Prerequisites</span></span>
<span data-ttu-id="2d138-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d138-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d138-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d138-109">Permission type</span></span>|<span data-ttu-id="2d138-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d138-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d138-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d138-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2d138-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d138-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2d138-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d138-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d138-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d138-114">Not supported.</span></span>|
|<span data-ttu-id="2d138-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d138-115">Application</span></span>|<span data-ttu-id="2d138-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d138-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d138-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d138-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="2d138-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d138-118">Request headers</span></span>
|<span data-ttu-id="2d138-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d138-119">Header</span></span>|<span data-ttu-id="2d138-120">値</span><span class="sxs-lookup"><span data-stu-id="2d138-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d138-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d138-121">Authorization</span></span>|<span data-ttu-id="2d138-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d138-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d138-123">承諾</span><span class="sxs-lookup"><span data-stu-id="2d138-123">Accept</span></span>|<span data-ttu-id="2d138-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2d138-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d138-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d138-125">Request body</span></span>
<span data-ttu-id="2d138-126">要求本文で、[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d138-126">In the request body, supply a JSON representation for the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

<span data-ttu-id="2d138-127">次の表に、[windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2d138-127">The following table shows the properties that are required when you create the [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md).</span></span>

|<span data-ttu-id="2d138-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d138-128">Property</span></span>|<span data-ttu-id="2d138-129">型</span><span class="sxs-lookup"><span data-stu-id="2d138-129">Type</span></span>|<span data-ttu-id="2d138-130">説明</span><span class="sxs-lookup"><span data-stu-id="2d138-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d138-131">id</span><span class="sxs-lookup"><span data-stu-id="2d138-131">id</span></span>|<span data-ttu-id="2d138-132">文字列</span><span class="sxs-lookup"><span data-stu-id="2d138-132">String</span></span>|<span data-ttu-id="2d138-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2d138-133">Key of the entity.</span></span> <span data-ttu-id="2d138-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2d138-135">displayName</span></span>|<span data-ttu-id="2d138-136">文字列</span><span class="sxs-lookup"><span data-stu-id="2d138-136">String</span></span>|<span data-ttu-id="2d138-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="2d138-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="2d138-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-139">description</span><span class="sxs-lookup"><span data-stu-id="2d138-139">description</span></span>|<span data-ttu-id="2d138-140">String</span><span class="sxs-lookup"><span data-stu-id="2d138-140">String</span></span>|<span data-ttu-id="2d138-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="2d138-141">The description of the app.</span></span> <span data-ttu-id="2d138-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-143">publisher</span><span class="sxs-lookup"><span data-stu-id="2d138-143">publisher</span></span>|<span data-ttu-id="2d138-144">String</span><span class="sxs-lookup"><span data-stu-id="2d138-144">String</span></span>|<span data-ttu-id="2d138-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="2d138-145">The publisher of the app.</span></span> <span data-ttu-id="2d138-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="2d138-147">largeIcon</span></span>|[<span data-ttu-id="2d138-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="2d138-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="2d138-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="2d138-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="2d138-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d138-151">createdDateTime</span></span>|<span data-ttu-id="2d138-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d138-152">DateTimeOffset</span></span>|<span data-ttu-id="2d138-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="2d138-153">The date and time the app was created.</span></span> <span data-ttu-id="2d138-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d138-155">lastModifiedDateTime</span></span>|<span data-ttu-id="2d138-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d138-156">DateTimeOffset</span></span>|<span data-ttu-id="2d138-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="2d138-157">The date and time the app was last modified.</span></span> <span data-ttu-id="2d138-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="2d138-159">isFeatured</span></span>|<span data-ttu-id="2d138-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d138-160">Boolean</span></span>|<span data-ttu-id="2d138-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="2d138-162">privacyInformationUrl</span></span>|<span data-ttu-id="2d138-163">String</span><span class="sxs-lookup"><span data-stu-id="2d138-163">String</span></span>|<span data-ttu-id="2d138-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="2d138-164">The privacy statement Url.</span></span> <span data-ttu-id="2d138-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="2d138-166">informationUrl</span></span>|<span data-ttu-id="2d138-167">String</span><span class="sxs-lookup"><span data-stu-id="2d138-167">String</span></span>|<span data-ttu-id="2d138-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="2d138-168">The more information Url.</span></span> <span data-ttu-id="2d138-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-170">owner</span><span class="sxs-lookup"><span data-stu-id="2d138-170">owner</span></span>|<span data-ttu-id="2d138-171">String</span><span class="sxs-lookup"><span data-stu-id="2d138-171">String</span></span>|<span data-ttu-id="2d138-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="2d138-172">The owner of the app.</span></span> <span data-ttu-id="2d138-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-174">developer</span><span class="sxs-lookup"><span data-stu-id="2d138-174">developer</span></span>|<span data-ttu-id="2d138-175">String</span><span class="sxs-lookup"><span data-stu-id="2d138-175">String</span></span>|<span data-ttu-id="2d138-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="2d138-176">The developer of the app.</span></span> <span data-ttu-id="2d138-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-178">notes</span><span class="sxs-lookup"><span data-stu-id="2d138-178">notes</span></span>|<span data-ttu-id="2d138-179">String</span><span class="sxs-lookup"><span data-stu-id="2d138-179">String</span></span>|<span data-ttu-id="2d138-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="2d138-180">Notes for the app.</span></span> <span data-ttu-id="2d138-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="2d138-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="2d138-182">publishingState</span></span>|[<span data-ttu-id="2d138-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="2d138-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="2d138-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="2d138-184">The publishing state for the app.</span></span> <span data-ttu-id="2d138-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="2d138-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="2d138-186">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="2d138-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="2d138-187">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="2d138-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="2d138-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="2d138-188">committedContentVersion</span></span>|<span data-ttu-id="2d138-189">String</span><span class="sxs-lookup"><span data-stu-id="2d138-189">String</span></span>|<span data-ttu-id="2d138-190">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2d138-190">The internal committed content version.</span></span> <span data-ttu-id="2d138-191">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2d138-192">fileName</span><span class="sxs-lookup"><span data-stu-id="2d138-192">fileName</span></span>|<span data-ttu-id="2d138-193">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2d138-193">String</span></span>|<span data-ttu-id="2d138-194">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="2d138-194">The name of the main Lob application file.</span></span> <span data-ttu-id="2d138-195">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2d138-196">size</span><span class="sxs-lookup"><span data-stu-id="2d138-196">size</span></span>|<span data-ttu-id="2d138-197">Int64</span><span class="sxs-lookup"><span data-stu-id="2d138-197">Int64</span></span>|<span data-ttu-id="2d138-198">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="2d138-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="2d138-199">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2d138-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="2d138-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="2d138-200">applicableArchitectures</span></span>|[<span data-ttu-id="2d138-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="2d138-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="2d138-202">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="2d138-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="2d138-203">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="2d138-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="2d138-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="2d138-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="2d138-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="2d138-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="2d138-206">このアプリを実行できる Windows デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="2d138-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="2d138-207">可能な値は、`none`、`desktop`、`mobile`、`holographic`、`team` です。</span><span class="sxs-lookup"><span data-stu-id="2d138-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="2d138-208">identityName</span><span class="sxs-lookup"><span data-stu-id="2d138-208">identityName</span></span>|<span data-ttu-id="2d138-209">String</span><span class="sxs-lookup"><span data-stu-id="2d138-209">String</span></span>|<span data-ttu-id="2d138-210">ID 名。</span><span class="sxs-lookup"><span data-stu-id="2d138-210">The Identity Name.</span></span>|
|<span data-ttu-id="2d138-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="2d138-211">identityPublisherHash</span></span>|<span data-ttu-id="2d138-212">String</span><span class="sxs-lookup"><span data-stu-id="2d138-212">String</span></span>|<span data-ttu-id="2d138-213">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="2d138-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="2d138-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="2d138-214">identityResourceIdentifier</span></span>|<span data-ttu-id="2d138-215">String</span><span class="sxs-lookup"><span data-stu-id="2d138-215">String</span></span>|<span data-ttu-id="2d138-216">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="2d138-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="2d138-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="2d138-217">isBundle</span></span>|<span data-ttu-id="2d138-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d138-218">Boolean</span></span>|<span data-ttu-id="2d138-219">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2d138-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="2d138-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2d138-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="2d138-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="2d138-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="2d138-222">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="2d138-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="2d138-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="2d138-223">identityVersion</span></span>|<span data-ttu-id="2d138-224">String</span><span class="sxs-lookup"><span data-stu-id="2d138-224">String</span></span>|<span data-ttu-id="2d138-225">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="2d138-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="2d138-226">応答</span><span class="sxs-lookup"><span data-stu-id="2d138-226">Response</span></span>
<span data-ttu-id="2d138-227">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="2d138-227">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d138-228">例</span><span class="sxs-lookup"><span data-stu-id="2d138-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d138-229">要求</span><span class="sxs-lookup"><span data-stu-id="2d138-229">Request</span></span>
<span data-ttu-id="2d138-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d138-230">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1189

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="2d138-231">応答</span><span class="sxs-lookup"><span data-stu-id="2d138-231">Response</span></span>
<span data-ttu-id="2d138-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d138-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1361

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppX",
  "id": "4bc47eba-7eba-4bc4-ba7e-c44bba7ec44b",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "applicableDeviceTypes": "desktop",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true
  },
  "identityVersion": "Identity Version value"
}
```



