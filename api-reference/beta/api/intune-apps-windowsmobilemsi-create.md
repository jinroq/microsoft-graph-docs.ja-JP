---
title: Create windowsMobileMSI
description: 新しく windowsMobileMSI オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a794ea35428b606c825dc95de3a76aa839708489
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405115"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="67c41-103">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="67c41-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="67c41-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="67c41-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="67c41-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c41-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67c41-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="67c41-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67c41-107">新しく [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="67c41-107">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67c41-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="67c41-108">Prerequisites</span></span>
<span data-ttu-id="67c41-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="67c41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="67c41-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="67c41-111">Permission type</span></span>|<span data-ttu-id="67c41-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="67c41-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67c41-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="67c41-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67c41-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67c41-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67c41-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="67c41-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67c41-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c41-116">Not supported.</span></span>|
|<span data-ttu-id="67c41-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="67c41-117">Application</span></span>|<span data-ttu-id="67c41-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="67c41-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67c41-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="67c41-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="67c41-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67c41-120">Request headers</span></span>
|<span data-ttu-id="67c41-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="67c41-121">Header</span></span>|<span data-ttu-id="67c41-122">値</span><span class="sxs-lookup"><span data-stu-id="67c41-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67c41-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="67c41-123">Authorization</span></span>|<span data-ttu-id="67c41-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="67c41-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67c41-125">Accept</span><span class="sxs-lookup"><span data-stu-id="67c41-125">Accept</span></span>|<span data-ttu-id="67c41-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67c41-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67c41-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="67c41-127">Request body</span></span>
<span data-ttu-id="67c41-128">要求本文で、windowsMobileMSI オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="67c41-128">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="67c41-129">次の表に、windowsMobileMSI 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="67c41-129">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="67c41-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="67c41-130">Property</span></span>|<span data-ttu-id="67c41-131">型</span><span class="sxs-lookup"><span data-stu-id="67c41-131">Type</span></span>|<span data-ttu-id="67c41-132">説明</span><span class="sxs-lookup"><span data-stu-id="67c41-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67c41-133">id</span><span class="sxs-lookup"><span data-stu-id="67c41-133">id</span></span>|<span data-ttu-id="67c41-134">String</span><span class="sxs-lookup"><span data-stu-id="67c41-134">String</span></span>|<span data-ttu-id="67c41-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="67c41-135">Key of the entity.</span></span> <span data-ttu-id="67c41-136">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-137">displayName</span><span class="sxs-lookup"><span data-stu-id="67c41-137">displayName</span></span>|<span data-ttu-id="67c41-138">String</span><span class="sxs-lookup"><span data-stu-id="67c41-138">String</span></span>|<span data-ttu-id="67c41-139">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="67c41-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="67c41-140">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-141">説明</span><span class="sxs-lookup"><span data-stu-id="67c41-141">description</span></span>|<span data-ttu-id="67c41-142">String</span><span class="sxs-lookup"><span data-stu-id="67c41-142">String</span></span>|<span data-ttu-id="67c41-143">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="67c41-143">The description of the app.</span></span> <span data-ttu-id="67c41-144">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-145">publisher</span><span class="sxs-lookup"><span data-stu-id="67c41-145">publisher</span></span>|<span data-ttu-id="67c41-146">String</span><span class="sxs-lookup"><span data-stu-id="67c41-146">String</span></span>|<span data-ttu-id="67c41-147">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="67c41-147">The publisher of the app.</span></span> <span data-ttu-id="67c41-148">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="67c41-149">largeIcon</span></span>|[<span data-ttu-id="67c41-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="67c41-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="67c41-151">アプリの詳細に表示され、アイコンのアップロードに使用される大きなアイコン。</span><span class="sxs-lookup"><span data-stu-id="67c41-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="67c41-152">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67c41-153">createdDateTime</span></span>|<span data-ttu-id="67c41-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67c41-154">DateTimeOffset</span></span>|<span data-ttu-id="67c41-155">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="67c41-155">The date and time the app was created.</span></span> <span data-ttu-id="67c41-156">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67c41-157">lastModifiedDateTime</span></span>|<span data-ttu-id="67c41-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67c41-158">DateTimeOffset</span></span>|<span data-ttu-id="67c41-159">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="67c41-159">The date and time the app was last modified.</span></span> <span data-ttu-id="67c41-160">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="67c41-161">isFeatured</span></span>|<span data-ttu-id="67c41-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c41-162">Boolean</span></span>|<span data-ttu-id="67c41-163">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="67c41-164">privacyInformationUrl</span></span>|<span data-ttu-id="67c41-165">String</span><span class="sxs-lookup"><span data-stu-id="67c41-165">String</span></span>|<span data-ttu-id="67c41-166">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="67c41-166">The privacy statement Url.</span></span> <span data-ttu-id="67c41-167">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="67c41-168">informationUrl</span></span>|<span data-ttu-id="67c41-169">String</span><span class="sxs-lookup"><span data-stu-id="67c41-169">String</span></span>|<span data-ttu-id="67c41-170">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="67c41-170">The more information Url.</span></span> <span data-ttu-id="67c41-171">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-172">owner</span><span class="sxs-lookup"><span data-stu-id="67c41-172">owner</span></span>|<span data-ttu-id="67c41-173">String</span><span class="sxs-lookup"><span data-stu-id="67c41-173">String</span></span>|<span data-ttu-id="67c41-174">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="67c41-174">The owner of the app.</span></span> <span data-ttu-id="67c41-175">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-176">developer</span><span class="sxs-lookup"><span data-stu-id="67c41-176">developer</span></span>|<span data-ttu-id="67c41-177">String</span><span class="sxs-lookup"><span data-stu-id="67c41-177">String</span></span>|<span data-ttu-id="67c41-178">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="67c41-178">The developer of the app.</span></span> <span data-ttu-id="67c41-179">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-180">notes</span><span class="sxs-lookup"><span data-stu-id="67c41-180">notes</span></span>|<span data-ttu-id="67c41-181">String</span><span class="sxs-lookup"><span data-stu-id="67c41-181">String</span></span>|<span data-ttu-id="67c41-182">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="67c41-182">Notes for the app.</span></span> <span data-ttu-id="67c41-183">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="67c41-184">uploadState</span></span>|<span data-ttu-id="67c41-185">Int32</span><span class="sxs-lookup"><span data-stu-id="67c41-185">Int32</span></span>|<span data-ttu-id="67c41-186">アップロードの状態です。</span><span class="sxs-lookup"><span data-stu-id="67c41-186">The upload state.</span></span> <span data-ttu-id="67c41-187">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="67c41-188">publishingState</span></span>|[<span data-ttu-id="67c41-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="67c41-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="67c41-190">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="67c41-190">The publishing state for the app.</span></span> <span data-ttu-id="67c41-191">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="67c41-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="67c41-192">[MobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="67c41-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="67c41-193">可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="67c41-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="67c41-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="67c41-194">isAssigned</span></span>|<span data-ttu-id="67c41-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c41-195">Boolean</span></span>|<span data-ttu-id="67c41-196">アプリケーションが少なくとも 1 つのグループに割り当てられているかどうかを示す値です。</span><span class="sxs-lookup"><span data-stu-id="67c41-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="67c41-197">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67c41-198">roleScopeTagIds</span></span>|<span data-ttu-id="67c41-199">String コレクション</span><span class="sxs-lookup"><span data-stu-id="67c41-199">String collection</span></span>|<span data-ttu-id="67c41-200">このモバイル アプリケーションのスコープのタグ id の一覧です。</span><span class="sxs-lookup"><span data-stu-id="67c41-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="67c41-201">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="67c41-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="67c41-202">committedContentVersion</span></span>|<span data-ttu-id="67c41-203">String</span><span class="sxs-lookup"><span data-stu-id="67c41-203">String</span></span>|<span data-ttu-id="67c41-204">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="67c41-204">The internal committed content version.</span></span> <span data-ttu-id="67c41-205">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="67c41-206">fileName</span><span class="sxs-lookup"><span data-stu-id="67c41-206">fileName</span></span>|<span data-ttu-id="67c41-207">String</span><span class="sxs-lookup"><span data-stu-id="67c41-207">String</span></span>|<span data-ttu-id="67c41-208">メインの Lob アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="67c41-208">The name of the main Lob application file.</span></span> <span data-ttu-id="67c41-209">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="67c41-210">size</span><span class="sxs-lookup"><span data-stu-id="67c41-210">size</span></span>|<span data-ttu-id="67c41-211">Int64</span><span class="sxs-lookup"><span data-stu-id="67c41-211">Int64</span></span>|<span data-ttu-id="67c41-212">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="67c41-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="67c41-213">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="67c41-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="67c41-214">commandLine</span><span class="sxs-lookup"><span data-stu-id="67c41-214">commandLine</span></span>|<span data-ttu-id="67c41-215">String</span><span class="sxs-lookup"><span data-stu-id="67c41-215">String</span></span>|<span data-ttu-id="67c41-216">コマンド ライン。</span><span class="sxs-lookup"><span data-stu-id="67c41-216">The command line.</span></span>|
|<span data-ttu-id="67c41-217">productCode</span><span class="sxs-lookup"><span data-stu-id="67c41-217">productCode</span></span>|<span data-ttu-id="67c41-218">String</span><span class="sxs-lookup"><span data-stu-id="67c41-218">String</span></span>|<span data-ttu-id="67c41-219">製品コード。</span><span class="sxs-lookup"><span data-stu-id="67c41-219">The product code.</span></span>|
|<span data-ttu-id="67c41-220">productVersion</span><span class="sxs-lookup"><span data-stu-id="67c41-220">productVersion</span></span>|<span data-ttu-id="67c41-221">String</span><span class="sxs-lookup"><span data-stu-id="67c41-221">String</span></span>|<span data-ttu-id="67c41-222">Windows Mobile MSI 基幹業務 (LoB) アプリの製品のバージョン。</span><span class="sxs-lookup"><span data-stu-id="67c41-222">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="67c41-223">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="67c41-223">ignoreVersionDetection</span></span>|<span data-ttu-id="67c41-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="67c41-224">Boolean</span></span>|<span data-ttu-id="67c41-225">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="67c41-225">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="67c41-226">自己更新機能を使用する Windows Mobile MSI 基幹業務 (LoB) アプリの場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="67c41-226">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="67c41-227">identityVersion</span><span class="sxs-lookup"><span data-stu-id="67c41-227">identityVersion</span></span>|<span data-ttu-id="67c41-228">String</span><span class="sxs-lookup"><span data-stu-id="67c41-228">String</span></span>|<span data-ttu-id="67c41-229">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="67c41-229">The identity version.</span></span>|
|<span data-ttu-id="67c41-230">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="67c41-230">useDeviceContext</span></span>|<span data-ttu-id="67c41-231">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="67c41-231">Boolean</span></span>|<span data-ttu-id="67c41-232">デバイス コンテキストのデュアル モードの MSI をインストールするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="67c41-232">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="67c41-233">True の場合、すべてのユーザーに対してアプリケーションがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="67c41-233">If true, app will be installed for all users.</span></span> <span data-ttu-id="67c41-234">False の場合、アプリケーションはユーザーごとのインストールになります。</span><span class="sxs-lookup"><span data-stu-id="67c41-234">If false, app will be installed per-user.</span></span> <span data-ttu-id="67c41-235">Null の場合、サービスは、MSI パッケージの既定のインストールのコンテキストを使用します。</span><span class="sxs-lookup"><span data-stu-id="67c41-235">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="67c41-236">デュアル モードの MSI が発生した場合は、ユーザーがこの既定値になります。</span><span class="sxs-lookup"><span data-stu-id="67c41-236">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="67c41-237">非デュアル モードのアプリケーション用に設定できません。</span><span class="sxs-lookup"><span data-stu-id="67c41-237">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="67c41-238">アプリケーションの初期作成後は変更できません。</span><span class="sxs-lookup"><span data-stu-id="67c41-238">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="67c41-239">応答</span><span class="sxs-lookup"><span data-stu-id="67c41-239">Response</span></span>
<span data-ttu-id="67c41-240">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="67c41-240">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67c41-241">例</span><span class="sxs-lookup"><span data-stu-id="67c41-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="67c41-242">要求</span><span class="sxs-lookup"><span data-stu-id="67c41-242">Request</span></span>
<span data-ttu-id="67c41-243">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="67c41-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="67c41-244">応答</span><span class="sxs-lookup"><span data-stu-id="67c41-244">Response</span></span>
<span data-ttu-id="67c41-p124">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="67c41-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
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
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




