---
title: メッセージを更新する
description: メッセージ オブジェクトのプロパティを更新します。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 0bb42f1690f4391b5a99cb2bcbb0361bfb495862
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/25/2019
ms.locfileid: "35884687"
---
# <a name="update-message"></a><span data-ttu-id="6608e-103">メッセージを更新する</span><span class="sxs-lookup"><span data-stu-id="6608e-103">Update message</span></span>

<span data-ttu-id="6608e-104">メッセージ オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="6608e-104">Update the properties of a message object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6608e-105">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="6608e-105">Permissions</span></span>
<span data-ttu-id="6608e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6608e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6608e-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6608e-108">Permission type</span></span>      | <span data-ttu-id="6608e-109">アクセス許可 (特権の小さいものから大きいものへ)</span><span class="sxs-lookup"><span data-stu-id="6608e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6608e-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6608e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="6608e-111">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6608e-111">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6608e-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6608e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6608e-113">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6608e-113">Mail.ReadWrite</span></span>    |
|<span data-ttu-id="6608e-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6608e-114">Application</span></span> | <span data-ttu-id="6608e-115">Mail.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="6608e-115">Mail.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="6608e-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6608e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/messages/{id}
PATCH /users/{id | userPrincipalName}/messages/{id}
PATCH /me/mailFolders/{id}/messages/{id}
PATCH /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6608e-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6608e-117">Request headers</span></span>
| <span data-ttu-id="6608e-118">名前</span><span class="sxs-lookup"><span data-stu-id="6608e-118">Name</span></span>       | <span data-ttu-id="6608e-119">型</span><span class="sxs-lookup"><span data-stu-id="6608e-119">Type</span></span> | <span data-ttu-id="6608e-120">説明</span><span class="sxs-lookup"><span data-stu-id="6608e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6608e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6608e-121">Authorization</span></span>  | <span data-ttu-id="6608e-122">string</span><span class="sxs-lookup"><span data-stu-id="6608e-122">string</span></span>  | <span data-ttu-id="6608e-p102">ベアラー {トークン}。必須。</span><span class="sxs-lookup"><span data-stu-id="6608e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6608e-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6608e-125">Content-Type</span></span> | <span data-ttu-id="6608e-126">string</span><span class="sxs-lookup"><span data-stu-id="6608e-126">string</span></span>  | <span data-ttu-id="6608e-p103">エンティティ本文内のデータの性質です。必須。</span><span class="sxs-lookup"><span data-stu-id="6608e-p103">Nature of the data in the body of an entity. Required.</span></span> |
## <a name="request-body"></a><span data-ttu-id="6608e-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="6608e-129">Request body</span></span>
<span data-ttu-id="6608e-130">要求本文で、更新する関連フィールドの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="6608e-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6608e-131">要求本文に含まれない既存のプロパティは、以前の値のままになるか、他のプロパティ値の変化に基づいて再計算されます。</span><span class="sxs-lookup"><span data-stu-id="6608e-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6608e-132">最適なパフォーマンスを得るためには、変更されていない既存の値を含めないでください。</span><span class="sxs-lookup"><span data-stu-id="6608e-132">For best performance you shouldn't include existing values that haven't changed.</span></span> <span data-ttu-id="6608e-133">次のプロパティを更新できます。</span><span class="sxs-lookup"><span data-stu-id="6608e-133">The following properties can be updated.</span></span>

| <span data-ttu-id="6608e-134">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6608e-134">Property</span></span>     | <span data-ttu-id="6608e-135">型</span><span class="sxs-lookup"><span data-stu-id="6608e-135">Type</span></span>   |<span data-ttu-id="6608e-136">説明</span><span class="sxs-lookup"><span data-stu-id="6608e-136">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6608e-137">bccRecipients</span><span class="sxs-lookup"><span data-stu-id="6608e-137">bccRecipients</span></span>|<span data-ttu-id="6608e-138">受信者</span><span class="sxs-lookup"><span data-stu-id="6608e-138">Recipient</span></span>|<span data-ttu-id="6608e-139">メッセージの BCC 受信者。</span><span class="sxs-lookup"><span data-stu-id="6608e-139">The Bcc recipients for the message.</span></span> |
|<span data-ttu-id="6608e-140">body</span><span class="sxs-lookup"><span data-stu-id="6608e-140">body</span></span>|<span data-ttu-id="6608e-141">ItemBody</span><span class="sxs-lookup"><span data-stu-id="6608e-141">ItemBody</span></span>|<span data-ttu-id="6608e-142">メッセージの本文。</span><span class="sxs-lookup"><span data-stu-id="6608e-142">The body of the message.</span></span> <span data-ttu-id="6608e-143">isDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="6608e-143">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="6608e-144">categories</span><span class="sxs-lookup"><span data-stu-id="6608e-144">categories</span></span>|<span data-ttu-id="6608e-145">String collection</span><span class="sxs-lookup"><span data-stu-id="6608e-145">String collection</span></span>|<span data-ttu-id="6608e-146">メッセージに関連付けられたカテゴリ。</span><span class="sxs-lookup"><span data-stu-id="6608e-146">The categories associated with the message.</span></span>|
|<span data-ttu-id="6608e-147">ccRecipients</span><span class="sxs-lookup"><span data-stu-id="6608e-147">ccRecipients</span></span>|<span data-ttu-id="6608e-148">受信者コレクション</span><span class="sxs-lookup"><span data-stu-id="6608e-148">Recipient collection</span></span>|<span data-ttu-id="6608e-149">メッセージの CC 受信者。</span><span class="sxs-lookup"><span data-stu-id="6608e-149">The Cc recipients for the message.</span></span> |
|<span data-ttu-id="6608e-150">flag</span><span class="sxs-lookup"><span data-stu-id="6608e-150">flag</span></span>|[<span data-ttu-id="6608e-151">followUpFlag</span><span class="sxs-lookup"><span data-stu-id="6608e-151">followupFlag</span></span>](../resources/followupflag.md)|<span data-ttu-id="6608e-152">メッセージのステータス、開始日、期限、または完了日を示すフラグ値。</span><span class="sxs-lookup"><span data-stu-id="6608e-152">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="6608e-153">from</span><span class="sxs-lookup"><span data-stu-id="6608e-153">from</span></span>|<span data-ttu-id="6608e-154">受信者</span><span class="sxs-lookup"><span data-stu-id="6608e-154">Recipient</span></span>|<span data-ttu-id="6608e-155">メッセージのメールボックス所有者と送信者。</span><span class="sxs-lookup"><span data-stu-id="6608e-155">The mailbox owner and sender of the message.</span></span> <span data-ttu-id="6608e-156">実際に使用されているメールボックスに対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="6608e-156">Must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="6608e-157">importance</span><span class="sxs-lookup"><span data-stu-id="6608e-157">importance</span></span>|<span data-ttu-id="6608e-158">String</span><span class="sxs-lookup"><span data-stu-id="6608e-158">String</span></span>|<span data-ttu-id="6608e-159">メッセージの重要度です。</span><span class="sxs-lookup"><span data-stu-id="6608e-159">The importance of the message.</span></span> <span data-ttu-id="6608e-160">使用可能な値: `Low`、`Normal`、`High`。</span><span class="sxs-lookup"><span data-stu-id="6608e-160">The possible values are: `Low`, `Normal`, `High`.</span></span>|
|<span data-ttu-id="6608e-161">inferenceClassification</span><span class="sxs-lookup"><span data-stu-id="6608e-161">inferenceClassification</span></span> | <span data-ttu-id="6608e-162">String</span><span class="sxs-lookup"><span data-stu-id="6608e-162">String</span></span> | <span data-ttu-id="6608e-163">推定される関連性や重要性、または明示的なオーバーライドに基づく、ユーザーのメッセージの分類。</span><span class="sxs-lookup"><span data-stu-id="6608e-163">The classification of the message for the user, based on inferred relevance or importance, or on an explicit override.</span></span> <span data-ttu-id="6608e-164">使用可能な値: `focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="6608e-164">The possible values are: `focused` or `other`.</span></span> |
|<span data-ttu-id="6608e-165">internetMessageId</span><span class="sxs-lookup"><span data-stu-id="6608e-165">internetMessageId</span></span> |<span data-ttu-id="6608e-166">String</span><span class="sxs-lookup"><span data-stu-id="6608e-166">String</span></span> |<span data-ttu-id="6608e-167">[RFC2822](https://www.ietf.org/rfc/rfc2822.txt) によって指定された形式のメッセージ ID。</span><span class="sxs-lookup"><span data-stu-id="6608e-167">The message ID in the format specified by [RFC2822](https://www.ietf.org/rfc/rfc2822.txt).</span></span> <span data-ttu-id="6608e-168">isDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="6608e-168">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="6608e-169">isDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6608e-169">isDeliveryReceiptRequested</span></span>|<span data-ttu-id="6608e-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="6608e-170">Boolean</span></span>|<span data-ttu-id="6608e-171">メッセージの開封応答が要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6608e-171">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="6608e-172">isRead</span><span class="sxs-lookup"><span data-stu-id="6608e-172">isRead</span></span>|<span data-ttu-id="6608e-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="6608e-173">Boolean</span></span>|<span data-ttu-id="6608e-174">メッセージが開封されたかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6608e-174">Indicates whether the message has been read.</span></span>|
|<span data-ttu-id="6608e-175">isReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="6608e-175">isReadReceiptRequested</span></span>|<span data-ttu-id="6608e-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="6608e-176">Boolean</span></span>|<span data-ttu-id="6608e-177">メッセージの開封確認メッセージが要求されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6608e-177">Indicates whether a read receipt is requested for the message.</span></span>|
|<span data-ttu-id="6608e-178">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="6608e-178">multiValueExtendedProperties</span></span>|<span data-ttu-id="6608e-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6608e-179">[multiValueLegacyExtendedProperty](../resources/multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6608e-180">メッセージに対して定義された、複数値の拡張プロパティのコレクション。</span><span class="sxs-lookup"><span data-stu-id="6608e-180">The collection of multi-value extended properties defined for the message.</span></span> <span data-ttu-id="6608e-181">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="6608e-181">Nullable.</span></span>|
|<span data-ttu-id="6608e-182">replyTo</span><span class="sxs-lookup"><span data-stu-id="6608e-182">replyTo</span></span>|<span data-ttu-id="6608e-183">受信者コレクション</span><span class="sxs-lookup"><span data-stu-id="6608e-183">Recipient collection</span></span>|<span data-ttu-id="6608e-184">返信時に使用される電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="6608e-184">The email addresses to use when replying.</span></span> <span data-ttu-id="6608e-185">isDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="6608e-185">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="6608e-186">sender</span><span class="sxs-lookup"><span data-stu-id="6608e-186">sender</span></span>|<span data-ttu-id="6608e-187">受信者</span><span class="sxs-lookup"><span data-stu-id="6608e-187">Recipient</span></span>|<span data-ttu-id="6608e-188">メッセージを生成するために実際に使用されるアカウント。</span><span class="sxs-lookup"><span data-stu-id="6608e-188">The account that is actually used to generate the message.</span></span> <span data-ttu-id="6608e-189">
  [共有メールボックス](https://docs.microsoft.com/ja-JP/exchange/collaboration/shared-mailboxes/shared-mailboxes)からメッセージを送信するとき、またはメッセージを [delegate](https://support.office.com/ja-JP/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926) として送信するときに、更新可能です。</span><span class="sxs-lookup"><span data-stu-id="6608e-189">Updatable when sending a message from a [shared mailbox](https://docs.microsoft.com/en-us/exchange/collaboration/shared-mailboxes/shared-mailboxes), or sending a message as a [delegate](https://support.office.com/en-us/article/allow-someone-else-to-manage-your-mail-and-calendar-41c40c04-3bd1-4d22-963a-28eafec25926).</span></span> <span data-ttu-id="6608e-190">いずれの場合でも、この値は、実際に使用されているメールボックスに対応している必要があります。</span><span class="sxs-lookup"><span data-stu-id="6608e-190">In any case, the value must correspond to the actual mailbox used.</span></span>|
|<span data-ttu-id="6608e-191">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="6608e-191">singleValueExtendedProperties</span></span>|<span data-ttu-id="6608e-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6608e-192">[singleValueLegacyExtendedProperty](../resources/singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="6608e-193">メッセージに対して定義された、単一値の拡張プロパティのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6608e-193">The collection of single-value extended properties defined for the message.</span></span> <span data-ttu-id="6608e-194">Null 許容型です。</span><span class="sxs-lookup"><span data-stu-id="6608e-194">Nullable.</span></span>|
|<span data-ttu-id="6608e-195">subject</span><span class="sxs-lookup"><span data-stu-id="6608e-195">subject</span></span>|<span data-ttu-id="6608e-196">String</span><span class="sxs-lookup"><span data-stu-id="6608e-196">String</span></span>|<span data-ttu-id="6608e-197">メッセージの件名。</span><span class="sxs-lookup"><span data-stu-id="6608e-197">The subject of the message.</span></span> <span data-ttu-id="6608e-198">isDraft = true の場合にのみ更新可能です。</span><span class="sxs-lookup"><span data-stu-id="6608e-198">Updatable only if isDraft = true.</span></span>|
|<span data-ttu-id="6608e-199">toRecipients</span><span class="sxs-lookup"><span data-stu-id="6608e-199">toRecipients</span></span>|<span data-ttu-id="6608e-200">受信者コレクション</span><span class="sxs-lookup"><span data-stu-id="6608e-200">Recipient collection</span></span>|<span data-ttu-id="6608e-201">メッセージの宛先受信者。</span><span class="sxs-lookup"><span data-stu-id="6608e-201">The To recipients for the message.</span></span>|

<span data-ttu-id="6608e-202">**メッセージ** リソースは[拡張機能](/graph/extensibility-overview)をサポートしているため、`PATCH` 操作を使用して、既存の**メッセージ** インスタンスで拡張機能のカスタム プロパティにあるアプリ固有のデータを追加、更新、または削除することができます。</span><span class="sxs-lookup"><span data-stu-id="6608e-202">Since the **message** resource supports [extensions](/graph/extensibility-overview), you can use the `PATCH` operation to add, update, or delete your own app-specific data in custom properties of an extension in an existing **message** instance.</span></span>

## <a name="response"></a><span data-ttu-id="6608e-203">応答</span><span class="sxs-lookup"><span data-stu-id="6608e-203">Response</span></span>

<span data-ttu-id="6608e-204">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [message](../resources/message.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="6608e-204">If successful, this method returns a `200 OK` response code and updated [message](../resources/message.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6608e-205">例</span><span class="sxs-lookup"><span data-stu-id="6608e-205">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6608e-206">要求</span><span class="sxs-lookup"><span data-stu-id="6608e-206">Request</span></span>
<span data-ttu-id="6608e-207">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6608e-207">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6608e-208">HTTP</span><span class="sxs-lookup"><span data-stu-id="6608e-208">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_message"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/messages/{id}
Content-type: application/json
Content-length: 248

{
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "inferenceClassification": "other"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6608e-209">C#</span><span class="sxs-lookup"><span data-stu-id="6608e-209">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-message-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6608e-210">Javascript</span><span class="sxs-lookup"><span data-stu-id="6608e-210">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-message-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="6608e-211">Java</span><span class="sxs-lookup"><span data-stu-id="6608e-211">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-message-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6608e-212">応答</span><span class="sxs-lookup"><span data-stu-id="6608e-212">Response</span></span>
<span data-ttu-id="6608e-p115">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6608e-p115">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.message"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 248

{
  "receivedDateTime": "datetime-value",
  "sentDateTime": "datetime-value",
  "hasAttachments": true,
  "subject": "subject-value",
  "body": {
    "contentType": "",
    "content": "content-value"
  },
  "bodyPreview": "bodyPreview-value",
  "inferenceClassification": "other"
}
```

## <a name="see-also"></a><span data-ttu-id="6608e-216">関連項目</span><span class="sxs-lookup"><span data-stu-id="6608e-216">See also</span></span>

- [<span data-ttu-id="6608e-217">拡張機能を使用してカスタム データをリソースに追加する</span><span class="sxs-lookup"><span data-stu-id="6608e-217">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="6608e-218">オープン拡張機能を使用したユーザーへのカスタム データの追加 (プレビュー)</span><span class="sxs-lookup"><span data-stu-id="6608e-218">Add custom data to users using open extensions (preview)</span></span>](/graph/extensibility-open-users)
<!--
- [Add custom data to groups using schema extensions (preview)](/graph/extensibility-schema-groups)
-->


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update message",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
