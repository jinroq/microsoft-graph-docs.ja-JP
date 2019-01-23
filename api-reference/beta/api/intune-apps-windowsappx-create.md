---
title: WindowsAppX を作成します。
description: 新しい windowsAppX オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1bba1587ababb35a608663865209ad27d5f67738
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420319"
---
# <a name="create-windowsappx"></a><span data-ttu-id="ba040-103">WindowsAppX を作成します。</span><span class="sxs-lookup"><span data-stu-id="ba040-103">Create windowsAppX</span></span>

> <span data-ttu-id="ba040-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ba040-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ba040-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba040-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba040-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba040-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba040-107">新しい[windowsAppX](../resources/intune-apps-windowsappx.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ba040-107">Create a new [windowsAppX](../resources/intune-apps-windowsappx.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba040-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ba040-108">Prerequisites</span></span>
<span data-ttu-id="ba040-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba040-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ba040-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba040-111">Permission type</span></span>|<span data-ttu-id="ba040-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba040-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba040-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba040-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba040-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba040-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ba040-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba040-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba040-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba040-116">Not supported.</span></span>|
|<span data-ttu-id="ba040-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba040-117">Application</span></span>|<span data-ttu-id="ba040-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba040-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba040-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba040-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="ba040-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba040-120">Request headers</span></span>
|<span data-ttu-id="ba040-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba040-121">Header</span></span>|<span data-ttu-id="ba040-122">値</span><span class="sxs-lookup"><span data-stu-id="ba040-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba040-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba040-123">Authorization</span></span>|<span data-ttu-id="ba040-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ba040-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba040-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ba040-125">Accept</span></span>|<span data-ttu-id="ba040-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba040-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba040-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba040-127">Request body</span></span>
<span data-ttu-id="ba040-128">要求の本文に windowsAppX オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="ba040-128">In the request body, supply a JSON representation for the windowsAppX object.</span></span>

<span data-ttu-id="ba040-129">次の表は、windowsAppX を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ba040-129">The following table shows the properties that are required when you create the windowsAppX.</span></span>

|<span data-ttu-id="ba040-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba040-130">Property</span></span>|<span data-ttu-id="ba040-131">型</span><span class="sxs-lookup"><span data-stu-id="ba040-131">Type</span></span>|<span data-ttu-id="ba040-132">説明</span><span class="sxs-lookup"><span data-stu-id="ba040-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba040-133">id</span><span class="sxs-lookup"><span data-stu-id="ba040-133">id</span></span>|<span data-ttu-id="ba040-134">String</span><span class="sxs-lookup"><span data-stu-id="ba040-134">String</span></span>|<span data-ttu-id="ba040-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ba040-135">Key of the entity.</span></span> <span data-ttu-id="ba040-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ba040-137">displayName</span></span>|<span data-ttu-id="ba040-138">String</span><span class="sxs-lookup"><span data-stu-id="ba040-138">String</span></span>|<span data-ttu-id="ba040-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="ba040-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="ba040-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-141">説明</span><span class="sxs-lookup"><span data-stu-id="ba040-141">description</span></span>|<span data-ttu-id="ba040-142">String</span><span class="sxs-lookup"><span data-stu-id="ba040-142">String</span></span>|<span data-ttu-id="ba040-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="ba040-143">The description of the app.</span></span> <span data-ttu-id="ba040-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-145">publisher</span><span class="sxs-lookup"><span data-stu-id="ba040-145">publisher</span></span>|<span data-ttu-id="ba040-146">String</span><span class="sxs-lookup"><span data-stu-id="ba040-146">String</span></span>|<span data-ttu-id="ba040-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="ba040-147">The publisher of the app.</span></span> <span data-ttu-id="ba040-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="ba040-149">largeIcon</span></span>|[<span data-ttu-id="ba040-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="ba040-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="ba040-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="ba040-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="ba040-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ba040-153">createdDateTime</span></span>|<span data-ttu-id="ba040-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba040-154">DateTimeOffset</span></span>|<span data-ttu-id="ba040-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ba040-155">The date and time the app was created.</span></span> <span data-ttu-id="ba040-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ba040-157">lastModifiedDateTime</span></span>|<span data-ttu-id="ba040-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba040-158">DateTimeOffset</span></span>|<span data-ttu-id="ba040-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ba040-159">The date and time the app was last modified.</span></span> <span data-ttu-id="ba040-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="ba040-161">isFeatured</span></span>|<span data-ttu-id="ba040-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba040-162">Boolean</span></span>|<span data-ttu-id="ba040-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="ba040-164">privacyInformationUrl</span></span>|<span data-ttu-id="ba040-165">String</span><span class="sxs-lookup"><span data-stu-id="ba040-165">String</span></span>|<span data-ttu-id="ba040-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="ba040-166">The privacy statement Url.</span></span> <span data-ttu-id="ba040-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="ba040-168">informationUrl</span></span>|<span data-ttu-id="ba040-169">String</span><span class="sxs-lookup"><span data-stu-id="ba040-169">String</span></span>|<span data-ttu-id="ba040-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="ba040-170">The more information Url.</span></span> <span data-ttu-id="ba040-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-172">owner</span><span class="sxs-lookup"><span data-stu-id="ba040-172">owner</span></span>|<span data-ttu-id="ba040-173">String</span><span class="sxs-lookup"><span data-stu-id="ba040-173">String</span></span>|<span data-ttu-id="ba040-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="ba040-174">The owner of the app.</span></span> <span data-ttu-id="ba040-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-176">developer</span><span class="sxs-lookup"><span data-stu-id="ba040-176">developer</span></span>|<span data-ttu-id="ba040-177">String</span><span class="sxs-lookup"><span data-stu-id="ba040-177">String</span></span>|<span data-ttu-id="ba040-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="ba040-178">The developer of the app.</span></span> <span data-ttu-id="ba040-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-180">notes</span><span class="sxs-lookup"><span data-stu-id="ba040-180">notes</span></span>|<span data-ttu-id="ba040-181">String</span><span class="sxs-lookup"><span data-stu-id="ba040-181">String</span></span>|<span data-ttu-id="ba040-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="ba040-182">Notes for the app.</span></span> <span data-ttu-id="ba040-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="ba040-184">uploadState</span></span>|<span data-ttu-id="ba040-185">Int32</span><span class="sxs-lookup"><span data-stu-id="ba040-185">Int32</span></span>|<span data-ttu-id="ba040-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="ba040-186">The upload state.</span></span> <span data-ttu-id="ba040-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="ba040-188">publishingState</span></span>|[<span data-ttu-id="ba040-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="ba040-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="ba040-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="ba040-190">The publishing state for the app.</span></span> <span data-ttu-id="ba040-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="ba040-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="ba040-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="ba040-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="ba040-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="ba040-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="ba040-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ba040-194">isAssigned</span></span>|<span data-ttu-id="ba040-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba040-195">Boolean</span></span>|<span data-ttu-id="ba040-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="ba040-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="ba040-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ba040-198">roleScopeTagIds</span></span>|<span data-ttu-id="ba040-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="ba040-199">String collection</span></span>|<span data-ttu-id="ba040-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="ba040-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="ba040-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="ba040-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="ba040-202">committedContentVersion</span></span>|<span data-ttu-id="ba040-203">String</span><span class="sxs-lookup"><span data-stu-id="ba040-203">String</span></span>|<span data-ttu-id="ba040-204">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ba040-204">The internal committed content version.</span></span> <span data-ttu-id="ba040-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ba040-206">fileName</span><span class="sxs-lookup"><span data-stu-id="ba040-206">fileName</span></span>|<span data-ttu-id="ba040-207">String</span><span class="sxs-lookup"><span data-stu-id="ba040-207">String</span></span>|<span data-ttu-id="ba040-208">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="ba040-208">The name of the main Lob application file.</span></span> <span data-ttu-id="ba040-209">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ba040-210">size</span><span class="sxs-lookup"><span data-stu-id="ba040-210">size</span></span>|<span data-ttu-id="ba040-211">Int64</span><span class="sxs-lookup"><span data-stu-id="ba040-211">Int64</span></span>|<span data-ttu-id="ba040-212">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="ba040-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="ba040-213">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ba040-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="ba040-214">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="ba040-214">applicableArchitectures</span></span>|[<span data-ttu-id="ba040-215">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="ba040-215">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="ba040-216">このアプリを実行できる Windows アーキテクチャ。</span><span class="sxs-lookup"><span data-stu-id="ba040-216">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="ba040-217">使用可能な値: `none`、`x86`、`x64`、`arm`、`neutral`、`arm64`。</span><span class="sxs-lookup"><span data-stu-id="ba040-217">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`, `arm64`.</span></span>|
|<span data-ttu-id="ba040-218">identityName</span><span class="sxs-lookup"><span data-stu-id="ba040-218">identityName</span></span>|<span data-ttu-id="ba040-219">String</span><span class="sxs-lookup"><span data-stu-id="ba040-219">String</span></span>|<span data-ttu-id="ba040-220">ID 名。</span><span class="sxs-lookup"><span data-stu-id="ba040-220">The Identity Name.</span></span>|
|<span data-ttu-id="ba040-221">identityPublisherHash</span><span class="sxs-lookup"><span data-stu-id="ba040-221">identityPublisherHash</span></span>|<span data-ttu-id="ba040-222">String</span><span class="sxs-lookup"><span data-stu-id="ba040-222">String</span></span>|<span data-ttu-id="ba040-223">ID の発行元のハッシュ。</span><span class="sxs-lookup"><span data-stu-id="ba040-223">The Identity Publisher Hash.</span></span>|
|<span data-ttu-id="ba040-224">identityResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="ba040-224">identityResourceIdentifier</span></span>|<span data-ttu-id="ba040-225">String</span><span class="sxs-lookup"><span data-stu-id="ba040-225">String</span></span>|<span data-ttu-id="ba040-226">ID のリソースの識別子。</span><span class="sxs-lookup"><span data-stu-id="ba040-226">The Identity Resource Identifier.</span></span>|
|<span data-ttu-id="ba040-227">isBundle</span><span class="sxs-lookup"><span data-stu-id="ba040-227">isBundle</span></span>|<span data-ttu-id="ba040-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="ba040-228">Boolean</span></span>|<span data-ttu-id="ba040-229">アプリがバンドルかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ba040-229">Whether or not the app is a bundle.</span></span>|
|<span data-ttu-id="ba040-230">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ba040-230">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="ba040-231">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="ba040-231">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="ba040-232">該当するオペレーティング システムの最小の値です。</span><span class="sxs-lookup"><span data-stu-id="ba040-232">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="ba040-233">identityVersion</span><span class="sxs-lookup"><span data-stu-id="ba040-233">identityVersion</span></span>|<span data-ttu-id="ba040-234">String</span><span class="sxs-lookup"><span data-stu-id="ba040-234">String</span></span>|<span data-ttu-id="ba040-235">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="ba040-235">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="ba040-236">応答</span><span class="sxs-lookup"><span data-stu-id="ba040-236">Response</span></span>
<span data-ttu-id="ba040-237">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[windowsAppX](../resources/intune-apps-windowsappx.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="ba040-237">If successful, this method returns a `201 Created` response code and a [windowsAppX](../resources/intune-apps-windowsappx.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba040-238">例</span><span class="sxs-lookup"><span data-stu-id="ba040-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba040-239">要求</span><span class="sxs-lookup"><span data-stu-id="ba040-239">Request</span></span>
<span data-ttu-id="ba040-240">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ba040-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1340

{
  "@odata.type": "#microsoft.graph.windowsAppX",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="ba040-241">応答</span><span class="sxs-lookup"><span data-stu-id="ba040-241">Response</span></span>
<span data-ttu-id="ba040-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ba040-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1512

{
  "@odata.type": "#microsoft.graph.windowsAppX",
  "id": "b5179a93-9a93-b517-939a-17b5939a17b5",
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
  "applicableArchitectures": "x86",
  "identityName": "Identity Name value",
  "identityPublisherHash": "Identity Publisher Hash value",
  "identityResourceIdentifier": "Identity Resource Identifier value",
  "isBundle": true,
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
  "identityVersion": "Identity Version value"
}
```




