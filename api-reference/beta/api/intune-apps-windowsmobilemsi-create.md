---
title: Create windowsMobileMSI
description: 新しく windowsMobileMSI オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e9e9ba8c10d80ea75799046b951678d34bf88a2d
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966377"
---
# <a name="create-windowsmobilemsi"></a><span data-ttu-id="1e775-103">Create windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="1e775-103">Create windowsMobileMSI</span></span>

> <span data-ttu-id="1e775-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e775-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e775-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e775-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e775-106">新しく [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1e775-106">Create a new [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e775-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1e775-107">Prerequisites</span></span>
<span data-ttu-id="1e775-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e775-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e775-110">Permission type</span></span>|<span data-ttu-id="1e775-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e775-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e775-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e775-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e775-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e775-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1e775-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e775-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e775-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e775-115">Not supported.</span></span>|
|<span data-ttu-id="1e775-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e775-116">Application</span></span>|<span data-ttu-id="1e775-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e775-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e775-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e775-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="1e775-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e775-119">Request headers</span></span>
|<span data-ttu-id="1e775-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e775-120">Header</span></span>|<span data-ttu-id="1e775-121">値</span><span class="sxs-lookup"><span data-stu-id="1e775-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e775-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e775-122">Authorization</span></span>|<span data-ttu-id="1e775-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e775-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e775-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1e775-124">Accept</span></span>|<span data-ttu-id="1e775-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e775-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e775-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e775-126">Request body</span></span>
<span data-ttu-id="1e775-127">要求本文で、windowsMobileMSI オブジェクト用の JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e775-127">In the request body, supply a JSON representation for the windowsMobileMSI object.</span></span>

<span data-ttu-id="1e775-128">次の表に、windowsMobileMSI 作成時に必要となるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1e775-128">The following table shows the properties that are required when you create the windowsMobileMSI.</span></span>

|<span data-ttu-id="1e775-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e775-129">Property</span></span>|<span data-ttu-id="1e775-130">型</span><span class="sxs-lookup"><span data-stu-id="1e775-130">Type</span></span>|<span data-ttu-id="1e775-131">説明</span><span class="sxs-lookup"><span data-stu-id="1e775-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e775-132">id</span><span class="sxs-lookup"><span data-stu-id="1e775-132">id</span></span>|<span data-ttu-id="1e775-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1e775-133">String</span></span>|<span data-ttu-id="1e775-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1e775-134">Key of the entity.</span></span> <span data-ttu-id="1e775-135">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-136">displayName</span><span class="sxs-lookup"><span data-stu-id="1e775-136">displayName</span></span>|<span data-ttu-id="1e775-137">String</span><span class="sxs-lookup"><span data-stu-id="1e775-137">String</span></span>|<span data-ttu-id="1e775-138">管理者が提供またはインポートしたアプリのタイトル。</span><span class="sxs-lookup"><span data-stu-id="1e775-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="1e775-139">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-140">description</span><span class="sxs-lookup"><span data-stu-id="1e775-140">description</span></span>|<span data-ttu-id="1e775-141">String</span><span class="sxs-lookup"><span data-stu-id="1e775-141">String</span></span>|<span data-ttu-id="1e775-142">アプリの説明。</span><span class="sxs-lookup"><span data-stu-id="1e775-142">The description of the app.</span></span> <span data-ttu-id="1e775-143">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-144">publisher</span><span class="sxs-lookup"><span data-stu-id="1e775-144">publisher</span></span>|<span data-ttu-id="1e775-145">String</span><span class="sxs-lookup"><span data-stu-id="1e775-145">String</span></span>|<span data-ttu-id="1e775-146">アプリの発行元。</span><span class="sxs-lookup"><span data-stu-id="1e775-146">The publisher of the app.</span></span> <span data-ttu-id="1e775-147">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="1e775-148">largeIcon</span></span>|[<span data-ttu-id="1e775-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="1e775-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="1e775-150">アプリの詳細に表示され、アイコンのアップロードに使用される大きいアイコン。</span><span class="sxs-lookup"><span data-stu-id="1e775-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="1e775-151">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e775-152">createdDateTime</span></span>|<span data-ttu-id="1e775-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e775-153">DateTimeOffset</span></span>|<span data-ttu-id="1e775-154">アプリが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1e775-154">The date and time the app was created.</span></span> <span data-ttu-id="1e775-155">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e775-156">lastModifiedDateTime</span></span>|<span data-ttu-id="1e775-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e775-157">DateTimeOffset</span></span>|<span data-ttu-id="1e775-158">アプリが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="1e775-158">The date and time the app was last modified.</span></span> <span data-ttu-id="1e775-159">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="1e775-160">isFeatured</span></span>|<span data-ttu-id="1e775-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e775-161">Boolean</span></span>|<span data-ttu-id="1e775-162">アプリが管理者のおすすめとしてマークされたかどうかを示す値。[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="1e775-163">privacyInformationUrl</span></span>|<span data-ttu-id="1e775-164">String</span><span class="sxs-lookup"><span data-stu-id="1e775-164">String</span></span>|<span data-ttu-id="1e775-165">プライバシーに関する声明の URL。</span><span class="sxs-lookup"><span data-stu-id="1e775-165">The privacy statement Url.</span></span> <span data-ttu-id="1e775-166">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="1e775-167">informationUrl</span></span>|<span data-ttu-id="1e775-168">String</span><span class="sxs-lookup"><span data-stu-id="1e775-168">String</span></span>|<span data-ttu-id="1e775-169">詳細情報の URL。</span><span class="sxs-lookup"><span data-stu-id="1e775-169">The more information Url.</span></span> <span data-ttu-id="1e775-170">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-171">owner</span><span class="sxs-lookup"><span data-stu-id="1e775-171">owner</span></span>|<span data-ttu-id="1e775-172">String</span><span class="sxs-lookup"><span data-stu-id="1e775-172">String</span></span>|<span data-ttu-id="1e775-173">アプリの所有者。</span><span class="sxs-lookup"><span data-stu-id="1e775-173">The owner of the app.</span></span> <span data-ttu-id="1e775-174">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-175">developer</span><span class="sxs-lookup"><span data-stu-id="1e775-175">developer</span></span>|<span data-ttu-id="1e775-176">String</span><span class="sxs-lookup"><span data-stu-id="1e775-176">String</span></span>|<span data-ttu-id="1e775-177">アプリの開発者。</span><span class="sxs-lookup"><span data-stu-id="1e775-177">The developer of the app.</span></span> <span data-ttu-id="1e775-178">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-179">notes</span><span class="sxs-lookup"><span data-stu-id="1e775-179">notes</span></span>|<span data-ttu-id="1e775-180">String</span><span class="sxs-lookup"><span data-stu-id="1e775-180">String</span></span>|<span data-ttu-id="1e775-181">アプリ用のメモ。</span><span class="sxs-lookup"><span data-stu-id="1e775-181">Notes for the app.</span></span> <span data-ttu-id="1e775-182">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-183">uploadState</span><span class="sxs-lookup"><span data-stu-id="1e775-183">uploadState</span></span>|<span data-ttu-id="1e775-184">Int32</span><span class="sxs-lookup"><span data-stu-id="1e775-184">Int32</span></span>|<span data-ttu-id="1e775-185">アップロード状態。</span><span class="sxs-lookup"><span data-stu-id="1e775-185">The upload state.</span></span> <span data-ttu-id="1e775-186">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-186">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-187">publishingState</span><span class="sxs-lookup"><span data-stu-id="1e775-187">publishingState</span></span>|[<span data-ttu-id="1e775-188">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="1e775-188">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="1e775-189">アプリの発行の状態。</span><span class="sxs-lookup"><span data-stu-id="1e775-189">The publishing state for the app.</span></span> <span data-ttu-id="1e775-190">アプリが発行されていない限り、アプリを割り当てることができません。</span><span class="sxs-lookup"><span data-stu-id="1e775-190">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="1e775-191">[mobileApp](../resources/intune-apps-mobileapp.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="1e775-191">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="1e775-192">使用可能な値は、`notPublished`、`processing`、`published` です。</span><span class="sxs-lookup"><span data-stu-id="1e775-192">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="1e775-193">isAssigned</span><span class="sxs-lookup"><span data-stu-id="1e775-193">isAssigned</span></span>|<span data-ttu-id="1e775-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e775-194">Boolean</span></span>|<span data-ttu-id="1e775-195">アプリが少なくとも1つのグループに割り当てられているかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="1e775-195">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="1e775-196">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-196">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-197">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1e775-197">roleScopeTagIds</span></span>|<span data-ttu-id="1e775-198">String collection</span><span class="sxs-lookup"><span data-stu-id="1e775-198">String collection</span></span>|<span data-ttu-id="1e775-199">このモバイルアプリの範囲タグ id のリスト。</span><span class="sxs-lookup"><span data-stu-id="1e775-199">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="1e775-200">[mobileApp](../resources/intune-apps-mobileapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-200">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="1e775-201">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="1e775-201">committedContentVersion</span></span>|<span data-ttu-id="1e775-202">String</span><span class="sxs-lookup"><span data-stu-id="1e775-202">String</span></span>|<span data-ttu-id="1e775-203">内部にコミットされたコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1e775-203">The internal committed content version.</span></span> <span data-ttu-id="1e775-204">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-204">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1e775-205">fileName</span><span class="sxs-lookup"><span data-stu-id="1e775-205">fileName</span></span>|<span data-ttu-id="1e775-206">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="1e775-206">String</span></span>|<span data-ttu-id="1e775-207">メインの LOB アプリケーションのファイル名。</span><span class="sxs-lookup"><span data-stu-id="1e775-207">The name of the main Lob application file.</span></span> <span data-ttu-id="1e775-208">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-208">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1e775-209">size</span><span class="sxs-lookup"><span data-stu-id="1e775-209">size</span></span>|<span data-ttu-id="1e775-210">Int64</span><span class="sxs-lookup"><span data-stu-id="1e775-210">Int64</span></span>|<span data-ttu-id="1e775-211">アップロードされたすべてのファイルを含む合計サイズ。</span><span class="sxs-lookup"><span data-stu-id="1e775-211">The total size, including all uploaded files.</span></span> <span data-ttu-id="1e775-212">[mobileLobApp](../resources/intune-apps-mobilelobapp.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1e775-212">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="1e775-213">commandLine</span><span class="sxs-lookup"><span data-stu-id="1e775-213">commandLine</span></span>|<span data-ttu-id="1e775-214">String</span><span class="sxs-lookup"><span data-stu-id="1e775-214">String</span></span>|<span data-ttu-id="1e775-215">コマンド ライン。</span><span class="sxs-lookup"><span data-stu-id="1e775-215">The command line.</span></span>|
|<span data-ttu-id="1e775-216">productCode</span><span class="sxs-lookup"><span data-stu-id="1e775-216">productCode</span></span>|<span data-ttu-id="1e775-217">String</span><span class="sxs-lookup"><span data-stu-id="1e775-217">String</span></span>|<span data-ttu-id="1e775-218">製品コード。</span><span class="sxs-lookup"><span data-stu-id="1e775-218">The product code.</span></span>|
|<span data-ttu-id="1e775-219">productVersion</span><span class="sxs-lookup"><span data-stu-id="1e775-219">productVersion</span></span>|<span data-ttu-id="1e775-220">String</span><span class="sxs-lookup"><span data-stu-id="1e775-220">String</span></span>|<span data-ttu-id="1e775-221">Windows Mobile MSI 基幹業務 (LoB) アプリの製品のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1e775-221">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="1e775-222">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="1e775-222">ignoreVersionDetection</span></span>|<span data-ttu-id="1e775-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e775-223">Boolean</span></span>|<span data-ttu-id="1e775-224">アプリをデバイスにインストールした後に、アプリのバージョンを使用してアプリを検出するかどうかを制御するブール値。</span><span class="sxs-lookup"><span data-stu-id="1e775-224">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="1e775-225">自己更新機能を使用する Windows Mobile MSI 基幹業務 (LoB) アプリの場合は、true に設定します。</span><span class="sxs-lookup"><span data-stu-id="1e775-225">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="1e775-226">identityVersion</span><span class="sxs-lookup"><span data-stu-id="1e775-226">identityVersion</span></span>|<span data-ttu-id="1e775-227">String</span><span class="sxs-lookup"><span data-stu-id="1e775-227">String</span></span>|<span data-ttu-id="1e775-228">ID のバージョン。</span><span class="sxs-lookup"><span data-stu-id="1e775-228">The identity version.</span></span>|
|<span data-ttu-id="1e775-229">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="1e775-229">useDeviceContext</span></span>|<span data-ttu-id="1e775-230">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1e775-230">Boolean</span></span>|<span data-ttu-id="1e775-231">デバイスコンテキストにデュアルモード MSI をインストールするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1e775-231">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="1e775-232">true の場合、すべてのユーザーに対してアプリがインストールされます。</span><span class="sxs-lookup"><span data-stu-id="1e775-232">If true, app will be installed for all users.</span></span> <span data-ttu-id="1e775-233">false の場合、アプリはユーザーごとにインストールされます。</span><span class="sxs-lookup"><span data-stu-id="1e775-233">If false, app will be installed per-user.</span></span> <span data-ttu-id="1e775-234">null の場合、サービスは MSI パッケージの既定のインストールコンテキストを使用します。</span><span class="sxs-lookup"><span data-stu-id="1e775-234">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="1e775-235">デュアルモード MSI の場合、この既定値はユーザーごとになります。</span><span class="sxs-lookup"><span data-stu-id="1e775-235">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="1e775-236">デュアルモード以外のアプリには設定できません。</span><span class="sxs-lookup"><span data-stu-id="1e775-236">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="1e775-237">アプリケーションを最初に作成した後に変更することはできません。</span><span class="sxs-lookup"><span data-stu-id="1e775-237">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="1e775-238">応答</span><span class="sxs-lookup"><span data-stu-id="1e775-238">Response</span></span>
<span data-ttu-id="1e775-239">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1e775-239">If successful, this method returns a `201 Created` response code and a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e775-240">例</span><span class="sxs-lookup"><span data-stu-id="1e775-240">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e775-241">要求</span><span class="sxs-lookup"><span data-stu-id="1e775-241">Request</span></span>
<span data-ttu-id="1e775-242">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e775-242">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e775-243">応答</span><span class="sxs-lookup"><span data-stu-id="1e775-243">Response</span></span>
<span data-ttu-id="1e775-p123">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e775-p123">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




