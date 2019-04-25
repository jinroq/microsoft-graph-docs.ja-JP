---
title: iosLobApp の更新
description: iosLobApp オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31ab4faf738ea103fa0a7236e0adb9ae2cda9ba3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577365"
---
# <a name="update-ioslobapp"></a><span data-ttu-id="1a258-103">iosLobApp の更新</span><span class="sxs-lookup"><span data-stu-id="1a258-103">Update iosLobApp</span></span>

> <span data-ttu-id="1a258-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a258-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a258-105">[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1a258-105">Update the properties of a [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a258-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1a258-106">Prerequisites</span></span>
<span data-ttu-id="1a258-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1a258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a258-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1a258-109">Permission type</span></span>|<span data-ttu-id="1a258-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1a258-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a258-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1a258-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1a258-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a258-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a258-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1a258-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a258-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a258-114">Not supported.</span></span>|
|<span data-ttu-id="1a258-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1a258-115">Application</span></span>|<span data-ttu-id="1a258-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1a258-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a258-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1a258-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="1a258-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a258-118">Request headers</span></span>
|<span data-ttu-id="1a258-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1a258-119">Header</span></span>|<span data-ttu-id="1a258-120">値</span><span class="sxs-lookup"><span data-stu-id="1a258-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a258-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a258-121">Authorization</span></span>|<span data-ttu-id="1a258-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1a258-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a258-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1a258-123">Accept</span></span>|<span data-ttu-id="1a258-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1a258-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a258-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1a258-125">Request body</span></span>
<span data-ttu-id="1a258-126">要求本文で、[iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1a258-126">In the request body, supply a JSON representation for the [iosLobApp](../resources/intune-apps-ioslobapp.md) object.</span></span>

<span data-ttu-id="1a258-127">次の表に、[iosLobApp](../resources/intune-apps-ioslobapp.md) 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1a258-127">The following table shows the properties that are required when you create the [iosLobApp](../resources/intune-apps-ioslobapp.md).</span></span>

|<span data-ttu-id="1a258-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1a258-128">Property</span></span>|<span data-ttu-id="1a258-129">型</span><span class="sxs-lookup"><span data-stu-id="1a258-129">Type</span></span>|<span data-ttu-id="1a258-130">説明</span><span class="sxs-lookup"><span data-stu-id="1a258-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a258-131">id</span><span class="sxs-lookup"><span data-stu-id="1a258-131">id</span></span>|<span data-ttu-id="1a258-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1a258-132">String</span></span>|<span data-ttu-id="1a258-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1a258-133">Key of the entity.</span></span> <span data-ttu-id="1a258-134">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-134">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1a258-135">displayName</span></span>|<span data-ttu-id="1a258-136">String</span><span class="sxs-lookup"><span data-stu-id="1a258-136">String</span></span>|<span data-ttu-id="1a258-137">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="1a258-137">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1a258-138">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-138">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-139">説明</span><span class="sxs-lookup"><span data-stu-id="1a258-139">description</span></span>|<span data-ttu-id="1a258-140">String</span><span class="sxs-lookup"><span data-stu-id="1a258-140">String</span></span>|<span data-ttu-id="1a258-141">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="1a258-141">The description of the app.</span></span> <span data-ttu-id="1a258-142">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-142">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-143">publisher</span><span class="sxs-lookup"><span data-stu-id="1a258-143">publisher</span></span>|<span data-ttu-id="1a258-144">String</span><span class="sxs-lookup"><span data-stu-id="1a258-144">String</span></span>|<span data-ttu-id="1a258-145">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="1a258-145">The publisher of the app.</span></span> <span data-ttu-id="1a258-146">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-146">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-147">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1a258-147">largeIcon</span></span>|[<span data-ttu-id="1a258-148">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1a258-148">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1a258-149">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="1a258-149">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1a258-150">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-150">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1a258-151">createdDateTime</span></span>|<span data-ttu-id="1a258-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a258-152">DateTimeOffset</span></span>|<span data-ttu-id="1a258-153">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1a258-153">The date and time the app was created.</span></span> <span data-ttu-id="1a258-154">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-154">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-155">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1a258-155">lastModifiedDateTime</span></span>|<span data-ttu-id="1a258-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a258-156">DateTimeOffset</span></span>|<span data-ttu-id="1a258-157">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="1a258-157">The date and time the app was last modified.</span></span> <span data-ttu-id="1a258-158">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-158">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-159">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1a258-159">isFeatured</span></span>|<span data-ttu-id="1a258-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="1a258-160">Boolean</span></span>|<span data-ttu-id="1a258-161">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-161">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-162">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1a258-162">privacyInformationUrl</span></span>|<span data-ttu-id="1a258-163">String</span><span class="sxs-lookup"><span data-stu-id="1a258-163">String</span></span>|<span data-ttu-id="1a258-164">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="1a258-164">The privacy statement Url.</span></span> <span data-ttu-id="1a258-165">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-165">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-166">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1a258-166">informationUrl</span></span>|<span data-ttu-id="1a258-167">String</span><span class="sxs-lookup"><span data-stu-id="1a258-167">String</span></span>|<span data-ttu-id="1a258-168">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="1a258-168">The more information Url.</span></span> <span data-ttu-id="1a258-169">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-169">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-170">owner</span><span class="sxs-lookup"><span data-stu-id="1a258-170">owner</span></span>|<span data-ttu-id="1a258-171">String</span><span class="sxs-lookup"><span data-stu-id="1a258-171">String</span></span>|<span data-ttu-id="1a258-172">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="1a258-172">The owner of the app.</span></span> <span data-ttu-id="1a258-173">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-173">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-174">developer</span><span class="sxs-lookup"><span data-stu-id="1a258-174">developer</span></span>|<span data-ttu-id="1a258-175">String</span><span class="sxs-lookup"><span data-stu-id="1a258-175">String</span></span>|<span data-ttu-id="1a258-176">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="1a258-176">The developer of the app.</span></span> <span data-ttu-id="1a258-177">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-177">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-178">notes</span><span class="sxs-lookup"><span data-stu-id="1a258-178">notes</span></span>|<span data-ttu-id="1a258-179">String</span><span class="sxs-lookup"><span data-stu-id="1a258-179">String</span></span>|<span data-ttu-id="1a258-180">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="1a258-180">Notes for the app.</span></span> <span data-ttu-id="1a258-181">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-181">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1a258-182">publishingState</span><span class="sxs-lookup"><span data-stu-id="1a258-182">publishingState</span></span>|[<span data-ttu-id="1a258-183">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1a258-183">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1a258-184">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="1a258-184">The publishing state for the app.</span></span> <span data-ttu-id="1a258-185">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="1a258-185">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1a258-186">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1a258-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1a258-187">可能な値は `notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="1a258-187">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1a258-188">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1a258-188">committedContentVersion</span></span>|<span data-ttu-id="1a258-189">String</span><span class="sxs-lookup"><span data-stu-id="1a258-189">String</span></span>|<span data-ttu-id="1a258-190">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1a258-190">The internal committed content version.</span></span> <span data-ttu-id="1a258-191">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-191">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1a258-192">fileName</span><span class="sxs-lookup"><span data-stu-id="1a258-192">fileName</span></span>|<span data-ttu-id="1a258-193">String</span><span class="sxs-lookup"><span data-stu-id="1a258-193">String</span></span>|<span data-ttu-id="1a258-194">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="1a258-194">The name of the main Lob application file.</span></span> <span data-ttu-id="1a258-195">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-195">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1a258-196">size</span><span class="sxs-lookup"><span data-stu-id="1a258-196">size</span></span>|<span data-ttu-id="1a258-197">Int64</span><span class="sxs-lookup"><span data-stu-id="1a258-197">Int64</span></span>|<span data-ttu-id="1a258-198">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="1a258-198">The total size, including all uploaded files.</span></span> <span data-ttu-id="1a258-199">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1a258-199">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1a258-200">bundleId</span><span class="sxs-lookup"><span data-stu-id="1a258-200">bundleId</span></span>|<span data-ttu-id="1a258-201">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1a258-201">String</span></span>|<span data-ttu-id="1a258-202">ID 名。</span><span class="sxs-lookup"><span data-stu-id="1a258-202">The Identity Name.</span></span>|
|<span data-ttu-id="1a258-203">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="1a258-203">applicableDeviceType</span></span>|[<span data-ttu-id="1a258-204">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="1a258-204">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="1a258-205">このアプリを実行できる iOS アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="1a258-205">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="1a258-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1a258-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="1a258-207">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="1a258-207">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="1a258-208">該当するオペレーティング システムの最小の値。</span><span class="sxs-lookup"><span data-stu-id="1a258-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="1a258-209">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1a258-209">expirationDateTime</span></span>|<span data-ttu-id="1a258-210">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1a258-210">DateTimeOffset</span></span>|<span data-ttu-id="1a258-211">有効期限。</span><span class="sxs-lookup"><span data-stu-id="1a258-211">The expiration time.</span></span>|
|<span data-ttu-id="1a258-212">VersionNumber</span><span class="sxs-lookup"><span data-stu-id="1a258-212">versionNumber</span></span>|<span data-ttu-id="1a258-213">String</span><span class="sxs-lookup"><span data-stu-id="1a258-213">String</span></span>|<span data-ttu-id="1a258-214">iOS 基幹業務 (LoB) アプリのバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="1a258-214">The version number of iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1a258-215">buildNumber</span><span class="sxs-lookup"><span data-stu-id="1a258-215">buildNumber</span></span>|<span data-ttu-id="1a258-216">String</span><span class="sxs-lookup"><span data-stu-id="1a258-216">String</span></span>|<span data-ttu-id="1a258-217">iOS 基幹業務 (LoB) アプリのビルド番号。</span><span class="sxs-lookup"><span data-stu-id="1a258-217">The build number of iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="1a258-218">応答</span><span class="sxs-lookup"><span data-stu-id="1a258-218">Response</span></span>
<span data-ttu-id="1a258-219">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、更新された [iosLobApp](../resources/intune-apps-ioslobapp.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="1a258-219">If successful, this method returns a `200 OK` response code and an updated [iosLobApp](../resources/intune-apps-ioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a258-220">例</span><span class="sxs-lookup"><span data-stu-id="1a258-220">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a258-221">要求</span><span class="sxs-lookup"><span data-stu-id="1a258-221">Request</span></span>
<span data-ttu-id="1a258-222">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1a258-222">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1209

{
  "@odata.type": "#microsoft.graph.iosLobApp",
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
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="1a258-223">応答</span><span class="sxs-lookup"><span data-stu-id="1a258-223">Response</span></span>
<span data-ttu-id="1a258-p118">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1a258-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1381

{
  "@odata.type": "#microsoft.graph.iosLobApp",
  "id": "b34052ea-52ea-b340-ea52-40b3ea5240b3",
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
  "buildNumber": "Build Number value"
}
```



