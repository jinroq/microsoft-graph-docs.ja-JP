---
title: Win32LobApp を更新します。
description: Win32LobApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 962059965abb2691ba1777518ad8aabc64adafe7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405339"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="1ef89-103">Win32LobApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="1ef89-103">Update win32LobApp</span></span>

> <span data-ttu-id="1ef89-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1ef89-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1ef89-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ef89-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1ef89-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ef89-107">[Win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1ef89-107">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ef89-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1ef89-108">Prerequisites</span></span>
<span data-ttu-id="1ef89-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1ef89-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1ef89-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1ef89-111">Permission type</span></span>|<span data-ttu-id="1ef89-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1ef89-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ef89-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1ef89-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1ef89-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ef89-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1ef89-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1ef89-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ef89-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ef89-116">Not supported.</span></span>|
|<span data-ttu-id="1ef89-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1ef89-117">Application</span></span>|<span data-ttu-id="1ef89-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1ef89-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ef89-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1ef89-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="1ef89-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ef89-120">Request headers</span></span>
|<span data-ttu-id="1ef89-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1ef89-121">Header</span></span>|<span data-ttu-id="1ef89-122">値</span><span class="sxs-lookup"><span data-stu-id="1ef89-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ef89-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1ef89-123">Authorization</span></span>|<span data-ttu-id="1ef89-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1ef89-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ef89-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1ef89-125">Accept</span></span>|<span data-ttu-id="1ef89-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1ef89-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ef89-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1ef89-127">Request body</span></span>
<span data-ttu-id="1ef89-128">要求の本文に[win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="1ef89-128">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="1ef89-129">[Win32LobApp](../resources/intune-apps-win32lobapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="1ef89-129">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="1ef89-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1ef89-130">Property</span></span>|<span data-ttu-id="1ef89-131">型</span><span class="sxs-lookup"><span data-stu-id="1ef89-131">Type</span></span>|<span data-ttu-id="1ef89-132">説明</span><span class="sxs-lookup"><span data-stu-id="1ef89-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ef89-133">id</span><span class="sxs-lookup"><span data-stu-id="1ef89-133">id</span></span>|<span data-ttu-id="1ef89-134">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-134">String</span></span>|<span data-ttu-id="1ef89-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1ef89-135">Key of the entity.</span></span> <span data-ttu-id="1ef89-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-137">displayName</span><span class="sxs-lookup"><span data-stu-id="1ef89-137">displayName</span></span>|<span data-ttu-id="1ef89-138">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-138">String</span></span>|<span data-ttu-id="1ef89-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="1ef89-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1ef89-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-141">説明</span><span class="sxs-lookup"><span data-stu-id="1ef89-141">description</span></span>|<span data-ttu-id="1ef89-142">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-142">String</span></span>|<span data-ttu-id="1ef89-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="1ef89-143">The description of the app.</span></span> <span data-ttu-id="1ef89-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-145">publisher</span><span class="sxs-lookup"><span data-stu-id="1ef89-145">publisher</span></span>|<span data-ttu-id="1ef89-146">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-146">String</span></span>|<span data-ttu-id="1ef89-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="1ef89-147">The publisher of the app.</span></span> <span data-ttu-id="1ef89-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1ef89-149">largeIcon</span></span>|[<span data-ttu-id="1ef89-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1ef89-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1ef89-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="1ef89-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1ef89-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1ef89-153">createdDateTime</span></span>|<span data-ttu-id="1ef89-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ef89-154">DateTimeOffset</span></span>|<span data-ttu-id="1ef89-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1ef89-155">The date and time the app was created.</span></span> <span data-ttu-id="1ef89-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ef89-157">lastModifiedDateTime</span></span>|<span data-ttu-id="1ef89-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ef89-158">DateTimeOffset</span></span>|<span data-ttu-id="1ef89-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="1ef89-159">The date and time the app was last modified.</span></span> <span data-ttu-id="1ef89-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1ef89-161">isFeatured</span></span>|<span data-ttu-id="1ef89-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef89-162">Boolean</span></span>|<span data-ttu-id="1ef89-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1ef89-164">privacyInformationUrl</span></span>|<span data-ttu-id="1ef89-165">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-165">String</span></span>|<span data-ttu-id="1ef89-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="1ef89-166">The privacy statement Url.</span></span> <span data-ttu-id="1ef89-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1ef89-168">informationUrl</span></span>|<span data-ttu-id="1ef89-169">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-169">String</span></span>|<span data-ttu-id="1ef89-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="1ef89-170">The more information Url.</span></span> <span data-ttu-id="1ef89-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-172">owner</span><span class="sxs-lookup"><span data-stu-id="1ef89-172">owner</span></span>|<span data-ttu-id="1ef89-173">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-173">String</span></span>|<span data-ttu-id="1ef89-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="1ef89-174">The owner of the app.</span></span> <span data-ttu-id="1ef89-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-176">developer</span><span class="sxs-lookup"><span data-stu-id="1ef89-176">developer</span></span>|<span data-ttu-id="1ef89-177">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-177">String</span></span>|<span data-ttu-id="1ef89-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="1ef89-178">The developer of the app.</span></span> <span data-ttu-id="1ef89-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-180">notes</span><span class="sxs-lookup"><span data-stu-id="1ef89-180">notes</span></span>|<span data-ttu-id="1ef89-181">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-181">String</span></span>|<span data-ttu-id="1ef89-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="1ef89-182">Notes for the app.</span></span> <span data-ttu-id="1ef89-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="1ef89-184">uploadState</span></span>|<span data-ttu-id="1ef89-185">Int32</span><span class="sxs-lookup"><span data-stu-id="1ef89-185">Int32</span></span>|<span data-ttu-id="1ef89-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-186">The upload state.</span></span> <span data-ttu-id="1ef89-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="1ef89-188">publishingState</span></span>|[<span data-ttu-id="1ef89-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1ef89-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1ef89-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="1ef89-190">The publishing state for the app.</span></span> <span data-ttu-id="1ef89-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="1ef89-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1ef89-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1ef89-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1ef89-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1ef89-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1ef89-194">isAssigned</span></span>|<span data-ttu-id="1ef89-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ef89-195">Boolean</span></span>|<span data-ttu-id="1ef89-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1ef89-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1ef89-198">roleScopeTagIds</span></span>|<span data-ttu-id="1ef89-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1ef89-199">String collection</span></span>|<span data-ttu-id="1ef89-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1ef89-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1ef89-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1ef89-202">committedContentVersion</span></span>|<span data-ttu-id="1ef89-203">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-203">String</span></span>|<span data-ttu-id="1ef89-204">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1ef89-204">The internal committed content version.</span></span> <span data-ttu-id="1ef89-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1ef89-206">fileName</span><span class="sxs-lookup"><span data-stu-id="1ef89-206">fileName</span></span>|<span data-ttu-id="1ef89-207">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-207">String</span></span>|<span data-ttu-id="1ef89-208">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="1ef89-208">The name of the main Lob application file.</span></span> <span data-ttu-id="1ef89-209">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1ef89-210">size</span><span class="sxs-lookup"><span data-stu-id="1ef89-210">size</span></span>|<span data-ttu-id="1ef89-211">Int64</span><span class="sxs-lookup"><span data-stu-id="1ef89-211">Int64</span></span>|<span data-ttu-id="1ef89-212">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="1ef89-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="1ef89-213">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1ef89-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1ef89-214">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="1ef89-214">installCommandLine</span></span>|<span data-ttu-id="1ef89-215">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-215">String</span></span>|<span data-ttu-id="1ef89-216">このアプリケーションをインストールするのにはコマンド ・ ライン</span><span class="sxs-lookup"><span data-stu-id="1ef89-216">The command line to install this app</span></span>|
|<span data-ttu-id="1ef89-217">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="1ef89-217">uninstallCommandLine</span></span>|<span data-ttu-id="1ef89-218">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-218">String</span></span>|<span data-ttu-id="1ef89-219">このアプリケーションをアンインストールするのにはコマンド ・ ライン</span><span class="sxs-lookup"><span data-stu-id="1ef89-219">The command line to uninstall this app</span></span>|
|<span data-ttu-id="1ef89-220">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="1ef89-220">applicableArchitectures</span></span>|[<span data-ttu-id="1ef89-221">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="1ef89-221">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="1ef89-222">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="1ef89-222">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="1ef89-223">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="1ef89-223">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="1ef89-224">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1ef89-224">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1ef89-225">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1ef89-225">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="1ef89-226">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-226">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1ef89-227">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="1ef89-227">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="1ef89-228">Int32</span><span class="sxs-lookup"><span data-stu-id="1ef89-228">Int32</span></span>|<span data-ttu-id="1ef89-229">このアプリケーションをインストールするために必要な最小空きディスク容量の値。</span><span class="sxs-lookup"><span data-stu-id="1ef89-229">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="1ef89-230">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="1ef89-230">minimumMemoryInMB</span></span>|<span data-ttu-id="1ef89-231">Int32</span><span class="sxs-lookup"><span data-stu-id="1ef89-231">Int32</span></span>|<span data-ttu-id="1ef89-232">このアプリケーションをインストールするために必要な物理メモリの最小の値。</span><span class="sxs-lookup"><span data-stu-id="1ef89-232">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="1ef89-233">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="1ef89-233">minimumNumberOfProcessors</span></span>|<span data-ttu-id="1ef89-234">Int32</span><span class="sxs-lookup"><span data-stu-id="1ef89-234">Int32</span></span>|<span data-ttu-id="1ef89-235">このアプリケーションをインストールするために必要な最小のプロセッサの数の値。</span><span class="sxs-lookup"><span data-stu-id="1ef89-235">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="1ef89-236">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="1ef89-236">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="1ef89-237">Int32</span><span class="sxs-lookup"><span data-stu-id="1ef89-237">Int32</span></span>|<span data-ttu-id="1ef89-238">このアプリケーションをインストールするために必要な最低限の CPU 速度の値です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-238">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="1ef89-239">detectionRules</span><span class="sxs-lookup"><span data-stu-id="1ef89-239">detectionRules</span></span>|<span data-ttu-id="1ef89-240">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ef89-240">[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md) collection</span></span>|<span data-ttu-id="1ef89-241">Win32 基幹業務 (LoB) アプリケーションを検出する検出ルールです。</span><span class="sxs-lookup"><span data-stu-id="1ef89-241">The detection rules to detect Win32 Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1ef89-242">installExperience</span><span class="sxs-lookup"><span data-stu-id="1ef89-242">installExperience</span></span>|[<span data-ttu-id="1ef89-243">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="1ef89-243">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="1ef89-244">このアプリケーションのインストール経験。</span><span class="sxs-lookup"><span data-stu-id="1ef89-244">The install experience for this app.</span></span>|
|<span data-ttu-id="1ef89-245">開始</span><span class="sxs-lookup"><span data-stu-id="1ef89-245">returnCodes</span></span>|<span data-ttu-id="1ef89-246">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="1ef89-246">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="1ef89-247">リターン コードは、インストール時の動作を転記します。</span><span class="sxs-lookup"><span data-stu-id="1ef89-247">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="1ef89-248">msiInformation</span><span class="sxs-lookup"><span data-stu-id="1ef89-248">msiInformation</span></span>|[<span data-ttu-id="1ef89-249">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="1ef89-249">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="1ef89-250">この Win32 アプリケーションでは、MSI アプリケーションの場合は、MSI 詳細です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-250">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="1ef89-251">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="1ef89-251">setupFilePath</span></span>|<span data-ttu-id="1ef89-252">String</span><span class="sxs-lookup"><span data-stu-id="1ef89-252">String</span></span>|<span data-ttu-id="1ef89-253">暗号化された Win32LobApp パッケージのセットアップ ファイルの相対パスです。</span><span class="sxs-lookup"><span data-stu-id="1ef89-253">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|



## <a name="response"></a><span data-ttu-id="1ef89-254">応答</span><span class="sxs-lookup"><span data-stu-id="1ef89-254">Response</span></span>
<span data-ttu-id="1ef89-255">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[win32LobApp](../resources/intune-apps-win32lobapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="1ef89-255">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ef89-256">例</span><span class="sxs-lookup"><span data-stu-id="1ef89-256">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ef89-257">要求</span><span class="sxs-lookup"><span data-stu-id="1ef89-257">Request</span></span>
<span data-ttu-id="1ef89-258">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1ef89-258">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2285

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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

### <a name="response"></a><span data-ttu-id="1ef89-259">応答</span><span class="sxs-lookup"><span data-stu-id="1ef89-259">Response</span></span>
<span data-ttu-id="1ef89-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1ef89-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2457

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
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
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




