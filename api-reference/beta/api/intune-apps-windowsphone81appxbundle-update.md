---
title: WindowsPhone81AppXBundle を更新します。
description: WindowsPhone81AppXBundle オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 7e377b7ec81d16df768c42555cbdd17b9f2fdd64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336674"
---
# <a name="update-windowsphone81appxbundle"></a><span data-ttu-id="1b0bf-103">WindowsPhone81AppXBundle を更新します。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-103">Update windowsPhone81AppXBundle</span></span>

> <span data-ttu-id="1b0bf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1b0bf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1b0bf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1b0bf-107">[WindowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-107">Update the properties of a [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1b0bf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1b0bf-108">Prerequisites</span></span>
<span data-ttu-id="1b0bf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1b0bf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1b0bf-111">Permission type</span></span>|<span data-ttu-id="1b0bf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1b0bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1b0bf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1b0bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1b0bf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1b0bf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1b0bf-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1b0bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1b0bf-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-116">Not supported.</span></span>|
|<span data-ttu-id="1b0bf-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1b0bf-117">Application</span></span>|<span data-ttu-id="1b0bf-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1b0bf-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1b0bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1b0bf-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b0bf-120">Request headers</span></span>
|<span data-ttu-id="1b0bf-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1b0bf-121">Header</span></span>|<span data-ttu-id="1b0bf-122">値</span><span class="sxs-lookup"><span data-stu-id="1b0bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1b0bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1b0bf-123">Authorization</span></span>|<span data-ttu-id="1b0bf-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1b0bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1b0bf-125">Accept</span></span>|<span data-ttu-id="1b0bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1b0bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1b0bf-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1b0bf-127">Request body</span></span>
<span data-ttu-id="1b0bf-128">要求の本文に[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-128">In the request body, supply a JSON representation for the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object.</span></span>

<span data-ttu-id="1b0bf-129">[WindowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-129">The following table shows the properties that are required when you create the [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md).</span></span>

|<span data-ttu-id="1b0bf-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1b0bf-130">Property</span></span>|<span data-ttu-id="1b0bf-131">種類</span><span class="sxs-lookup"><span data-stu-id="1b0bf-131">Type</span></span>|<span data-ttu-id="1b0bf-132">説明</span><span class="sxs-lookup"><span data-stu-id="1b0bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b0bf-133">ID</span><span class="sxs-lookup"><span data-stu-id="1b0bf-133">id</span></span>|<span data-ttu-id="1b0bf-134">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-134">String</span></span>|<span data-ttu-id="1b0bf-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-135">Key of the entity.</span></span> <span data-ttu-id="1b0bf-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1b0bf-137">displayName</span></span>|<span data-ttu-id="1b0bf-138">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-138">String</span></span>|<span data-ttu-id="1b0bf-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1b0bf-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-141">説明</span><span class="sxs-lookup"><span data-stu-id="1b0bf-141">description</span></span>|<span data-ttu-id="1b0bf-142">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-142">String</span></span>|<span data-ttu-id="1b0bf-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-143">The description of the app.</span></span> <span data-ttu-id="1b0bf-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1b0bf-145">publisher</span></span>|<span data-ttu-id="1b0bf-146">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-146">String</span></span>|<span data-ttu-id="1b0bf-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-147">The publisher of the app.</span></span> <span data-ttu-id="1b0bf-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1b0bf-149">largeIcon</span></span>|[<span data-ttu-id="1b0bf-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1b0bf-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1b0bf-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1b0bf-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0bf-153">createdDateTime</span></span>|<span data-ttu-id="1b0bf-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0bf-154">DateTimeOffset</span></span>|<span data-ttu-id="1b0bf-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-155">The date and time the app was created.</span></span> <span data-ttu-id="1b0bf-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1b0bf-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1b0bf-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b0bf-158">DateTimeOffset</span></span>|<span data-ttu-id="1b0bf-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1b0bf-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1b0bf-161">isFeatured</span></span>|<span data-ttu-id="1b0bf-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1b0bf-162">Boolean</span></span>|<span data-ttu-id="1b0bf-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1b0bf-164">privacyInformationUrl</span></span>|<span data-ttu-id="1b0bf-165">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-165">String</span></span>|<span data-ttu-id="1b0bf-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-166">The privacy statement Url.</span></span> <span data-ttu-id="1b0bf-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1b0bf-168">informationUrl</span></span>|<span data-ttu-id="1b0bf-169">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-169">String</span></span>|<span data-ttu-id="1b0bf-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-170">The more information Url.</span></span> <span data-ttu-id="1b0bf-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-172">owner</span><span class="sxs-lookup"><span data-stu-id="1b0bf-172">owner</span></span>|<span data-ttu-id="1b0bf-173">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-173">String</span></span>|<span data-ttu-id="1b0bf-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-174">The owner of the app.</span></span> <span data-ttu-id="1b0bf-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-176">developer</span><span class="sxs-lookup"><span data-stu-id="1b0bf-176">developer</span></span>|<span data-ttu-id="1b0bf-177">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-177">String</span></span>|<span data-ttu-id="1b0bf-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-178">The developer of the app.</span></span> <span data-ttu-id="1b0bf-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-180">notes</span><span class="sxs-lookup"><span data-stu-id="1b0bf-180">notes</span></span>|<span data-ttu-id="1b0bf-181">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-181">String</span></span>|<span data-ttu-id="1b0bf-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-182">Notes for the app.</span></span> <span data-ttu-id="1b0bf-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1b0bf-184">uploadState</span></span>|<span data-ttu-id="1b0bf-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1b0bf-185">Int32</span></span>|<span data-ttu-id="1b0bf-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-186">The upload state.</span></span> <span data-ttu-id="1b0bf-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1b0bf-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1b0bf-188">publishingState</span></span>|[<span data-ttu-id="1b0bf-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1b0bf-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1b0bf-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-190">The publishing state for the app.</span></span> <span data-ttu-id="1b0bf-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1b0bf-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1b0bf-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1b0bf-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1b0bf-194">committedContentVersion</span></span>|<span data-ttu-id="1b0bf-195">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-195">String</span></span>|<span data-ttu-id="1b0bf-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-196">The internal committed content version.</span></span> <span data-ttu-id="1b0bf-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1b0bf-198">fileName</span><span class="sxs-lookup"><span data-stu-id="1b0bf-198">fileName</span></span>|<span data-ttu-id="1b0bf-199">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-199">String</span></span>|<span data-ttu-id="1b0bf-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-200">The name of the main Lob application file.</span></span> <span data-ttu-id="1b0bf-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1b0bf-202">size</span><span class="sxs-lookup"><span data-stu-id="1b0bf-202">size</span></span>|<span data-ttu-id="1b0bf-203">Int64</span><span class="sxs-lookup"><span data-stu-id="1b0bf-203">Int64</span></span>|<span data-ttu-id="1b0bf-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="1b0bf-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1b0bf-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1b0bf-206">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="1b0bf-206">applicableArchitectures</span></span>|[<span data-ttu-id="1b0bf-207">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1b0bf-207">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1b0bf-208">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-208">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="1b0bf-209">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-209">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md).</span></span> <span data-ttu-id="1b0bf-210">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="1b0bf-211">identityName</span><span class="sxs-lookup"><span data-stu-id="1b0bf-211">identityName</span></span>|<span data-ttu-id="1b0bf-212">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-212">String</span></span>|<span data-ttu-id="1b0bf-213">ID 名。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-213">The Identity Name.</span></span> <span data-ttu-id="1b0bf-214">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-214">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1b0bf-215">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="1b0bf-215">identityPublisherHash</span></span>|<span data-ttu-id="1b0bf-216">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-216">String</span></span>|<span data-ttu-id="1b0bf-217">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-217">The Identity Publisher Hash.</span></span> <span data-ttu-id="1b0bf-218">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-218">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1b0bf-219">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="1b0bf-219">identityResourceIdentifier</span></span>|<span data-ttu-id="1b0bf-220">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-220">String</span></span>|<span data-ttu-id="1b0bf-221">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-221">The Identity Resource Identifier.</span></span> <span data-ttu-id="1b0bf-222">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-222">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1b0bf-223">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1b0bf-223">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1b0bf-224">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1b0bf-224">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1b0bf-225">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-225">The value for the minimum applicable operating system.</span></span> <span data-ttu-id="1b0bf-226">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-226">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1b0bf-227">phoneProductIdentifier</span><span class="sxs-lookup"><span data-stu-id="1b0bf-227">phoneProductIdentifier</span></span>|<span data-ttu-id="1b0bf-228">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-228">String</span></span>|<span data-ttu-id="1b0bf-229">電話の製品識別子です。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-229">The Phone Product Identifier.</span></span> <span data-ttu-id="1b0bf-230">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-230">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1b0bf-231">phonePublisherId</span><span class="sxs-lookup"><span data-stu-id="1b0bf-231">phonePublisherId</span></span>|<span data-ttu-id="1b0bf-232">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-232">String</span></span>|<span data-ttu-id="1b0bf-233">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承した電話のパブリッシャー id。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-233">The Phone Publisher Id. Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1b0bf-234">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1b0bf-234">identityVersion</span></span>|<span data-ttu-id="1b0bf-235">String</span><span class="sxs-lookup"><span data-stu-id="1b0bf-235">String</span></span>|<span data-ttu-id="1b0bf-236">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-236">The identity version.</span></span> <span data-ttu-id="1b0bf-237">[WindowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-237">Inherited from [windowsPhone81AppX](../resources/intune-apps-windowsphone81appx.md)</span></span>|
|<span data-ttu-id="1b0bf-238">appXPackageInformationList</span><span class="sxs-lookup"><span data-stu-id="1b0bf-238">appXPackageInformationList</span></span>|<span data-ttu-id="1b0bf-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1b0bf-239">[windowsPackageInformation](../resources/intune-apps-windowspackageinformation.md) collection</span></span>|<span data-ttu-id="1b0bf-240">AppX パッケージ情報の一覧です。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-240">The list of AppX Package Information.</span></span>|



## <a name="response"></a><span data-ttu-id="1b0bf-241">応答</span><span class="sxs-lookup"><span data-stu-id="1b0bf-241">Response</span></span>
<span data-ttu-id="1b0bf-242">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-242">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81AppXBundle](../resources/intune-apps-windowsphone81appxbundle.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1b0bf-243">例</span><span class="sxs-lookup"><span data-stu-id="1b0bf-243">Example</span></span>
### <a name="request"></a><span data-ttu-id="1b0bf-244">要求</span><span class="sxs-lookup"><span data-stu-id="1b0bf-244">Request</span></span>
<span data-ttu-id="1b0bf-245">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2100

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="1b0bf-246">応答</span><span class="sxs-lookup"><span data-stu-id="1b0bf-246">Response</span></span>
<span data-ttu-id="1b0bf-p127">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1b0bf-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2271

{
  "@odata.type": "#microsoft.graph.windowsPhone81AppXBundle",
  "id": "2433be7c-be7c-2433-7cbe-33247cbe3324",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "phoneProductIdentifier": "Phone Product Identifier value",
  "phonePublisherId": "Phone Publisher Id value",
  "identityVersion": "Identity Version value",
  "appXPackageInformationList": [
    {
      "@odata.type": "microsoft.graph.windowsPackageInformation",
      "applicableArchitecture": "x86",
      "displayName": "Display Name value",
      "identityName": "Identity Name value",
      "identityPublisher": "Identity Publisher value",
      "identityResourceIdentifier": "Identity Resource Identifier value",
      "identityVersion": "Identity Version value",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
        "v8_0": true,
        "v8_1": true,
        "v10_0": true,
        "v10_1607": true,
        "v10_1703": true,
        "v10_1709": true,
        "v10_1803": true
      }
    }
  ]
}
```





