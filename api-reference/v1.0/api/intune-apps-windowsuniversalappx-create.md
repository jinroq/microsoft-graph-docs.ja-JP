---
title: Create windowsUniversalAppX
description: 新しい windowsUniversalAppX オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c415d02f0c83a4ccf6d64400581c137e3b56af5f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454217"
---
# <a name="create-windowsuniversalappx"></a><span data-ttu-id="82b8c-103">Create windowsUniversalAppX</span><span class="sxs-lookup"><span data-stu-id="82b8c-103">Create windowsUniversalAppX</span></span>

> <span data-ttu-id="82b8c-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="82b8c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82b8c-105">新しい [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="82b8c-105">Create a new [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82b8c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="82b8c-106">Prerequisites</span></span>
<span data-ttu-id="82b8c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="82b8c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82b8c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="82b8c-109">Permission type</span></span>|<span data-ttu-id="82b8c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="82b8c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82b8c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="82b8c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82b8c-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82b8c-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="82b8c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="82b8c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82b8c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82b8c-114">Not supported.</span></span>|
|<span data-ttu-id="82b8c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="82b8c-115">Application</span></span>|<span data-ttu-id="82b8c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="82b8c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82b8c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="82b8c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="82b8c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82b8c-118">Request headers</span></span>
|<span data-ttu-id="82b8c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="82b8c-119">Header</span></span>|<span data-ttu-id="82b8c-120">値</span><span class="sxs-lookup"><span data-stu-id="82b8c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82b8c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82b8c-121">Authorization</span></span>|<span data-ttu-id="82b8c-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="82b8c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82b8c-123">承諾</span><span class="sxs-lookup"><span data-stu-id="82b8c-123">Accept</span></span>|<span data-ttu-id="82b8c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="82b8c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82b8c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="82b8c-125">Request body</span></span>
<span data-ttu-id="82b8c-126">要求本文で、windowsUniversalAppX オブジェクトの JSON 表現を指定します。</span><span class="sxs-lookup"><span data-stu-id="82b8c-126">In the request body, supply a JSON representation for the windowsUniversalAppX object.</span></span>

<span data-ttu-id="82b8c-127">次の表に、windowsUniversalAppX の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="82b8c-127">The following table shows the properties that are required when you create the windowsUniversalAppX.</span></span>

|<span data-ttu-id="82b8c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82b8c-128">Property</span></span>|<span data-ttu-id="82b8c-129">型</span><span class="sxs-lookup"><span data-stu-id="82b8c-129">Type</span></span>|<span data-ttu-id="82b8c-130">説明</span><span class="sxs-lookup"><span data-stu-id="82b8c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82b8c-131">id</span><span class="sxs-lookup"><span data-stu-id="82b8c-131">id</span></span>|<span data-ttu-id="82b8c-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="82b8c-132">String</span></span>|<span data-ttu-id="82b8c-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="82b8c-133">Key of the entity.</span></span> <span data-ttu-id="82b8c-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="82b8c-135">displayName</span></span>|<span data-ttu-id="82b8c-136">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-136">String</span></span>|<span data-ttu-id="82b8c-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="82b8c-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="82b8c-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-139">説明</span><span class="sxs-lookup"><span data-stu-id="82b8c-139">description</span></span>|<span data-ttu-id="82b8c-140">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-140">String</span></span>|<span data-ttu-id="82b8c-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="82b8c-141">The description of the app.</span></span> <span data-ttu-id="82b8c-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-143">publisher</span><span class="sxs-lookup"><span data-stu-id="82b8c-143">publisher</span></span>|<span data-ttu-id="82b8c-144">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-144">String</span></span>|<span data-ttu-id="82b8c-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="82b8c-145">The publisher of the app.</span></span> <span data-ttu-id="82b8c-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="82b8c-147">largeIcon</span></span>|[<span data-ttu-id="82b8c-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="82b8c-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="82b8c-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="82b8c-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="82b8c-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82b8c-151">createdDateTime</span></span>|<span data-ttu-id="82b8c-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82b8c-152">DateTimeOffset</span></span>|<span data-ttu-id="82b8c-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="82b8c-153">The date and time the app was created.</span></span> <span data-ttu-id="82b8c-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82b8c-155">lastModifiedDateTime</span></span>|<span data-ttu-id="82b8c-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82b8c-156">DateTimeOffset</span></span>|<span data-ttu-id="82b8c-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="82b8c-157">The date and time the app was last modified.</span></span> <span data-ttu-id="82b8c-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="82b8c-159">isFeatured</span></span>|<span data-ttu-id="82b8c-160">ブール型</span><span class="sxs-lookup"><span data-stu-id="82b8c-160">Boolean</span></span>|<span data-ttu-id="82b8c-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="82b8c-162">privacyInformationUrl</span></span>|<span data-ttu-id="82b8c-163">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-163">String</span></span>|<span data-ttu-id="82b8c-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="82b8c-164">The privacy statement Url.</span></span> <span data-ttu-id="82b8c-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="82b8c-166">informationUrl</span></span>|<span data-ttu-id="82b8c-167">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-167">String</span></span>|<span data-ttu-id="82b8c-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="82b8c-168">The more information Url.</span></span> <span data-ttu-id="82b8c-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-170">owner</span><span class="sxs-lookup"><span data-stu-id="82b8c-170">owner</span></span>|<span data-ttu-id="82b8c-171">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-171">String</span></span>|<span data-ttu-id="82b8c-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="82b8c-172">The owner of the app.</span></span> <span data-ttu-id="82b8c-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-174">developer</span><span class="sxs-lookup"><span data-stu-id="82b8c-174">developer</span></span>|<span data-ttu-id="82b8c-175">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-175">String</span></span>|<span data-ttu-id="82b8c-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="82b8c-176">The developer of the app.</span></span> <span data-ttu-id="82b8c-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-178">notes</span><span class="sxs-lookup"><span data-stu-id="82b8c-178">notes</span></span>|<span data-ttu-id="82b8c-179">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-179">String</span></span>|<span data-ttu-id="82b8c-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="82b8c-180">Notes for the app.</span></span> <span data-ttu-id="82b8c-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="82b8c-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="82b8c-182">publishingState</span></span>|[<span data-ttu-id="82b8c-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="82b8c-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="82b8c-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="82b8c-184">The publishing state for the app.</span></span> <span data-ttu-id="82b8c-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="82b8c-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="82b8c-186">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="82b8c-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="82b8c-187">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="82b8c-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="82b8c-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="82b8c-188">committedContentVersion</span></span>|<span data-ttu-id="82b8c-189">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-189">String</span></span>|<span data-ttu-id="82b8c-190">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="82b8c-190">The internal committed content version.</span></span> <span data-ttu-id="82b8c-191">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="82b8c-192">fileName</span><span class="sxs-lookup"><span data-stu-id="82b8c-192">fileName</span></span>|<span data-ttu-id="82b8c-193">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="82b8c-193">String</span></span>|<span data-ttu-id="82b8c-194">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="82b8c-194">The name of the main Lob application file.</span></span> <span data-ttu-id="82b8c-195">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="82b8c-196">size</span><span class="sxs-lookup"><span data-stu-id="82b8c-196">size</span></span>|<span data-ttu-id="82b8c-197">Int64</span><span class="sxs-lookup"><span data-stu-id="82b8c-197">Int64</span></span>|<span data-ttu-id="82b8c-198">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="82b8c-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="82b8c-199">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="82b8c-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="82b8c-200">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="82b8c-200">applicableArchitectures</span></span>|[<span data-ttu-id="82b8c-201">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="82b8c-201">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="82b8c-202">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="82b8c-202">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="82b8c-203">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="82b8c-203">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="82b8c-204">applicableDeviceTypes</span><span class="sxs-lookup"><span data-stu-id="82b8c-204">applicableDeviceTypes</span></span>|[<span data-ttu-id="82b8c-205">windowsDeviceType</span><span class="sxs-lookup"><span data-stu-id="82b8c-205">windowsDeviceType</span></span>](../resources/intune-apps-windowsdevicetype.md)|<span data-ttu-id="82b8c-206">このアプリを実行できる Windows デバイスの種類。</span><span class="sxs-lookup"><span data-stu-id="82b8c-206">The Windows device type(s) for which this app can run on.</span></span> <span data-ttu-id="82b8c-207">可能な値は、`none`、`desktop`、`mobile`、`holographic`、`team` です。</span><span class="sxs-lookup"><span data-stu-id="82b8c-207">Possible values are: `none`, `desktop`, `mobile`, `holographic`, `team`.</span></span>|
|<span data-ttu-id="82b8c-208">identityName</span><span class="sxs-lookup"><span data-stu-id="82b8c-208">identityName</span></span>|<span data-ttu-id="82b8c-209">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-209">String</span></span>|<span data-ttu-id="82b8c-210">ID 名。</span><span class="sxs-lookup"><span data-stu-id="82b8c-210">The Identity Name.</span></span>|
|<span data-ttu-id="82b8c-211">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="82b8c-211">identityPublisherHash</span></span>|<span data-ttu-id="82b8c-212">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-212">String</span></span>|<span data-ttu-id="82b8c-213">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="82b8c-213">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="82b8c-214">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="82b8c-214">identityResourceIdentifier</span></span>|<span data-ttu-id="82b8c-215">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-215">String</span></span>|<span data-ttu-id="82b8c-216">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="82b8c-216">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="82b8c-217">isBundle</span><span class="sxs-lookup"><span data-stu-id="82b8c-217">isBundle</span></span>|<span data-ttu-id="82b8c-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="82b8c-218">Boolean</span></span>|<span data-ttu-id="82b8c-219">アプリがバンドルかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="82b8c-219">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="82b8c-220">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="82b8c-220">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="82b8c-221">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="82b8c-221">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="82b8c-222">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="82b8c-222">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="82b8c-223">identityVersion</span><span class="sxs-lookup"><span data-stu-id="82b8c-223">identityVersion</span></span>|<span data-ttu-id="82b8c-224">String</span><span class="sxs-lookup"><span data-stu-id="82b8c-224">String</span></span>|<span data-ttu-id="82b8c-225">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="82b8c-225">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="82b8c-226">応答</span><span class="sxs-lookup"><span data-stu-id="82b8c-226">Response</span></span>
<span data-ttu-id="82b8c-227">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="82b8c-227">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppX](../resources/intune-apps-windowsuniversalappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82b8c-228">例</span><span class="sxs-lookup"><span data-stu-id="82b8c-228">Example</span></span>

### <a name="request"></a><span data-ttu-id="82b8c-229">要求</span><span class="sxs-lookup"><span data-stu-id="82b8c-229">Request</span></span>
<span data-ttu-id="82b8c-230">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="82b8c-230">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
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

### <a name="response"></a><span data-ttu-id="82b8c-231">応答</span><span class="sxs-lookup"><span data-stu-id="82b8c-231">Response</span></span>
<span data-ttu-id="82b8c-p120">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="82b8c-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



