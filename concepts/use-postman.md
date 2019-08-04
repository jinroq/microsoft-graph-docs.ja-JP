---
title: Microsoft Graph API で Postman を使用する
description: Microsoft Graph Postman のコレクションを使用して、Microsoft Graph API をすぐに開始できます。
author: ''
localization_priority: Priority
ms.openlocfilehash: 2140dec07328b75f7b1729cd3e7cf7c86e65f738
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038186"
---
# <a name="use-postman-with-the-microsoft-graph-api"></a><span data-ttu-id="8dbb7-103">Microsoft Graph API で Postman を使用する</span><span class="sxs-lookup"><span data-stu-id="8dbb7-103">Use the Microsoft Graph API</span></span>

<span data-ttu-id="8dbb7-104">Microsoft Graph Postman のコレクションを使用して、Microsoft Graph API をすぐに開始できます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-104">You can use the Microsoft Graph Postman collection to get started with Microsoft Graph APIs in minutes.</span></span>

![Postman の画像](https://github.com/microsoftgraph/microsoftgraph-postman-collections/blob/master/images/postman.png?raw=true)

<span data-ttu-id="8dbb7-106">この記事では、Postman と Microsoft Graph の使用方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-106">This article explains how to get up and running with Postman and Microsoft Graph.</span></span> <span data-ttu-id="8dbb7-107">
  [Graph Explorer](https://developer.microsoft.com/ja-JP/graph/graph-explorer) を使用して、web ブラウザーで直接 Microsoft Graph API を検索することもできます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-107">You can also explore Microsoft Graph APIs directly in your web browser by using [Graph Explorer](https://developer.microsoft.com/en-us/graph/graph-explorer).</span></span>

## <a name="accessing-the-collection"></a><span data-ttu-id="8dbb7-108">コレクションへのアクセス</span><span class="sxs-lookup"><span data-stu-id="8dbb7-108">Accessing the collection</span></span>
<span data-ttu-id="8dbb7-109">Postman のコレクションにアクセスするには、2 つの方法があります。使用する方法、付与する方法です。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-109">You can access the collection in Postman in two ways: by consuming it or by contributing to it.</span></span> <span data-ttu-id="8dbb7-110">最初にコンピューターで [Postman](https://www.getpostman.com/) を実行している必要があります。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-110">You will need to have [Postman](https://www.getpostman.com/) running on your computer first.</span></span>

### <a name="consume-the-collection"></a><span data-ttu-id="8dbb7-111">コレクションを使用する</span><span class="sxs-lookup"><span data-stu-id="8dbb7-111">Consume the collection</span></span>
<span data-ttu-id="8dbb7-112">Microsoft Graph API の使用を開始するには、コレクションを使用するのが最も簡単な方法です。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-112">Consuming the collection is the easiest way to get started with Microsoft Graph APIs.</span></span> <span data-ttu-id="8dbb7-113">[Postman 共有リンク](https://www.getpostman.com/collections/d89a737b5f0c0825898a) によって Postman が起動します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-113">The [Postman sharing link](https://www.getpostman.com/collections/d89a737b5f0c0825898a) will launch Postman.</span></span>

<span data-ttu-id="8dbb7-114">共有コレクションを使用する利点は、追加の作業をすることなく、新しい要求が自動的に表示されることです。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-114">The advantage to using the shared collection is that new requests will automatically show for you without any additional steps.</span></span>

<span data-ttu-id="8dbb7-115">コレクションを取得したら、環境変数をセットアップする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-115">After you have the collection, you'll need to set up the environment variables:</span></span>

1. <span data-ttu-id="8dbb7-116">**[ファイル | インポート ...]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-116">Choose **File | Import ...**.</span></span>
2. <span data-ttu-id="8dbb7-117">**[URL からインポートする]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-117">Select **Import From Link**.</span></span>
3. <span data-ttu-id="8dbb7-118">次の URL をコピーして貼り付け、**[インポート]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-118">Copy and paste the following URL and choose **Import**.</span></span>
 
    ```
    https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json
    ```

<span data-ttu-id="8dbb7-119">右上のドロップダウンに目のアイコンで **Microsoft Graph 環境** が表示されます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-119">You should now see the **Microsoft Graph environment** in the top right environment drop down by the eye icon.</span></span> <span data-ttu-id="8dbb7-120">次に、[環境の設定](#using-the-collection)をする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-120">Now you need to set up your workflow.</span></span>

### <a name="contribute-to-the-collection"></a><span data-ttu-id="8dbb7-121">コレクションに付与する</span><span class="sxs-lookup"><span data-stu-id="8dbb7-121">Contribute to the collection</span></span>
<span data-ttu-id="8dbb7-122">独自の要求を付与する場合は、[Microsoft Graph Postman コレクション](https://github.com/microsoftgraph/microsoftgraph-postman-collections)の github リポジトリにフォークする必要があります。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-122">If you want to contribute your own requests, you will need to fork the [Microsoft Graph Postman collections](https://github.com/microsoftgraph/microsoftgraph-postman-collections) github repo.</span></span> 

<span data-ttu-id="8dbb7-123">詳細については、次のビデオをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-123">For details about how to do this, watch the following video.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/4tg-OBdv_8o]

<span data-ttu-id="8dbb7-124">Postman コレクションをインポートするには:</span><span class="sxs-lookup"><span data-stu-id="8dbb7-124">To import the Postman collections:</span></span>

1. <span data-ttu-id="8dbb7-125">[Postman](https://www.getpostman.com/) をダウンロードして登録します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-125">Download and register for [Postman](https://www.getpostman.com/).</span></span>
2. <span data-ttu-id="8dbb7-126">**[ファイル | インポート ...]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-126">Choose **File | Import ...**.</span></span>
3. <span data-ttu-id="8dbb7-127">**[URL からインポートする]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-127">Select **Import From Link**.</span></span>
4. <span data-ttu-id="8dbb7-128">次の 2 つの URL を貼り付けて **[インポート]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-128">Paste the following two URLs and choose **Import** after each.</span></span>

    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_collection.json
      
    ```
    ```
      https://raw.githubusercontent.com/microsoftgraph/microsoftgraph-postman-collections/master/Microsoft%20Graph%20v1.0.postman_environment.json

    ```

<span data-ttu-id="8dbb7-129">**[コレクション]** ウィンドウに **Microsoft Graph v1.0** コレクションが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-129">You should now see the **Microsoft Graph v1.0** collection on the **Collections** pane.</span></span>

## <a name="using-the-collection"></a><span data-ttu-id="8dbb7-130">コレクションの使用</span><span class="sxs-lookup"><span data-stu-id="8dbb7-130">Using the collection</span></span>
<span data-ttu-id="8dbb7-131">Postman に **Microsoft Graph v1.0** コレクションと **Microsoftr Graph 環境** を取得したら、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-131">After you have the **Microsoft Graph v1.0** collection and the **Microsoftr Graph environment** in Postman, follow these steps.</span></span>

### <a name="set-up-application-api-calls"></a><span data-ttu-id="8dbb7-132">アプリケーション API の呼び出しを設定する</span><span class="sxs-lookup"><span data-stu-id="8dbb7-132">Set up application API calls</span></span>

1. <span data-ttu-id="8dbb7-133">右上隅の **[環境なし]** ドロップダウンを選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-133">Choose the **No environment** drop down in top right corner.</span></span>
2. <span data-ttu-id="8dbb7-134">**[Microsoft Graph 環境]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-134">Select **Microsoft Graph environment**.</span></span>
3. <span data-ttu-id="8dbb7-135">右の **目**のアイコンを選択し、**[編集]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-135">Choose the **eye** icon to the right and then choose **Edit**.</span></span>
4. <span data-ttu-id="8dbb7-136">**カレント** (非**初期**) 変数で Microsoft ID アプリケーションを入力します: **ClientID**、**ClientSecret**、**TenantID**。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-136">Enter your Microsoft Identity Application in the **current** (not **initial**) variables: **ClientID**, **ClientSecret** and **TenantID**.</span></span> 
 <span data-ttu-id="8dbb7-137">アプリケーションの作成方法、およびアプリのみのフローの管理方法の詳細については、[Postman を使用して Microsoft Graph を呼び出す](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) ブログの投稿を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-137">For more information about how to create an application and to admin consent the app-only flow, see the [Use Postman to make Microsoft Graph calls](https://developer.microsoft.com/en-us/graph/blogs/30daysmsgraph-day-13-postman-to-make-microsoft-graph-calls/) blog post.</span></span>

5. <span data-ttu-id="8dbb7-138">**[更新]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-138">Select **Update info**.</span></span> <span data-ttu-id="8dbb7-139">**[環境の管理]** ダイアログボックスを閉じます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-139">Close the **Manage Environments** dialog box.</span></span> <span data-ttu-id="8dbb7-140">**MicrosoftGraph v1.0 | アプリケーション** コレクションの左側の、**[アプリ専用アクセス トークンの取得]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-140">In the **MicrosoftGraph v1.0 | Application** collection on left side, choose **Get App-only Access Token**.</span></span> <span data-ttu-id="8dbb7-141">右側の **[送信]** を選びます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-141">Then choose **Send** on the right.</span></span>
6. <span data-ttu-id="8dbb7-142">**アプリケーション | ユーザー** フォルダーを展開し、**[ユーザーの取得]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-142">Expand the **Application | Users** folder and choose **Get Users**.</span></span> <span data-ttu-id="8dbb7-143">次に **[送信]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-143">Then choose **Send**.</span></span>

<span data-ttu-id="8dbb7-144">Microsoft Graph v 1.0 コレクションを使用する準備ができました。。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-144">You are now up and running with the Microsoft Graph v1.0 collections.</span></span>

><span data-ttu-id="8dbb7-145">**Note:** コレクション内の他の API を実行する場合は、アプリケーションに必要なアクセス許可に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-145">**Note:** If you want to run other APIs in the collection, you will need to consent the required permissions for your application.</span></span>

### <a name="set-up-on-behalf-of-api-calls"></a><span data-ttu-id="8dbb7-146">代理として API 呼び出しを設定する</span><span class="sxs-lookup"><span data-stu-id="8dbb7-146">Set up on-behalf-of API calls</span></span>
<span data-ttu-id="8dbb7-147">代理として API 呼び出しを設定するには、環境設定で、**ユーザー名** と **ユーザー パスワード** を設定し、\*\*ユーザーの代理 | ユーザーのアクセス トークンを取得 \*\* を使用します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-147">The simplest way to set up on-behalf-of API calls is to provide a **UserName** and **UserPassword** in the environment settings and use the **On Behalf of a User | Get User Access Token**.</span></span> 

><span data-ttu-id="8dbb7-148">**重要:** この情報は Postman に直接格納されるため、実稼働ユーザーアカウントを使用することはお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-148">**Important:** We don't recommend using production user accounts because this information is stored directly in Postman.</span></span> <span data-ttu-id="8dbb7-149">また、この方法を使用して、運用環境でアクセス トークンを取得することもお勧めしません。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-149">We also don't  recommend using this approach to obtain access tokens in production.</span></span> <span data-ttu-id="8dbb7-150">テスト目的にのみ使用ください。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-150">Use it only for testing purposes.</span></span>

<span data-ttu-id="8dbb7-151">ユーザー名とパスワードを Postman cloud アカウントに同期する環境変数に格納しない場合は、**[新しいアクセス トークンの取得]** 機能を使用して、Postman を終了せずにトークンを取得できます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-151">If you don't want to store user names and passwords in environment variables that sync to your Postman cloud account, you can use the  **Get New Access Token** capability to get a token without leaving Postman.</span></span>

1. <span data-ttu-id="8dbb7-152">\*\*ユーザーの代理 | Postman を使用してアクセス トークンを取得する \*\* を選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-152">Select **On behalf of a User | Get Access Token using Postman**.</span></span>
2. <span data-ttu-id="8dbb7-153">**[承認]** タブを選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-153">Choose the Authorization tab in the Request Editor.</span></span>
3. <span data-ttu-id="8dbb7-154">**[アクセス トークンを取得する]** ボタン選択します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-154">Choose the **get access token** button.</span></span>
4. <span data-ttu-id="8dbb7-155">実際のテナントとアプリケーションの値を、次のボックスに入力します。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-155">Fill out the following boxes with your real tenant and application values.</span></span> <span data-ttu-id="8dbb7-156">ここでは環境変数を使用できません。実際の値を使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-156">Note that you cannot use the environment variables here; you have to use the actual values.</span></span> <span data-ttu-id="8dbb7-157">Portal.azure.com のアプリケーションブレードで **EndPoints** を選ぶと、値を見つけることができます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-157">You can find them by selecting **EndPoints** in the application blade in portal.azure.com.</span></span>

    - <span data-ttu-id="8dbb7-158">コールバック URL: https://app.getpostman.com/oauth2/callback</span><span class="sxs-lookup"><span data-stu-id="8dbb7-158">Callback URL: https://app.getpostman.com/oauth2/callback</span></span>
    - <span data-ttu-id="8dbb7-159">認証 URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span><span class="sxs-lookup"><span data-stu-id="8dbb7-159">Auth URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/authorize</span></span>
    - <span data-ttu-id="8dbb7-160">アクセス トークン URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span><span class="sxs-lookup"><span data-stu-id="8dbb7-160">Access Token URL: https://login.microsoftonline.com/**TENANTID**/oauth2/v2.0/token</span></span>
    - <span data-ttu-id="8dbb7-161">クライアント ID: **CLIENTID**</span><span class="sxs-lookup"><span data-stu-id="8dbb7-161">Client ID: **CLIENTID**</span></span>
    - <span data-ttu-id="8dbb7-162">クライアントシークレット: **CLIENTSECRET**</span><span class="sxs-lookup"><span data-stu-id="8dbb7-162">Client Secret: **CLIENTSECRET**</span></span>
    - <span data-ttu-id="8dbb7-163">スコープ: https://graph.microsoft.com/.default</span><span class="sxs-lookup"><span data-stu-id="8dbb7-163">scopehttps://graph.microsoft.com/.default</span></span>
    - <span data-ttu-id="8dbb7-164">状態: **RANDOMSTRING**</span><span class="sxs-lookup"><span data-stu-id="8dbb7-164">State: **RANDOMSTRING**</span></span>
 
5. <span data-ttu-id="8dbb7-165">**トークンを要求する**を選択する。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-165">Choose **Request Token**.</span></span> <span data-ttu-id="8dbb7-166">サインインと同意の許可を求める UI プロンプトが表示されます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-166">You should see a UI prompt to sign in and consent permissions.</span></span>
6. <span data-ttu-id="8dbb7-167">アクセス トークンをコピーし、環境変数を開いて、 **UserAccessToken** フィールドに貼り付けます。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-167">Copy the access token, open your environment variables, and paste it into the **UserAccessToken** field.</span></span>

<span data-ttu-id="8dbb7-168">すべての依頼が機能するようになりました。</span><span class="sxs-lookup"><span data-stu-id="8dbb7-168">Now all your requests will work.</span></span>
