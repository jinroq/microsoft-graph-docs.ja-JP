---
title: Microsoft Graph の OneNote API のエラー コード
description: この記事では、API を通して送信した要求が失敗した場合に、Microsoft Graph の OneNote API から返されるエラー コードについて説明します。
author: Jewan-microsoft
ms.openlocfilehash: 9c715b25e9b3114d6db21a3b935a266123ca0601
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352466"
---
# <a name="error-codes-for-onenote-apis-in-microsoft-graph"></a><span data-ttu-id="9ef23-103">Microsoft Graph の OneNote API のエラー コード</span><span class="sxs-lookup"><span data-stu-id="9ef23-103">Error codes for OneNote APIs in Microsoft Graph</span></span>

<span data-ttu-id="9ef23-104">この記事では、API を通して送信した要求が失敗した場合に、Microsoft Graph の OneNote API から返されるエラー コードについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-104">This article describes error codes that are returned by the OneNote APIs in Microsoft Graph whenever a request sent through the API fails.</span></span>

## <a name="error-response-example"></a><span data-ttu-id="9ef23-105">エラー応答例</span><span class="sxs-lookup"><span data-stu-id="9ef23-105">Error response example</span></span>

<span data-ttu-id="9ef23-p101">送信した要求でエラーが発生すると、OneNote API はその要求の実行を停止し、エラー応答を JSON オブジェクトとして返します。エラー応答には、関連付けられているエラー コード、メッセージ、およびこの記事の該当するセクションへのリンクが含まれます。次の例は、エラー応答の様子を示しています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p101">When your request generates an error, the OneNote API stops performing the request and returns an error response as a JSON object. An error response contains the associated error code, a message, and a link to the appropriate section of this article. The following example shows how an error response looks.</span></span>

```json
{
   "error":{
      "code":"10002",
      "message":"The service is currently unavailable. Please try again later.",
      "innerError": {
        "requestId": "request-id",
        "date": "date-time"
      }
   }
}
```

<span data-ttu-id="9ef23-109">Microsoft Graph エラーの詳細については、「[Microsoft Graph エラー応答およびリソースの種類](errors.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-109">For more information about Microsoft Graph errors, see [Microsoft Graph error responses and resource types](errors.md).</span></span>

## <a name="codes-from-10001-to-19999"></a><span data-ttu-id="9ef23-110">10001 から 19999 のコード</span><span class="sxs-lookup"><span data-stu-id="9ef23-110">Codes from 10001 to 19999</span></span>

<span data-ttu-id="9ef23-111">サービスで問題が発生したか、サービスからアプリケーションに情報が送られました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-111">The service is having problems or is sending information to the application.</span></span>

### <a name="10001"></a><span data-ttu-id="9ef23-112">10001</span><span class="sxs-lookup"><span data-stu-id="9ef23-112">10001</span></span>
<span data-ttu-id="9ef23-113">予期しないエラーが発生し、要求が失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-113">An unexpected error occurred and the request failed.</span></span>

### <a name="10002"></a><span data-ttu-id="9ef23-114">10002</span><span class="sxs-lookup"><span data-stu-id="9ef23-114">10002</span></span>
<span data-ttu-id="9ef23-115">サービスは現在利用できません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-115">The service is not currently available.</span></span>

### <a name="10003"></a><span data-ttu-id="9ef23-116">10003</span><span class="sxs-lookup"><span data-stu-id="9ef23-116">10003</span></span>
<span data-ttu-id="9ef23-p102">現在のユーザーのアカウントで、アクティブな要求の最大数を超えました。アプリは要求を繰り返す必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p102">The current user's account has exceeded the maximum number of active requests. Your app will have to repeat the request.</span></span>

### <a name="10004"></a><span data-ttu-id="9ef23-119">10004</span><span class="sxs-lookup"><span data-stu-id="9ef23-119">10004</span></span>
<span data-ttu-id="9ef23-120">サービスは要求されたセクション内にページを作成できません。そのセクションはパスワードで保護されています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-120">The service can't create a page in the requested section because that section is protected by a password.</span></span>

### <a name="10005"></a><span data-ttu-id="9ef23-121">10005</span><span class="sxs-lookup"><span data-stu-id="9ef23-121">10005</span></span>
<span data-ttu-id="9ef23-p103">要求内で、**data-render-src** 属性に PDF が含まれる イメージ タグが最大数を超えました。詳細については、「[イメージおよびファイルの追加](onenote-images-files.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p103">The request contains more than the maximum number of image tags in which the **data-render-src** attribute contains a PDF. See [Add images and files](onenote-images-files.md).</span></span>

### <a name="10006"></a><span data-ttu-id="9ef23-124">10006</span><span class="sxs-lookup"><span data-stu-id="9ef23-124">10006</span></span>
<span data-ttu-id="9ef23-125">OneNote API は、指定されたセクション内にページを作成できませんでした。そのセクションは破損しています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-125">The OneNote API was unable to create a page in the specified section because that section is corrupt.</span></span>

### <a name="10007"></a><span data-ttu-id="9ef23-126">10007</span><span class="sxs-lookup"><span data-stu-id="9ef23-126">10007</span></span>
<span data-ttu-id="9ef23-p104">現在、サーバーがビジー状態であるため、受信した要求を処理できません。後でもう一度やり直してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p104">The server is too busy to handle the incoming request at this moment. Please try again later.</span></span>

### <a name="10008"></a><span data-ttu-id="9ef23-129">10008</span><span class="sxs-lookup"><span data-stu-id="9ef23-129">10008</span></span>
<span data-ttu-id="9ef23-130">ユーザーまたはグループの OneDrive にある 1 つ以上のドキュメント ライブラリに 5000 を超える OneNote のアイテム (ノートブック、セクション、セクション グループ) が含まれており、API を使用してクエリを実行することができません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-130">One or more of the document libraries on the user or group's OneDrive contains more than 5000 OneNote items (notebooks, sections, section groups), and cannot be queried using the API.</span></span> <span data-ttu-id="9ef23-131">ユーザーまたはグループのどのドキュメント ライブラリについても、その中の OneNote アイテム数が 5000 を超えることがないようにしてください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-131">Please make sure that none of the user or group's document libraries contains more than 5000 OneNote items.</span></span> <span data-ttu-id="9ef23-132">軽減の手順については「[OneNote 開発者ブログ](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-132">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10012"></a><span data-ttu-id="9ef23-133">10012</span><span class="sxs-lookup"><span data-stu-id="9ef23-133">10012</span></span>
<span data-ttu-id="9ef23-134">エンティティを作成または更新できません。ノートブックが含まれるライブラリの場合、アイテムを編集する前にチェックアウトする必要があるためです。</span><span class="sxs-lookup"><span data-stu-id="9ef23-134">Unable to create or update the entity because the library that contains the notebook requires items to be checked out before they can be edited.</span></span> <span data-ttu-id="9ef23-135">詳細については、「[ファイルのチェックアウトを必須にするようにライブラリを設定する](https://support.office.com/ja-JP/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-135">For more information, see [Set up a library to require check-out of files](https://support.office.com/ja-JP/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7).</span></span>

<span data-ttu-id="9ef23-136">ライブラリからチェックアウト要件を削除するか、ノートブックを移動します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-136">Either remove the check-out requirement from the library, or move the notebook.</span></span>

### <a name="10013"></a><span data-ttu-id="9ef23-137">10013</span><span class="sxs-lookup"><span data-stu-id="9ef23-137">10013</span></span>
<span data-ttu-id="9ef23-138">ユーザーまたはグループの OneDrive にある 1 つ以上のドキュメント ライブラリに 20,000 を超えるアイテムが含まれており、API を使用してクエリ用にインデックス付けをすることができません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-138">One or more of the document libraries on the user or group's OneDrive contains more than 20,000 items and cannot be indexed for querying using the API.</span></span> <span data-ttu-id="9ef23-139">ユーザーまたはグループのどのドキュメント ライブラリについても、その中のアイテム数が 20,000 を超えることがないようにしてください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-139">Please make sure that none of the user or group's document libraries contains more than 20,000 items.</span></span> <span data-ttu-id="9ef23-140">軽減の手順については「[OneNote 開発者ブログ](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-140">See the [OneNote Dev blog](https://blogs.msdn.microsoft.com/onenotedev/2016/09/11/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library/) for mitigation steps.</span></span>

### <a name="10014"></a><span data-ttu-id="9ef23-141">10014</span><span class="sxs-lookup"><span data-stu-id="9ef23-141">10014</span></span>
<span data-ttu-id="9ef23-142">現在、Azure Key Vault がビジー状態であるため、受信した要求を処理できません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-142">Azure Key Vault is too busy to handle the incoming request at this moment.</span></span> <span data-ttu-id="9ef23-143">後でもう一度お試しください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-143">Please try again later.</span></span>

### <a name="10015"></a><span data-ttu-id="9ef23-144">10015</span><span class="sxs-lookup"><span data-stu-id="9ef23-144">10015</span></span>
<span data-ttu-id="9ef23-145">SharePoint は現在利用できません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-145">SharePoint is currently unavailable.</span></span> <span data-ttu-id="9ef23-146">後でもう一度お試しください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-146">Please try again later.</span></span>

### <a name="10016"></a><span data-ttu-id="9ef23-147">10016</span><span class="sxs-lookup"><span data-stu-id="9ef23-147">10016</span></span>
<span data-ttu-id="9ef23-148">ユーザーまたはグループの OneDrive 上のドキュメント ライブラリで、固有のセキュリティ スコープのしきい値の制限を超えました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-148">Document library on the user or group’s OneDrive exceeded unique security scopes threshold limit.</span></span> <span data-ttu-id="9ef23-149">ライブラリに設定する固有のセキュリティ スコープの最大数が、50,000 個を超えることはできません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-149">The maximum number of unique security scopes set for a library cannot exceed 50,000.</span></span>

### <a name="10017"></a><span data-ttu-id="9ef23-150">10017</span><span class="sxs-lookup"><span data-stu-id="9ef23-150">10017</span></span>
<span data-ttu-id="9ef23-151">要求が正しくありません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-151">Bad Request.</span></span>

### <a name="19999"></a><span data-ttu-id="9ef23-152">19999</span><span class="sxs-lookup"><span data-stu-id="9ef23-152">19999</span></span>
<span data-ttu-id="9ef23-153">未定義のエラーが発生したため、要求は失敗しました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-153">The request failed because an undetermined error occurred.</span></span>

## <a name="codes-from-20001-to-29999"></a><span data-ttu-id="9ef23-154">20001 から 29999 のコード</span><span class="sxs-lookup"><span data-stu-id="9ef23-154">Codes from 20001 to 29999</span></span>

<span data-ttu-id="9ef23-155">アプリケーション コードが間違った処理を実行しました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-155">The application code has done something wrong.</span></span>

### <a name="20001"></a><span data-ttu-id="9ef23-156">20001</span><span class="sxs-lookup"><span data-stu-id="9ef23-156">20001</span></span>

<span data-ttu-id="9ef23-157">要求に必須の "Presentation" パートがありません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-157">The request is missing the required "Presentation" part.</span></span> <span data-ttu-id="9ef23-158">1 つだけ必要です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-158">Exactly one is required.</span></span> 

### <a name="20002"></a><span data-ttu-id="9ef23-159">20002</span><span class="sxs-lookup"><span data-stu-id="9ef23-159">20002</span></span>
<span data-ttu-id="9ef23-160">要求に "Presentation" パートが 2 つ以上あります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-160">The request contains two or more "Presentation" parts.</span></span> <span data-ttu-id="9ef23-161">1 つだけ必要です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-161">Exactly one is required.</span></span>

### <a name="20003"></a><span data-ttu-id="9ef23-162">20003</span><span class="sxs-lookup"><span data-stu-id="9ef23-162">20003</span></span>
<span data-ttu-id="9ef23-163">"Presentation" パートのコンテンツ タイプは、text/HTML または application/XHTML+XML のいずれかでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-163">The content type of the "Presentation" part can be only text/HTML or application/XHTML+XML.</span></span> 

### <a name="20004"></a><span data-ttu-id="9ef23-164">20004</span><span class="sxs-lookup"><span data-stu-id="9ef23-164">20004</span></span>
<span data-ttu-id="9ef23-165">"Presentation" パートの HTML に、**src** プロパティと **data-render-src** プロパティの両方が設定されている画像タグが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-165">The "Presentation" part HTML contains an image tag with both the **src** and the **data-render-src** properties set.</span></span> <span data-ttu-id="9ef23-166">API は **src** プロパティを無視し、**data-render-src** プロパティを使用します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-166">The API will ignore the **src** property and use the **data-render-src** property.</span></span> 

### <a name="20005"></a><span data-ttu-id="9ef23-167">20005</span><span class="sxs-lookup"><span data-stu-id="9ef23-167">20005</span></span>
<span data-ttu-id="9ef23-p114">要求 URI が長すぎます。URI の最大サイズ (すべてのパラメーターとデータを含む) は 16 KB (16,384 文字) です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p114">The request URI is too long. The maximum size of the URI (including all parameters and data) is 16 KB or 16,384 characters.</span></span>

### <a name="20006"></a><span data-ttu-id="9ef23-170">20006</span><span class="sxs-lookup"><span data-stu-id="9ef23-170">20006</span></span>
<span data-ttu-id="9ef23-171">"Presentation" パートの HTML に、src プロパティと **data-render-src** プロパティのいずれかが設定されている画像タグが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-171">The "Presentation" part HTML contains an image tag with neither the src nor the **data-render-src** properties set.</span></span> <span data-ttu-id="9ef23-172">API は **image** タグを無視します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-172">The API will ignore the **image** tag.</span></span> 

### <a name="20007"></a><span data-ttu-id="9ef23-173">20007</span><span class="sxs-lookup"><span data-stu-id="9ef23-173">20007</span></span>
<span data-ttu-id="9ef23-174">"Presentation" パートの HTML に含まれる作成日時の文字列が、許可される形式のいずれとも一致しません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-174">The "Presentation" part HTML contains a created date/time string that does not match any of the allowed formats.</span></span> 

### <a name="20008"></a><span data-ttu-id="9ef23-175">20008</span><span class="sxs-lookup"><span data-stu-id="9ef23-175">20008</span></span>
<span data-ttu-id="9ef23-176">要求のサイズが大きすぎます。</span><span class="sxs-lookup"><span data-stu-id="9ef23-176">The size of the request is too large.</span></span> 

### <a name="20009"></a><span data-ttu-id="9ef23-177">20009</span><span class="sxs-lookup"><span data-stu-id="9ef23-177">20009</span></span>
<span data-ttu-id="9ef23-178">要求のパートに名前が重複しているものがあります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-178">The request contains parts with duplicate names.</span></span> <span data-ttu-id="9ef23-179">パートの名前は一意にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-179">Part names must be unique.</span></span> 

### <a name="20010"></a><span data-ttu-id="9ef23-180">20010</span><span class="sxs-lookup"><span data-stu-id="9ef23-180">20010</span></span>
<span data-ttu-id="9ef23-181">指定のコンテンツ タイプには Content-Disposition ヘッダーが指定されていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-181">The Content-Disposition header was not supplied for the specified content type.</span></span> 

### <a name="20011"></a><span data-ttu-id="9ef23-182">20011</span><span class="sxs-lookup"><span data-stu-id="9ef23-182">20011</span></span>
<span data-ttu-id="9ef23-183">要求にはマルチパート ペイロードが含まれていますが、その形式が不正です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-183">The request contains a malformed multipart payload.</span></span> <span data-ttu-id="9ef23-184">空白行がない、最後の行がない、パートの区切りの書式が正しくないなどの問題が考えられます。</span><span class="sxs-lookup"><span data-stu-id="9ef23-184">Problems could include missing blank lines, a missing last line, incorrectly formatted part separators, and so on.</span></span> <span data-ttu-id="9ef23-185">マルチパート メッセージを手動で作成する場合、ロジックを注意深く確認するか、サードパーティ ライブラリの使用をご検討ください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-185">If you're building the multipart message by hand, carefully check the logic, or consider using a third-party library.</span></span> 

### <a name="20012"></a><span data-ttu-id="9ef23-186">20012</span><span class="sxs-lookup"><span data-stu-id="9ef23-186">20012</span></span>
<span data-ttu-id="9ef23-187">この要求は、指定のパートにコンテンツ タイプを指定しません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-187">The request doesn't supply a content type for the specified part.</span></span> 

### <a name="20013"></a><span data-ttu-id="9ef23-188">20013</span><span class="sxs-lookup"><span data-stu-id="9ef23-188">20013</span></span>
<span data-ttu-id="9ef23-189">要求の中で、指定したパートの Content-Type ヘッダーおよび Content-Disposition ヘッダーが提供されていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-189">The request doesn't supply Content-Type and Content-Disposition headers for the specified part.</span></span> 

### <a name="20014"></a><span data-ttu-id="9ef23-190">20014</span><span class="sxs-lookup"><span data-stu-id="9ef23-190">20014</span></span>
<span data-ttu-id="9ef23-191">マルチパート メッセージのパートの長さが最大サイズである 25 MB を超えています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-191">The length of a part in the multipart message exceeds the maximum size of 25 MB.</span></span> 

### <a name="20015"></a><span data-ttu-id="9ef23-192">20015</span><span class="sxs-lookup"><span data-stu-id="9ef23-192">20015</span></span>
<span data-ttu-id="9ef23-193">マルチパート メッセージのパート数が上限の 500 を超えています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-193">The count of parts in the multipart message exceeds the limit of 500.</span></span> 

### <a name="20016"></a><span data-ttu-id="9ef23-194">20016</span><span class="sxs-lookup"><span data-stu-id="9ef23-194">20016</span></span>
<span data-ttu-id="9ef23-195">マルチパート メッセージの長さが上限の 75 MB を超えています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-195">The length of the multipart message exceeds the limit of 75 MB.</span></span> 

### <a name="20017"></a><span data-ttu-id="9ef23-196">20017</span><span class="sxs-lookup"><span data-stu-id="9ef23-196">20017</span></span>
<span data-ttu-id="9ef23-197">電子メールの MIME の形式が正しくありませんでした。</span><span class="sxs-lookup"><span data-stu-id="9ef23-197">The email MIME was malformed.</span></span> 

### <a name="20018"></a><span data-ttu-id="9ef23-198">20018</span><span class="sxs-lookup"><span data-stu-id="9ef23-198">20018</span></span>
<span data-ttu-id="9ef23-199">会議の MIME または ICal の形式が正しくありませんでした。</span><span class="sxs-lookup"><span data-stu-id="9ef23-199">The meeting MIME or ICal was malformed.</span></span> 

### <a name="20019"></a><span data-ttu-id="9ef23-200">20019</span><span class="sxs-lookup"><span data-stu-id="9ef23-200">20019</span></span>
<span data-ttu-id="9ef23-201">ICal は見つかりませんでした。</span><span class="sxs-lookup"><span data-stu-id="9ef23-201">No ICal was found.</span></span> 

### <a name="20020"></a><span data-ttu-id="9ef23-202">20020</span><span class="sxs-lookup"><span data-stu-id="9ef23-202">20020</span></span>
<span data-ttu-id="9ef23-203">要求の本文に無効な形式の Json がありました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-203">Encountered malformed Json in request body.</span></span> 

### <a name="20100"></a><span data-ttu-id="9ef23-204">20100</span><span class="sxs-lookup"><span data-stu-id="9ef23-204">20100</span></span>
<span data-ttu-id="9ef23-205">要求の構文に誤りがあります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-205">Something is wrong with the syntax of your request.</span></span> 

### <a name="20101"></a><span data-ttu-id="9ef23-206">20101</span><span class="sxs-lookup"><span data-stu-id="9ef23-206">20101</span></span>
<span data-ttu-id="9ef23-207">要求したプロパティは存在しません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-207">The property that you requested doesn't exist.</span></span>

### <a name="20102"></a><span data-ttu-id="9ef23-208">20102</span><span class="sxs-lookup"><span data-stu-id="9ef23-208">20102</span></span>
<span data-ttu-id="9ef23-209">存在しないリソースが要求されました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-209">You requested a resource that doesn't exist.</span></span>

### <a name="20103"></a><span data-ttu-id="9ef23-210">20103</span><span class="sxs-lookup"><span data-stu-id="9ef23-210">20103</span></span>
<span data-ttu-id="9ef23-p118">**expand** クエリはこの要求ではサポートされません。「[サポートされている OData クエリ文字列オプション](onenote-get-content.md#supported-odata-query-string-options)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p118">The **expand** query is not supported for this request. See [Supported OData query string options](onenote-get-content.md#supported-odata-query-string-options).</span></span>

### <a name="20104"></a><span data-ttu-id="9ef23-213">20104</span><span class="sxs-lookup"><span data-stu-id="9ef23-213">20104</span></span>
<span data-ttu-id="9ef23-p119">**pagelevel** クエリ オプションは、セクションにあるページ コレクションまたは特定のページに対してクエリを行うときだけサポートされます。例:</span><span class="sxs-lookup"><span data-stu-id="9ef23-p119">The **pagelevel** query option is supported only when querying for the pages collection in a section or for a specific page. For example:</span></span>  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a><span data-ttu-id="9ef23-216">20106</span><span class="sxs-lookup"><span data-stu-id="9ef23-216">20106</span></span>
<span data-ttu-id="9ef23-217">要求に、サポートされていないクエリ演算子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-217">Your request contains a query operator that is not supported.</span></span> 

### <a name="20108"></a><span data-ttu-id="9ef23-218">20108</span><span class="sxs-lookup"><span data-stu-id="9ef23-218">20108</span></span>
<span data-ttu-id="9ef23-219">要求に、サポートされていない OData クエリ パラメーターが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-219">Your request contains unsupported OData query parameters.</span></span>

### <a name="20109"></a><span data-ttu-id="9ef23-220">20109</span><span class="sxs-lookup"><span data-stu-id="9ef23-220">20109</span></span>
<span data-ttu-id="9ef23-221">PATCH 要求内のペイロードの構成が正しくありません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-221">The payload in the PATCH request is not constructed correctly.</span></span>

### <a name="20110"></a><span data-ttu-id="9ef23-222">20110</span><span class="sxs-lookup"><span data-stu-id="9ef23-222">20110</span></span>
<span data-ttu-id="9ef23-223">データ パートを伴うページ作成要求では、コンテンツが "Presentation" パートを含むマルチパートである必要があります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-223">Page create requests with data parts require the content to be multipart, with a "Presentation" part.</span></span> 

### <a name="20111"></a><span data-ttu-id="9ef23-224">20111</span><span class="sxs-lookup"><span data-stu-id="9ef23-224">20111</span></span>
<span data-ttu-id="9ef23-225">要求で使用されている OData 機能はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-225">Your request uses an OData feature that isn't supported.</span></span>

### <a name="20112"></a><span data-ttu-id="9ef23-226">20112</span><span class="sxs-lookup"><span data-stu-id="9ef23-226">20112</span></span>
<span data-ttu-id="9ef23-227">ターゲット ノートブック、セクション グループ、セクション、またはページ エンティティの無効な ID が要求に含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-227">Your request contains an invalid ID for the target notebook, section group, section, or page entity.</span></span>

### <a name="20113"></a><span data-ttu-id="9ef23-228">20113</span><span class="sxs-lookup"><span data-stu-id="9ef23-228">20113</span></span>
<span data-ttu-id="9ef23-229">要求で指定されているリソースは削除されました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-229">The resource specified in the request has been deleted.</span></span>

### <a name="20115"></a><span data-ttu-id="9ef23-230">20115</span><span class="sxs-lookup"><span data-stu-id="9ef23-230">20115</span></span>
<span data-ttu-id="9ef23-231">名前に無効な文字が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-231">The name contains invalid characters.</span></span> <span data-ttu-id="9ef23-232">ノートブック名には次の文字を含めることはできません: `? * \ / : < > | ' "`</span><span class="sxs-lookup"><span data-stu-id="9ef23-232">A notebook name cannot contain any of the following characters: `? * \ / : < > | ' "`</span></span>

### <a name="20117"></a><span data-ttu-id="9ef23-233">20117</span><span class="sxs-lookup"><span data-stu-id="9ef23-233">20117</span></span>
<span data-ttu-id="9ef23-234">指定された名前のアイテムは、指定された場所に既に存在します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-234">An item with the name you specified already exists in the location that you specified.</span></span>

### <a name="20119"></a><span data-ttu-id="9ef23-235">20119</span><span class="sxs-lookup"><span data-stu-id="9ef23-235">20119</span></span>
<span data-ttu-id="9ef23-236">"Presentation" パートの HTML に含まれる **data-attachment** 属性の形式が無効であるか、またはファイル名には無効な文字 (`\ / : * ? < > | "`) が 1 つ以上含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-236">The HTML in the "Presentation" part contains a **data-attachment** attribute that either doesn't have a valid format or includes one or more of these invalid characters for a file name: `\ / : * ? < > | "`.</span></span> <span data-ttu-id="9ef23-237">要求では、エラー メッセージに示されている値に置き換えられました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-237">The request substituted the value indicated in the error message.</span></span>

### <a name="20120"></a><span data-ttu-id="9ef23-238">20120</span><span class="sxs-lookup"><span data-stu-id="9ef23-238">20120</span></span>
<span data-ttu-id="9ef23-239">要求で指定された PATCH ターゲットが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-239">Your request specifies a PATCH target that can't be located.</span></span>

### <a name="20121"></a><span data-ttu-id="9ef23-240">20121</span><span class="sxs-lookup"><span data-stu-id="9ef23-240">20121</span></span>
<span data-ttu-id="9ef23-p122">要求に含まれている PATCH 引数が無効です。「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p122">Your request contains an invalid PATCH argument. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20122"></a><span data-ttu-id="9ef23-243">20122</span><span class="sxs-lookup"><span data-stu-id="9ef23-243">20122</span></span>
<span data-ttu-id="9ef23-p123">要求で指定されている PATCH action はサポートされていません。「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p123">Your request specifies an unsupported PATCH action. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20123"></a><span data-ttu-id="9ef23-246">20123</span><span class="sxs-lookup"><span data-stu-id="9ef23-246">20123</span></span>
<span data-ttu-id="9ef23-247">PATCH 要求は、指定されたページを変更できません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-247">The PATCH request is unable to alter the specified page.</span></span>

### <a name="20124"></a><span data-ttu-id="9ef23-248">20124</span><span class="sxs-lookup"><span data-stu-id="9ef23-248">20124</span></span>
<span data-ttu-id="9ef23-249">マルチパートの PATCH 要求に、PATCH アクションの JSON 構造を指定した "commands" パートが含まれていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-249">Your multipart PATCH request doesn't include a "commands" part with the PATCH action JSON structure.</span></span> <span data-ttu-id="9ef23-250">「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-250">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20125"></a><span data-ttu-id="9ef23-251">20125</span><span class="sxs-lookup"><span data-stu-id="9ef23-251">20125</span></span>
<span data-ttu-id="9ef23-p125">PATCH 要求に action が含まれていません。「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p125">Your PATCH request contains no actions. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20126"></a><span data-ttu-id="9ef23-254">20126</span><span class="sxs-lookup"><span data-stu-id="9ef23-254">20126</span></span>
<span data-ttu-id="9ef23-255">メッセージ本文に、不正な書式設定の JSON またはこの操作に対してはサポートされていないフィールドが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-255">The message body contains either incorrectly formatted JSON or fields that are not supported for this operation.</span></span>

### <a name="20127"></a><span data-ttu-id="9ef23-256">20127</span><span class="sxs-lookup"><span data-stu-id="9ef23-256">20127</span></span>
<span data-ttu-id="9ef23-257">要求で指定された名前は不明なプロパティです。</span><span class="sxs-lookup"><span data-stu-id="9ef23-257">Your request specifies the name of an unknown property.</span></span>

### <a name="20128"></a><span data-ttu-id="9ef23-258">20128</span><span class="sxs-lookup"><span data-stu-id="9ef23-258">20128</span></span>
<span data-ttu-id="9ef23-259">要求に含まれている OData で、メッセージに示されている位置に構文エラーがあります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-259">Your request contains an OData syntax error at the position indicated in the message.</span></span>

### <a name="20129"></a><span data-ttu-id="9ef23-260">20129</span><span class="sxs-lookup"><span data-stu-id="9ef23-260">20129</span></span>
<span data-ttu-id="9ef23-p126">要求に、値が大きすぎる**上位**のクエリ文字列オプションが含まれます。ページのクエリの場合、最大値は 100 で、既定値は 20 です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p126">Your request contains a **top** query string option whose value is too high. For page queries, the maximum value is 100, and the default value is 20.</span></span>

### <a name="20130"></a><span data-ttu-id="9ef23-263">20130</span><span class="sxs-lookup"><span data-stu-id="9ef23-263">20130</span></span>
<span data-ttu-id="9ef23-264">要求に含まれている URI が指している HTTP リソースが見つかりません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-264">Your request contains a URI that points to an HTTP resource that can't be found.</span></span>

### <a name="20131"></a><span data-ttu-id="9ef23-265">20131</span><span class="sxs-lookup"><span data-stu-id="9ef23-265">20131</span></span>
<span data-ttu-id="9ef23-266">要求に Content-Type の無効な値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-266">Your request contains an invalid value for Content-Type.</span></span> <span data-ttu-id="9ef23-267">メッセージに指定されている値を使用します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-267">Use the value indicated in the message.</span></span> 

### <a name="20132"></a><span data-ttu-id="9ef23-268">20132</span><span class="sxs-lookup"><span data-stu-id="9ef23-268">20132</span></span>
<span data-ttu-id="9ef23-269">要求に無効なコンテンツが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-269">Your request contains invalid content.</span></span> <span data-ttu-id="9ef23-270">このエラーのよくある原因は、Content-Type 要求ヘッダーの欠落や、要求の本文にコンテンツが含まれていないことです。</span><span class="sxs-lookup"><span data-stu-id="9ef23-270">Common causes for this are a missing Content-Type request header and/or no content in the body of the request.</span></span> 

### <a name="20133"></a><span data-ttu-id="9ef23-271">20133</span><span class="sxs-lookup"><span data-stu-id="9ef23-271">20133</span></span>
<span data-ttu-id="9ef23-272">要求で指定された PATCH ターゲットはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-272">Your request specifies a PATCH target that is not supported.</span></span> <span data-ttu-id="9ef23-273">「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-273">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20134"></a><span data-ttu-id="9ef23-274">20134</span><span class="sxs-lookup"><span data-stu-id="9ef23-274">20134</span></span>
<span data-ttu-id="9ef23-p130">要求に、PATCH アクションのターゲットとして無効な要素が指定されています。ターゲットで **data-id** 識別子が使用されている場合は、プレフィックスとして # 記号が付いていることを確認してください。「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p130">Your request specifies an invalid element as the target of the PATCH action. If the target uses the **data-id** identifier, make sure it's prefixed with a # symbol. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20135"></a><span data-ttu-id="9ef23-278">20135</span><span class="sxs-lookup"><span data-stu-id="9ef23-278">20135</span></span>
<span data-ttu-id="9ef23-p131">要求に指定されたエンティティの種類は、PATCH 操作に対してはサポートされていません。「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p131">Your request specifies an entity type that is not supported for the PATCH operation. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20136"></a><span data-ttu-id="9ef23-281">20136</span><span class="sxs-lookup"><span data-stu-id="9ef23-281">20136</span></span>
<span data-ttu-id="9ef23-p132">要求に含まれている **data-render-src** または **data-render-method** 属性が無効であるか、または不足しています。「[キャプチャからデータを抽出する](onenote-extract-data.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p132">Your request contains an invalid or missing **data-render-src** or **data-render-method** attribute. See [Extract data from captures](onenote-extract-data.md).</span></span>

### <a name="20137"></a><span data-ttu-id="9ef23-284">20137</span><span class="sxs-lookup"><span data-stu-id="9ef23-284">20137</span></span>
<span data-ttu-id="9ef23-285">このターゲット ページにおいて、PATCH 要求はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-285">The target page does not support PATCH requests.</span></span>

### <a name="20138"></a><span data-ttu-id="9ef23-286">20138</span><span class="sxs-lookup"><span data-stu-id="9ef23-286">20138</span></span>
<span data-ttu-id="9ef23-p133">PATCH 要求のターゲット要素の種類では、**append** 操作はサポートされていません。「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p133">The target element type in your PATCH request doesn't support the **append** action. See [Update page content](onenote-update-page.md).</span></span>

### <a name="20139"></a><span data-ttu-id="9ef23-289">20139</span><span class="sxs-lookup"><span data-stu-id="9ef23-289">20139</span></span>
<span data-ttu-id="9ef23-p134">要求に、無効な **data-tag** 属性値が含まれています。「[ノート シールを使用する](onenote-note-tags.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p134">Your request contains an invalid **data-tag** attribute value. See [Use note tags](onenote-note-tags.md).</span></span>

### <a name="20140"></a><span data-ttu-id="9ef23-292">20140</span><span class="sxs-lookup"><span data-stu-id="9ef23-292">20140</span></span>
<span data-ttu-id="9ef23-293">要求に、無効な **data-tag** ステータス値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-293">Your request contains an invalid **data-tag** status value.</span></span> <span data-ttu-id="9ef23-294">チェック ボックスのノート シールには、**completed** ステータスを指定できます。</span><span class="sxs-lookup"><span data-stu-id="9ef23-294">Check box note tags can have a **completed** status.</span></span> 

<span data-ttu-id="9ef23-295">例:</span><span class="sxs-lookup"><span data-stu-id="9ef23-295">Example:</span></span>

```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
<span data-ttu-id="9ef23-296">「[ノート シールを使用する](onenote-note-tags.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-296">See [Use note tags](onenote-note-tags.md).</span></span>

### <a name="20141"></a><span data-ttu-id="9ef23-297">20141</span><span class="sxs-lookup"><span data-stu-id="9ef23-297">20141</span></span>
<span data-ttu-id="9ef23-298">PATCH 要求のターゲット要素の種類では、指定の操作はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-298">The target in your PATCH request doesn't support the specified action.</span></span> <span data-ttu-id="9ef23-299">「[ページ コンテンツの更新](onenote-update-page.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-299">See [Update page content](onenote-update-page.md).</span></span>

### <a name="20142"></a><span data-ttu-id="9ef23-300">20142</span><span class="sxs-lookup"><span data-stu-id="9ef23-300">20142</span></span>
<span data-ttu-id="9ef23-p137">要求に、子エンティティの親、または親エンティティの子に対する **expand** 式が含まれていますが、それはサポートされていません。「[サポートされる OData のクエリ文字列オプション](onenote-get-content.md#supported-odata-query-string-options)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p137">Your request contains an **expand** expression for a parent of child entities or a child of parent entities, which is not supported. See [Supported OData query string options](onenote-get-content.md#supported-odata-query-string-options).</span></span>

### <a name="20143"></a><span data-ttu-id="9ef23-303">20143</span><span class="sxs-lookup"><span data-stu-id="9ef23-303">20143</span></span>
<span data-ttu-id="9ef23-304">OData クエリが無効です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-304">The OData query is invalid.</span></span>

### <a name="20144"></a><span data-ttu-id="9ef23-305">20144</span><span class="sxs-lookup"><span data-stu-id="9ef23-305">20144</span></span>
<span data-ttu-id="9ef23-306">要求に、ナビゲートでないプロパティに対する **expand** 式が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-306">Your request contains an **expand** expression for a non-navigation property.</span></span> <span data-ttu-id="9ef23-307">展開できるのは、ナビゲート プロパティだけです。</span><span class="sxs-lookup"><span data-stu-id="9ef23-307">Only navigation properties can be expanded.</span></span>

### <a name="20145"></a><span data-ttu-id="9ef23-308">20145</span><span class="sxs-lookup"><span data-stu-id="9ef23-308">20145</span></span>
<span data-ttu-id="9ef23-309">要求の **select** 式または **expand** 式に、無効な用語が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-309">The **select** or **expand** expression in your request contains an invalid term.</span></span>

### <a name="20146"></a><span data-ttu-id="9ef23-310">20146</span><span class="sxs-lookup"><span data-stu-id="9ef23-310">20146</span></span>
<span data-ttu-id="9ef23-311">要素で `style="position:absolute"` 属性が指定されていますが、**body** 要素で `data-absolute-enabled="true"` が指定されていません。この指定は、配置をサポートするためには必須です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-311">The `style="position:absolute"` attribute is specified on an element, but the **body** element does not specify `data-absolute-enabled="true"`, which is required to support positioning.</span></span> <span data-ttu-id="9ef23-312">すべての位置設定が無視されます。</span><span class="sxs-lookup"><span data-stu-id="9ef23-312">All position settings will be ignored.</span></span> <span data-ttu-id="9ef23-313">「[絶対位置で配置された要素の作成](onenote-abs-pos.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-313">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20147"></a><span data-ttu-id="9ef23-314">20147</span><span class="sxs-lookup"><span data-stu-id="9ef23-314">20147</span></span>
<span data-ttu-id="9ef23-315">サポートされていない **body** 要素の直接の子ではない要素で `style="position:absolute"` 属性が指定されています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-315">The `style="position:absolute"` attribute is specified on an element that is not a direct child of the **body** element, which is not supported.</span></span> <span data-ttu-id="9ef23-316">要素が **div**、**img**、**object** の場合、それを body の直接の子にします。直接の子にしない場合、位置設定が無視され、絶対位置で配置された div の中でそのコンテンツがレンダリングされます。</span><span class="sxs-lookup"><span data-stu-id="9ef23-316">If the element is a **div**, **img**, or **object**, make it a direct child of the body; otherwise the position settings will be ignored and its content will render inside an absolute positioned div.</span></span> <span data-ttu-id="9ef23-317">「[絶対位置で配置された要素の作成](onenote-abs-pos.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-317">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20148"></a><span data-ttu-id="9ef23-318">20148</span><span class="sxs-lookup"><span data-stu-id="9ef23-318">20148</span></span>
<span data-ttu-id="9ef23-319">`style="position:absolute"` 属性がそれをサポートしない種類の要素で指定されています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-319">The `style="position:absolute"` attribute is specified on an element type that does not support it.</span></span> <span data-ttu-id="9ef23-320">ページ本文の直接の子である **div**、**img**、**object** 要素だけが位置設定をサポートします。</span><span class="sxs-lookup"><span data-stu-id="9ef23-320">Only **div**, **img**, and **object** elements that are direct children of the page body support positioning.</span></span> <span data-ttu-id="9ef23-321">「[絶対位置で配置された要素の作成](onenote-abs-pos.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-321">See [Create absolute positioned elements](onenote-abs-pos.md).</span></span>

### <a name="20149"></a><span data-ttu-id="9ef23-322">20149</span><span class="sxs-lookup"><span data-stu-id="9ef23-322">20149</span></span>
<span data-ttu-id="9ef23-323">要求が指定しているターゲット要素が見つかりません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-323">Your request specifies a target element that cannot be found.</span></span>

### <a name="20150"></a><span data-ttu-id="9ef23-324">20150</span><span class="sxs-lookup"><span data-stu-id="9ef23-324">20150</span></span>
<span data-ttu-id="9ef23-325">この認証の種類には、この要求は無効です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-325">The request is not valid for this authentication type.</span></span> <span data-ttu-id="9ef23-326">代わりに、`../me/onenote/` パスを使用してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-326">Use the `../me/onenote/` path instead.</span></span>

### <a name="20151"></a><span data-ttu-id="9ef23-327">20151</span><span class="sxs-lookup"><span data-stu-id="9ef23-327">20151</span></span>
<span data-ttu-id="9ef23-328">この認証の種類には、この要求は無効です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-328">The request is not valid for this authentication type.</span></span> <span data-ttu-id="9ef23-329">`../me/onenote/section/{id}/pages` エンドポイントを使用し、特定のセクションにページを作成します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-329">Use the `../me/onenote/section/{id}/pages` endpoint to create a page in a specific section.</span></span>

### <a name="20152"></a><span data-ttu-id="9ef23-330">20152</span><span class="sxs-lookup"><span data-stu-id="9ef23-330">20152</span></span>
<span data-ttu-id="9ef23-p144">エンティティに name 値が指定されていません。名前を定義する必要があり、その場合、名前が空白だけであってはなりません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p144">There is no name value specified for the entity. The name must be defined, and it cannot contain whitespaces only.</span></span>

### <a name="20153"></a><span data-ttu-id="9ef23-333">20153</span><span class="sxs-lookup"><span data-stu-id="9ef23-333">20153</span></span>
<span data-ttu-id="9ef23-334">エンティティ名に使用できない文字が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-334">The entity name contains invalid characters.</span></span> <span data-ttu-id="9ef23-335">名前には、以下の文字を含めることはできません: `? * \ / : < > | & # " % ~`</span><span class="sxs-lookup"><span data-stu-id="9ef23-335">The name cannot contain the following characters: `? * \ / : < > | & # " % ~`</span></span>

### <a name="20154"></a><span data-ttu-id="9ef23-336">20154</span><span class="sxs-lookup"><span data-stu-id="9ef23-336">20154</span></span>
<span data-ttu-id="9ef23-337">エンティティ名を空白で始めることはできません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-337">The entity name cannot start with a space.</span></span>

### <a name="20155"></a><span data-ttu-id="9ef23-338">20155</span><span class="sxs-lookup"><span data-stu-id="9ef23-338">20155</span></span>
<span data-ttu-id="9ef23-p146">エンティティ名が長すぎます。ノートブック名には 128 文字までの制限があります。他のエンティティ名には 50 文字までの制限があります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p146">The entity name is too long. Notebook names have a 128-character limit. Other entity names have a 50-character limit.</span></span>

### <a name="20156"></a><span data-ttu-id="9ef23-342">20156</span><span class="sxs-lookup"><span data-stu-id="9ef23-342">20156</span></span>
<span data-ttu-id="9ef23-343">宛先リソースの指定された ID が存在しません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-343">The specified ID for the destination resource does not exist.</span></span>

### <a name="20157"></a><span data-ttu-id="9ef23-344">20157</span><span class="sxs-lookup"><span data-stu-id="9ef23-344">20157</span></span>
<span data-ttu-id="9ef23-345">宛先エンティティの指定された ID が無効です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-345">The specified ID for the destination entity is invalid.</span></span>

### <a name="20158"></a><span data-ttu-id="9ef23-346">20158</span><span class="sxs-lookup"><span data-stu-id="9ef23-346">20158</span></span>
<span data-ttu-id="9ef23-347">要求に指定されているサイト URL のメタデータを取得できません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-347">Unable to get metadata for the site URL specified in the request.</span></span> <span data-ttu-id="9ef23-348">指定された URL の形式を確認してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-348">Check the format of the supplied URL.</span></span> <span data-ttu-id="9ef23-349">サポートされている形式は `https://domain.sharepoint.com/site-a` と `https://domain.com/sites/site-a` です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-349">Supported formats include `https://domain.sharepoint.com/site-a` and `https://domain.com/sites/site-a`.</span></span>

### <a name="20160"></a><span data-ttu-id="9ef23-350">20160</span><span class="sxs-lookup"><span data-stu-id="9ef23-350">20160</span></span>
<span data-ttu-id="9ef23-351">指定した ID を持つ Office 365 統合グループを見つけることができません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-351">Unable to find an Office 365 unified group that has the specified ID.</span></span>

### <a name="20161"></a><span data-ttu-id="9ef23-352">20161</span><span class="sxs-lookup"><span data-stu-id="9ef23-352">20161</span></span>
<span data-ttu-id="9ef23-p148">コンテキストで、有効なユーザー ID が指定されていません。一般的なエラーの 1 つとして、PUID/CID が 16 進数ではなく long 型として渡されたことが挙げられます。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p148">The context does not specify a valid user ID. One common error is that PUID/CID was passed in as a long instead of a hex.</span></span>

### <a name="20166"></a><span data-ttu-id="9ef23-355">20166</span><span class="sxs-lookup"><span data-stu-id="9ef23-355">20166</span></span>
<span data-ttu-id="9ef23-356">アプリケーションは、短時間に非常に多くの要求をユーザーの代理で発行しました。</span><span class="sxs-lookup"><span data-stu-id="9ef23-356">The application has issued too many requests on behalf of a user in a short period of time.</span></span> <span data-ttu-id="9ef23-357">OneNote API の安定性と応答性を保つために、アプリケーションがリソースを消費しすぎることが検出されると、API は 429 ステータス コードとこのエラーを返します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-357">To help ensure that the OneNote API remains stable and responsive, the API returns a 429 status code and this error when it detects that an application is using too many resources.</span></span> 

<span data-ttu-id="9ef23-358">詳細については、「[OneNote API の調整とその回避方法](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-358">For more information, see [OneNote API throttling and how to avoid it](https://blogs.msdn.com/b/onenotedev/archive/2016/01/13/onenote-api-throttling-and-best-practices.aspx).</span></span>

### <a name="20168"></a><span data-ttu-id="9ef23-359">20168</span><span class="sxs-lookup"><span data-stu-id="9ef23-359">20168</span></span>
<span data-ttu-id="9ef23-360">要求に指定されているビデオ ソースはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-360">The video source specified in the request is not supported.</span></span> <span data-ttu-id="9ef23-361">現行の一覧については、「[サポートされているビデオ サイト](onenote-images-files.md#adding-videos)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-361">See [Supported video sites](onenote-images-files.md#adding-videos) for the current list.</span></span>


## <a name="codes-from-30001-to-39999"></a><span data-ttu-id="9ef23-362">30001 から 39999 のコード</span><span class="sxs-lookup"><span data-stu-id="9ef23-362">Codes from 30001 to 39999</span></span>
<span data-ttu-id="9ef23-363">ユーザーのアカウントに問題があります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-363">Something is wrong with the user's account.</span></span>

### <a name="30101"></a><span data-ttu-id="9ef23-364">30101</span><span class="sxs-lookup"><span data-stu-id="9ef23-364">30101</span></span>
<span data-ttu-id="9ef23-p151">ユーザー アカウントの OneDrive のクォータを超えています。「[OneDrive](https://onedrive.live.com/about/ja-JP/)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p151">The user account has exceeded its OneDrive quota. See [OneDrive](https://onedrive.live.com/about/ja-JP/).</span></span>

### <a name="30102"></a><span data-ttu-id="9ef23-367">30102</span><span class="sxs-lookup"><span data-stu-id="9ef23-367">30102</span></span>
<span data-ttu-id="9ef23-368">要求されたセクションは、最大サイズに達したため、これ以上追加できません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-368">Nothing more can be added to the requested section because it has reached its maximum size.</span></span>

### <a name="30103"></a><span data-ttu-id="9ef23-369">30103</span><span class="sxs-lookup"><span data-stu-id="9ef23-369">30103</span></span>
<span data-ttu-id="9ef23-p152">要求に対するリソース消費量が多すぎます。対象のユーザー アカウントに大きいデータセットが含まれているか、サービスが同じサイト (ユーザーの個人用サイトやチーム サイトなど) に対する多数の要求を同時に受信しています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p152">Resource consumption is too high for the request. Either the target user account has a large dataset, or the service is receiving a high number of concurrent requests to the same site (for example, the user's personal site or a team site).</span></span>

### <a name="30104"></a><span data-ttu-id="9ef23-372">30104</span><span class="sxs-lookup"><span data-stu-id="9ef23-372">30104</span></span>
<span data-ttu-id="9ef23-373">ユーザー アカウントが中断されています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-373">The user account has been suspended.</span></span>

### <a name="30105"></a><span data-ttu-id="9ef23-374">30105</span><span class="sxs-lookup"><span data-stu-id="9ef23-374">30105</span></span>
<span data-ttu-id="9ef23-p153">ノートブックにアクセスする必要がある、ユーザーの個人用 OneDrive for Business サイトがプロビジョニングされていません。OneNote サービスは今すぐサイトをプロビジョニングします。この処理には数分かかることがあります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p153">The user's personal OneDrive for Business site is not provisioned, which is required to access notebooks. The OneNote service will provision the site now. This process may take several minutes.</span></span>

### <a name="30106"></a><span data-ttu-id="9ef23-378">30106</span><span class="sxs-lookup"><span data-stu-id="9ef23-378">30106</span></span>
<span data-ttu-id="9ef23-379">OneDrive for Business は、ユーザーのためにプロビジョニング中です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-379">OneDrive for Business is being provisioned for the user.</span></span>

### <a name="30108"></a><span data-ttu-id="9ef23-380">30108</span><span class="sxs-lookup"><span data-stu-id="9ef23-380">30108</span></span>
<span data-ttu-id="9ef23-381">ユーザーの個人用 OneDrive for Business を取得できませんでした。</span><span class="sxs-lookup"><span data-stu-id="9ef23-381">The user's personal OneDrive for Business could not be retrieved.</span></span> <span data-ttu-id="9ef23-382">次の表に、いくつか考えられる原因を示します。</span><span class="sxs-lookup"><span data-stu-id="9ef23-382">The following table lists some possible causes.</span></span>

| <span data-ttu-id="9ef23-383">原因</span><span class="sxs-lookup"><span data-stu-id="9ef23-383">Cause</span></span> | <span data-ttu-id="9ef23-384">解決策</span><span class="sxs-lookup"><span data-stu-id="9ef23-384">Resolution</span></span> |
|:------|:------|
| <span data-ttu-id="9ef23-385">ユーザーの個人用サイトがプロビジョニングされていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-385">The user's personal site has not been provisioned.</span></span> | <span data-ttu-id="9ef23-p155">ユーザーは、OneDrive for Business を開き、サイトをプロビジョニングするためのすべての指示に従います。これが失敗した場合は、Office 365 テナント管理者に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-p155">The user should open OneDrive for Business and follow any instructions to provision the site. If this fails, they should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="9ef23-388">ユーザーの個人用サイトは現在プロビジョニング中です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-388">The user's personal site is currently being provisioned.</span></span> | <span data-ttu-id="9ef23-389">後で要求を再試行してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-389">Try the request later.</span></span> |
| <span data-ttu-id="9ef23-390">ユーザーは、有効な OneDrive for Business ライセンスを持っていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-390">The user does not have a valid OneDrive for Business license.</span></span> | <span data-ttu-id="9ef23-391">Office 365 テナント管理者に問い合わせてください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-391">The user should contact their Office 365 tenant administrator.</span></span> |
| <span data-ttu-id="9ef23-392">ネットワークの問題により、要求が正常に送信されていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-392">A network issue prevented the request from being successfully sent.</span></span> | <span data-ttu-id="9ef23-393">後で要求をお試しください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-393">Try the request later.</span></span> |

### <a name="30109"></a><span data-ttu-id="9ef23-394">30109</span><span class="sxs-lookup"><span data-stu-id="9ef23-394">30109</span></span>
<span data-ttu-id="9ef23-395">要求の一部のユーザーは存在しません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-395">Some users in the request do not exist.</span></span>

### <a name="30110"></a><span data-ttu-id="9ef23-396">30110</span><span class="sxs-lookup"><span data-stu-id="9ef23-396">30110</span></span>
<span data-ttu-id="9ef23-397">このテナントの学生情報サービスが登録されていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-397">Student Information Services has not been registered for this tenant.</span></span>

### <a name="30111"></a><span data-ttu-id="9ef23-398">30111</span><span class="sxs-lookup"><span data-stu-id="9ef23-398">30111</span></span>
<span data-ttu-id="9ef23-399">学生情報サービスに一般的なエラーがあります。</span><span class="sxs-lookup"><span data-stu-id="9ef23-399">There is a generic error with Student Information Services.</span></span>

### <a name="30112"></a><span data-ttu-id="9ef23-400">30112</span><span class="sxs-lookup"><span data-stu-id="9ef23-400">30112</span></span>
<span data-ttu-id="9ef23-401">要求によって影響を受けた複数のユーザーは、同じユーザー名でした。</span><span class="sxs-lookup"><span data-stu-id="9ef23-401">Multiple users affected by the request had the same username.</span></span>

### <a name="30113"></a><span data-ttu-id="9ef23-402">30113</span><span class="sxs-lookup"><span data-stu-id="9ef23-402">30113</span></span>
<span data-ttu-id="9ef23-403">ノートブックは、招待を許可するように構成されていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-403">The notebook is not configured to allow invites.</span></span>

### <a name="30114"></a><span data-ttu-id="9ef23-404">30114</span><span class="sxs-lookup"><span data-stu-id="9ef23-404">30114</span></span>
<span data-ttu-id="9ef23-405">必須パラメーターがありません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-405">There is a required parameter missing.</span></span>

## <a name="codes-from-40001-to-49999"></a><span data-ttu-id="9ef23-406">40001 から 49999 のコード</span><span class="sxs-lookup"><span data-stu-id="9ef23-406">Codes from 40001 to 49999</span></span>
<span data-ttu-id="9ef23-407">ユーザーまたはアプリケーションに、適切なアクセス許可がありません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-407">The user or application does not have the correct permissions.</span></span>

### <a name="40001"></a><span data-ttu-id="9ef23-408">40001</span><span class="sxs-lookup"><span data-stu-id="9ef23-408">40001</span></span>
<span data-ttu-id="9ef23-409">要求に、有効な OAuth トークンが含まれていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-409">The request doesn't contain a valid OAuth token.</span></span> <span data-ttu-id="9ef23-410">「[メモのアクセス許可](permissions-reference.md#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-410">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40002"></a><span data-ttu-id="9ef23-411">40002</span><span class="sxs-lookup"><span data-stu-id="9ef23-411">40002</span></span>
<span data-ttu-id="9ef23-412">ユーザーは、要求された場所に書き込むアクセス許可を持っていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-412">The user doesn't have permission to write to the requested location.</span></span>

### <a name="40003"></a><span data-ttu-id="9ef23-413">40003</span><span class="sxs-lookup"><span data-stu-id="9ef23-413">40003</span></span>
<span data-ttu-id="9ef23-414">ユーザーは、要求されたリソースにアクセスする許可を持っていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-414">The user doesn't have permission to access the requested resource.</span></span>

### <a name="40004"></a><span data-ttu-id="9ef23-415">40004</span><span class="sxs-lookup"><span data-stu-id="9ef23-415">40004</span></span>
<span data-ttu-id="9ef23-416">OAuth トークンには、要求されたアクションを実行するために必要なスコープが含まれていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-416">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="9ef23-417">「[メモのアクセス許可](permissions-reference.md#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-417">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40006"></a><span data-ttu-id="9ef23-418">40006</span><span class="sxs-lookup"><span data-stu-id="9ef23-418">40006</span></span> 
<span data-ttu-id="9ef23-419">OAuth トークンには、要求されたアクションを実行するために必要なスコープが含まれていません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-419">The OAuth token doesn't have the required scopes to perform the requested action.</span></span> <span data-ttu-id="9ef23-420">具体的には、編集のアクセス許可です。</span><span class="sxs-lookup"><span data-stu-id="9ef23-420">Specifically the edit permission.</span></span> <span data-ttu-id="9ef23-421">「[メモのアクセス許可](permissions-reference.md#notes-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9ef23-421">See [Notes permissions](permissions-reference.md#notes-permissions).</span></span>

### <a name="40007"></a><span data-ttu-id="9ef23-422">40007</span><span class="sxs-lookup"><span data-stu-id="9ef23-422">40007</span></span>
<span data-ttu-id="9ef23-423">ユーザーには、このリソースにアクセスする権限がありません。</span><span class="sxs-lookup"><span data-stu-id="9ef23-423">The user does not have permissions to access this resource.</span></span>

### <a name="40008"></a><span data-ttu-id="9ef23-424">40008</span><span class="sxs-lookup"><span data-stu-id="9ef23-424">40008</span></span>
<span data-ttu-id="9ef23-425">このリソースへのアクセスが禁止されています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-425">Access is Forbidden for this resource.</span></span>

### <a name="40009"></a><span data-ttu-id="9ef23-426">40009</span><span class="sxs-lookup"><span data-stu-id="9ef23-426">40009</span></span>
<span data-ttu-id="9ef23-427">コンテナーは、既に別のリソースに使用されています。</span><span class="sxs-lookup"><span data-stu-id="9ef23-427">The container is already in use by another resource.</span></span>

## <a name="see-also"></a><span data-ttu-id="9ef23-428">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ef23-428">See also</span></span>

- [<span data-ttu-id="9ef23-429">Microsoft Graph のエラー応答とリソースの種類</span><span class="sxs-lookup"><span data-stu-id="9ef23-429">Microsoft Graph error responses and resource types</span></span>](errors.md)
- [<span data-ttu-id="9ef23-430">OneNote の参照</span><span class="sxs-lookup"><span data-stu-id="9ef23-430">OneNote reference</span></span>](/graph/api/resources/onenote?view=graph-rest-1.0)

