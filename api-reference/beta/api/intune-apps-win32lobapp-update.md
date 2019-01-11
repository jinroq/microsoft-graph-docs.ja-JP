---
title: Win32LobApp を更新します。
description: Win32LobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: c2deac829d1aad6cf0b1a1f3ec4a2a91e7b07c6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864933"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="d4c7f-103">Win32LobApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-103">Update win32LobApp</span></span>

> <span data-ttu-id="d4c7f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d4c7f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d4c7f-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4c7f-107">[Win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4c7f-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4c7f-108">Prerequisites</span></span>
<span data-ttu-id="d4c7f-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4c7f-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4c7f-111">Permission type</span></span>|<span data-ttu-id="d4c7f-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4c7f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4c7f-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4c7f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d4c7f-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4c7f-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4c7f-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4c7f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4c7f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-116">Not supported.</span></span>|
|<span data-ttu-id="d4c7f-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4c7f-117">Application</span></span>|<span data-ttu-id="d4c7f-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4c7f-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4c7f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="d4c7f-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4c7f-120">Request headers</span></span>
|<span data-ttu-id="d4c7f-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4c7f-121">Header</span></span>|<span data-ttu-id="d4c7f-122">値</span><span class="sxs-lookup"><span data-stu-id="d4c7f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4c7f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4c7f-123">Authorization</span></span>|<span data-ttu-id="d4c7f-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4c7f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d4c7f-125">Accept</span></span>|<span data-ttu-id="d4c7f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d4c7f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4c7f-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4c7f-127">Request body</span></span>
<span data-ttu-id="d4c7f-128">要求の本文に[win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="d4c7f-129">[Win32LobApp](../resources/intune-apps-win32lobapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="d4c7f-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4c7f-130">Property</span></span>|<span data-ttu-id="d4c7f-131">種類</span><span class="sxs-lookup"><span data-stu-id="d4c7f-131">Type</span></span>|<span data-ttu-id="d4c7f-132">説明</span><span class="sxs-lookup"><span data-stu-id="d4c7f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4c7f-133">ID</span><span class="sxs-lookup"><span data-stu-id="d4c7f-133">id</span></span>|<span data-ttu-id="d4c7f-134">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-134">String</span></span>|<span data-ttu-id="d4c7f-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-135">Key of the entity.</span></span> <span data-ttu-id="d4c7f-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d4c7f-137">displayName</span></span>|<span data-ttu-id="d4c7f-138">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-138">String</span></span>|<span data-ttu-id="d4c7f-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="d4c7f-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-141">説明</span><span class="sxs-lookup"><span data-stu-id="d4c7f-141">description</span></span>|<span data-ttu-id="d4c7f-142">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-142">String</span></span>|<span data-ttu-id="d4c7f-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-143">The description of the app.</span></span> <span data-ttu-id="d4c7f-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-145">publisher</span><span class="sxs-lookup"><span data-stu-id="d4c7f-145">publisher</span></span>|<span data-ttu-id="d4c7f-146">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-146">String</span></span>|<span data-ttu-id="d4c7f-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-147">The publisher of the app.</span></span> <span data-ttu-id="d4c7f-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="d4c7f-149">largeIcon</span></span>|[<span data-ttu-id="d4c7f-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="d4c7f-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="d4c7f-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="d4c7f-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d4c7f-153">createdDateTime</span></span>|<span data-ttu-id="d4c7f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4c7f-154">DateTimeOffset</span></span>|<span data-ttu-id="d4c7f-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-155">The date and time the app was created.</span></span> <span data-ttu-id="d4c7f-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d4c7f-157">lastModifiedDateTime</span></span>|<span data-ttu-id="d4c7f-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d4c7f-158">DateTimeOffset</span></span>|<span data-ttu-id="d4c7f-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-159">The date and time the app was last modified.</span></span> <span data-ttu-id="d4c7f-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="d4c7f-161">isFeatured</span></span>|<span data-ttu-id="d4c7f-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="d4c7f-162">Boolean</span></span>|<span data-ttu-id="d4c7f-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="d4c7f-164">privacyInformationUrl</span></span>|<span data-ttu-id="d4c7f-165">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-165">String</span></span>|<span data-ttu-id="d4c7f-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-166">The privacy statement Url.</span></span> <span data-ttu-id="d4c7f-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="d4c7f-168">informationUrl</span></span>|<span data-ttu-id="d4c7f-169">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-169">String</span></span>|<span data-ttu-id="d4c7f-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-170">The more information Url.</span></span> <span data-ttu-id="d4c7f-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-172">owner</span><span class="sxs-lookup"><span data-stu-id="d4c7f-172">owner</span></span>|<span data-ttu-id="d4c7f-173">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-173">String</span></span>|<span data-ttu-id="d4c7f-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-174">The owner of the app.</span></span> <span data-ttu-id="d4c7f-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-176">developer</span><span class="sxs-lookup"><span data-stu-id="d4c7f-176">developer</span></span>|<span data-ttu-id="d4c7f-177">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-177">String</span></span>|<span data-ttu-id="d4c7f-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-178">The developer of the app.</span></span> <span data-ttu-id="d4c7f-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-180">notes</span><span class="sxs-lookup"><span data-stu-id="d4c7f-180">notes</span></span>|<span data-ttu-id="d4c7f-181">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-181">String</span></span>|<span data-ttu-id="d4c7f-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-182">Notes for the app.</span></span> <span data-ttu-id="d4c7f-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="d4c7f-184">uploadState</span></span>|<span data-ttu-id="d4c7f-185">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c7f-185">Int32</span></span>|<span data-ttu-id="d4c7f-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-186">The upload state.</span></span> <span data-ttu-id="d4c7f-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="d4c7f-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="d4c7f-188">publishingState</span></span>|[<span data-ttu-id="d4c7f-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="d4c7f-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="d4c7f-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-190">The publishing state for the app.</span></span> <span data-ttu-id="d4c7f-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="d4c7f-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="d4c7f-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="d4c7f-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="d4c7f-194">committedContentVersion</span></span>|<span data-ttu-id="d4c7f-195">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-195">String</span></span>|<span data-ttu-id="d4c7f-196">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-196">The internal committed content version.</span></span> <span data-ttu-id="d4c7f-197">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d4c7f-198">fileName</span><span class="sxs-lookup"><span data-stu-id="d4c7f-198">fileName</span></span>|<span data-ttu-id="d4c7f-199">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-199">String</span></span>|<span data-ttu-id="d4c7f-200">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-200">The name of the main Lob application file.</span></span> <span data-ttu-id="d4c7f-201">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d4c7f-202">size</span><span class="sxs-lookup"><span data-stu-id="d4c7f-202">size</span></span>|<span data-ttu-id="d4c7f-203">Int64</span><span class="sxs-lookup"><span data-stu-id="d4c7f-203">Int64</span></span>|<span data-ttu-id="d4c7f-204">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="d4c7f-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d4c7f-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="d4c7f-206">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="d4c7f-206">installCommandLine</span></span>|<span data-ttu-id="d4c7f-207">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-207">String</span></span>|<span data-ttu-id="d4c7f-208">このアプリケーションをインストールするのにはコマンド ・ ライン</span><span class="sxs-lookup"><span data-stu-id="d4c7f-208">The command line to install this app</span></span>|
|<span data-ttu-id="d4c7f-209">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="d4c7f-209">uninstallCommandLine</span></span>|<span data-ttu-id="d4c7f-210">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-210">String</span></span>|<span data-ttu-id="d4c7f-211">このアプリケーションをアンインストールするのにはコマンド ・ ライン</span><span class="sxs-lookup"><span data-stu-id="d4c7f-211">The command line to uninstall this app</span></span>|
|<span data-ttu-id="d4c7f-212">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="d4c7f-212">applicableArchitectures</span></span>|[<span data-ttu-id="d4c7f-213">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="d4c7f-213">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="d4c7f-214">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-214">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="d4c7f-215">可能な値は、`none`、`x86`、`x64`、`arm`、`neutral` です。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-215">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="d4c7f-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d4c7f-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="d4c7f-217">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="d4c7f-217">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="d4c7f-218">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="d4c7f-219">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="d4c7f-219">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="d4c7f-220">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c7f-220">Int32</span></span>|<span data-ttu-id="d4c7f-221">このアプリケーションをインストールするために必要な最小空きディスク容量の値。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-221">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="d4c7f-222">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="d4c7f-222">minimumMemoryInMB</span></span>|<span data-ttu-id="d4c7f-223">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c7f-223">Int32</span></span>|<span data-ttu-id="d4c7f-224">このアプリケーションをインストールするために必要な物理メモリの最小の値。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-224">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="d4c7f-225">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="d4c7f-225">minimumNumberOfProcessors</span></span>|<span data-ttu-id="d4c7f-226">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c7f-226">Int32</span></span>|<span data-ttu-id="d4c7f-227">このアプリケーションをインストールするために必要な最小のプロセッサの数の値。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-227">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="d4c7f-228">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="d4c7f-228">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="d4c7f-229">Int32</span><span class="sxs-lookup"><span data-stu-id="d4c7f-229">Int32</span></span>|<span data-ttu-id="d4c7f-230">このアプリケーションをインストールするために必要な最低限の CPU 速度の値です。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-230">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="d4c7f-231">detectionRules</span><span class="sxs-lookup"><span data-stu-id="d4c7f-231">detectionRules</span></span>|<span data-ttu-id="d4c7f-232">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d4c7f-232">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="d4c7f-233">Win32 基幹業務 (LoB) アプリケーションを検出する検出ルールです。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-233">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="d4c7f-234">installExperience</span><span class="sxs-lookup"><span data-stu-id="d4c7f-234">installExperience</span></span>|[<span data-ttu-id="d4c7f-235">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="d4c7f-235">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="d4c7f-236">このアプリケーションのインストール経験。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-236">The install experience for this app.</span></span>|
|<span data-ttu-id="d4c7f-237">開始</span><span class="sxs-lookup"><span data-stu-id="d4c7f-237">returnCodes</span></span>|<span data-ttu-id="d4c7f-238">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d4c7f-238">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="d4c7f-239">リターン コードは、インストール時の動作を転記します。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-239">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="d4c7f-240">msiInformation</span><span class="sxs-lookup"><span data-stu-id="d4c7f-240">msiInformation</span></span>|[<span data-ttu-id="d4c7f-241">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="d4c7f-241">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="d4c7f-242">この Win32 アプリケーションでは、MSI アプリケーションの場合は、MSI 詳細です。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-242">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="d4c7f-243">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="d4c7f-243">setupFilePath</span></span>|<span data-ttu-id="d4c7f-244">String</span><span class="sxs-lookup"><span data-stu-id="d4c7f-244">String</span></span>|<span data-ttu-id="d4c7f-245">暗号化された Win32LobApp パッケージのセットアップ ファイルの相対パスです。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-245">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="d4c7f-246">応答</span><span class="sxs-lookup"><span data-stu-id="d4c7f-246">Response</span></span>
<span data-ttu-id="d4c7f-247">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-247">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4c7f-248">例</span><span class="sxs-lookup"><span data-stu-id="d4c7f-248">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4c7f-249">要求</span><span class="sxs-lookup"><span data-stu-id="d4c7f-249">Request</span></span>
<span data-ttu-id="d4c7f-250">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2214

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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```

### <a name="response"></a><span data-ttu-id="d4c7f-251">応答</span><span class="sxs-lookup"><span data-stu-id="d4c7f-251">Response</span></span>
<span data-ttu-id="d4c7f-p121">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4c7f-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2372

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
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
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "detectionRules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryDetection",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "detectionType": "exists",
      "operator": "equal",
      "detectionValue": "Detection Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser"
  },
  "setupFilePath": "Setup File Path value"
}
```





