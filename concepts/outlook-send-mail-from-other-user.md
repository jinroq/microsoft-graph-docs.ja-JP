---
title: 別のユーザーを差出人として Outlook メッセージを送信する
description: 別のユーザーまたは Microsoft Graph の共有メールボックスとして Outlook メッセージを送信するには、メールボックス所有者として送信するアクセス許可または代理人として送信するアクセス許可を使用します。
author: jasonjoh
localization_priority: Priority
ms.prod: outlook
ms.date: 01/16/2019
ms.openlocfilehash: 0921cec73d405262470ed30b7f0d61534f6b5ab4
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/15/2019
ms.locfileid: "34036571"
---
# <a name="send-outlook-messages-from-another-user"></a><span data-ttu-id="f22c3-103">別のユーザーを差出人として Outlook メッセージを送信する</span><span class="sxs-lookup"><span data-stu-id="f22c3-103">Send Outlook messages from another user</span></span>

<span data-ttu-id="f22c3-104">Exchange Online で提供される[メールボックスのアクセス許可](/Exchange/recipients/mailbox-permissions)を使用すると、ユーザーは、他のユーザー、配布リスト、グループ、リソース、または共有メールボックスから送信されたものとして表示されるメールを送信することができます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-104">Exchange Online provides [mailbox permissions](/Exchange/recipients/mailbox-permissions) that allow a user to send mail that appears to be sent from another user, distribution list, group, resource, or shared mailbox.</span></span> <span data-ttu-id="f22c3-105">この機能は Microsoft Graph でもサポートされていますが、最終的な動作は、Exchange Online で付与される許可の種類およびメールの送信に使用する API の種類により異なります。</span><span class="sxs-lookup"><span data-stu-id="f22c3-105">Microsoft Graph supports this feature as well, but the end result varies depending on the exact permissions granted in Exchange Online and which API you use to send the mail.</span></span>

## <a name="permissions"></a><span data-ttu-id="f22c3-106">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="f22c3-106">Permissions</span></span>

<span data-ttu-id="f22c3-107">別のユーザーを差出人としたメッセージ送信に適用されるアクセス許可には 2 種類あります。[Microsoft Graph のアクセス許可](permissions-reference.md)とメールボックスのアクセス許可です。</span><span class="sxs-lookup"><span data-stu-id="f22c3-107">Two types of permissions apply to sending messages from another user: [Microsoft Graph permissions](permissions-reference.md), and mailbox permissions.</span></span>

### <a name="microsoft-graph-permissions"></a><span data-ttu-id="f22c3-108">Microsoft Graph のアクセス許可</span><span class="sxs-lookup"><span data-stu-id="f22c3-108">Microsoft Graph permissions</span></span>

<span data-ttu-id="f22c3-109">ユーザー トークンを使用するアプリケーションは、他のユーザーからメッセージを送信するために **Mail.Send.Shared** アクセス許可を使用します。</span><span class="sxs-lookup"><span data-stu-id="f22c3-109">In order to send messages from another user, applications that use user tokens use the **Mail.Send.Shared** permission.</span></span>

> [!NOTE]
> <span data-ttu-id="f22c3-110">ユーザー トークンではなくアプリケーション トークンが使用され、管理者が **Mail.Send** アクセス許可に同意しているアプリケーションでは、ユーザーのメールボックスから通常の方法でメールを送信することで、組織内の任意のユーザーとしてメールを送信できます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-110">Applications that use application tokens instead of user tokens and have the **Mail.Send** permission consented by an administrator can send mail as any user in the organization by sending the mail normally through the user's mailbox.</span></span>

### <a name="mailbox-permissions"></a><span data-ttu-id="f22c3-111">メールボックスのアクセス許可</span><span class="sxs-lookup"><span data-stu-id="f22c3-111">Mailbox permissions</span></span>

<span data-ttu-id="f22c3-112">別のユーザーを差出人としたメッセージの送信の動作に影響を与えるアクセス許可には、次の 2 つがあります。**代理人として送信する**と**メールボックス所有者として送信する**です。</span><span class="sxs-lookup"><span data-stu-id="f22c3-112">Two permissions affect the end result of sending a message from another user: **Send on Behalf** and **Send As**.</span></span> <span data-ttu-id="f22c3-113">**Mail.Send.Shared** アクセス許可を使用してアプリケーションにサインインするユーザーは、このうち少なくとも 1 つのアクセス許可を送信元のメールボックス、グループ、または配布リストに付与しておく必要があります。</span><span class="sxs-lookup"><span data-stu-id="f22c3-113">The user that is signed in to your application with the **Mail.Send.Shared** permission MUST have at least one of these permissions granted to the mailbox, group, or distribution list that the mail is from.</span></span>

#### <a name="send-on-behalf"></a><span data-ttu-id="f22c3-114">代理人として送信する</span><span class="sxs-lookup"><span data-stu-id="f22c3-114">Send on Behalf</span></span>

<span data-ttu-id="f22c3-115">このアクセス許可を使用する場合、メールの受信者の電子メール クライアントには、メッセージは、他のユーザーの代理としてアプリケーションのユーザーから送信されたものだと表示されます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-115">With this permission, the recipient of the email has an indication in their email client that the message was sent by the user of your application on behalf of another user.</span></span>

![あるユーザーにより別のユーザーの代理として送信されたメッセージを示す Outlook on the web のスクリーン ショット](images/outlook-sent-on-behalf.png)

<span data-ttu-id="f22c3-117">Microsoft Graph では、これは `sender` プロパティ (実際にメッセージを送信したユーザー) と `from` プロパティ (メッセージの送信者のように表示されるユーザーやグループなど) により公開れます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-117">This is exposed in Microsoft Graph as the `sender` (user that actually sent the message) and `from` (user/group/etc. that the message appears to be from) properties.</span></span>

```json
{
  "id": "AAMkAGE1...",
  "subject": "Send mail test",
  "sender": {
    "emailAddress": {
      "name": "Adele Vance",
      "address": "AdeleV@contoso.com"
    }
  },
  "from": {
    "emailAddress": {
      "name": "Pradeep Gupta",
      "address": "PradeepG@contoso.com"
    }
  }
}
```

<span data-ttu-id="f22c3-118">ユーザーは [Outlook を使用](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926)して、ユーザー自身のメールボックスへのアクセス許可を別のユーザーに付与することができます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-118">A user can grant this permission for their own mailbox to another user by [using Outlook](https://support.office.com/article/Allow-someone-else-to-manage-your-mail-and-calendar-41C40C04-3BD1-4D22-963A-28EAFEC25926).</span></span> <span data-ttu-id="f22c3-119">管理者は、[Office 365 管理センター](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide)で、このアクセス許可をすべてのメールボックス、グループ、または配布リストにこのアクセス許可を付与ことができます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-119">Administrators can grant this permission for any mailbox, group, or distribution list in the [Office 365 admin center](/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide).</span></span>

#### <a name="send-as"></a><span data-ttu-id="f22c3-120">メールボックス所有者として送信する</span><span class="sxs-lookup"><span data-stu-id="f22c3-120">Send As</span></span>

<span data-ttu-id="f22c3-121">このアクセス許可を使用する場合、別のユーザーとしてメッセージが送信されたことは表示されません。</span><span class="sxs-lookup"><span data-stu-id="f22c3-121">With this permission, there is no indication that the message was sent as a different user.</span></span> <span data-ttu-id="f22c3-122">`sender` プロパティと `from` プロパティで同じ値が使われます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-122">The `sender` and `from` properties have the same value.</span></span>

<span data-ttu-id="f22c3-123">ユーザーは、自分のメールボックスにこのアクセス許可を付与することはできません。</span><span class="sxs-lookup"><span data-stu-id="f22c3-123">Users cannot grant this permission to their mailboxes.</span></span> <span data-ttu-id="f22c3-124">管理者は、このアクセス許可を Office 365 管理センターで付与することができます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-124">Admins can grant this permission in the Office 365 admin center.</span></span>

## <a name="sending-with-microsoft-graph"></a><span data-ttu-id="f22c3-125">Microsoft Graph を使用して送信する</span><span class="sxs-lookup"><span data-stu-id="f22c3-125">Sending with Microsoft Graph</span></span>

<span data-ttu-id="f22c3-126">別のユーザーからメッセージを送信するには、[直接送信](/graph/api/user-sendmail?view=graph-rest-1.0)するか、または[下書きを作成](/graph/api/user-post-messages?view=graph-rest-1.0)しその後に[送信](/graph/api/message-send?view=graph-rest-1.0)します。</span><span class="sxs-lookup"><span data-stu-id="f22c3-126">You can send messages from another user by either [sending directly](/graph/api/user-sendmail?view=graph-rest-1.0) or by [creating a draft](/graph/api/user-post-messages?view=graph-rest-1.0) and then [sending it](/graph/api/message-send?view=graph-rest-1.0).</span></span>

<span data-ttu-id="f22c3-127">別のユーザーを差出人として送信するには、差出人の電子メール アドレスに送信する[メッセージ](/graph/api/resources/message?view=graph-rest-1.0)で `from` プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="f22c3-127">In order to send from another user, set the `from` property on the [message](/graph/api/resources/message?view=graph-rest-1.0) sent to the email address of the user to send from.</span></span> <span data-ttu-id="f22c3-128">`sender` プロパティは、サインインしているユーザーに付与されているメールボックスへのアクセス許可に基づいて Microsoft Graph により適切に設定されるので、ユーザーがこのプロパティを設定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="f22c3-128">You don't need to set the `sender` property - Microsoft Graph will set it appropriately, based on the mailbox permissions granted to the user who has signed in.</span></span>

<span data-ttu-id="f22c3-129">たとえば、`sales@contoso.com` グループからメールを送信するには、メッセージを次のように構成します。</span><span class="sxs-lookup"><span data-stu-id="f22c3-129">For example, to send mail from the `sales@contoso.com` group, configure the message as follows.</span></span>

```json
{
  "subject": "January sales report",
  "toRecipients": [
    {
      "emailAddress": {
        "address": "MeganB@contoso.com"
      }
    }
  ],
  "from": {
    "emailAddress": {
      "address": "sales@contoso.com"
    }
  }
}
```

## <a name="sent-items-behavior"></a><span data-ttu-id="f22c3-130">送信されたアイテムの動作</span><span class="sxs-lookup"><span data-stu-id="f22c3-130">Sent Items behavior</span></span>

<span data-ttu-id="f22c3-131">メッセージを送信後、送信したメッセージはメッセージを送信したユーザーの [送信済みアイテム] フォルダー、差出人ユーザーの [送信済みアイテム] フォルダー、またはその両方に保存できます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-131">After the message is sent, it can be saved to the sending user's Sent Items folder, the from user's Sent Items folder, or both.</span></span> <span data-ttu-id="f22c3-132">どこにも保存されない場合もあります。</span><span class="sxs-lookup"><span data-stu-id="f22c3-132">It can also not be saved at all.</span></span>

> [!NOTE]
> <span data-ttu-id="f22c3-133">メールボックスを持たないアドレス (例: 配布リスト) からメッセージが送信する場合、差出人ユーザーの [送信済みアイテム] はありません。</span><span class="sxs-lookup"><span data-stu-id="f22c3-133">If the message is sent from an address that does not have a mailbox (a distribution list, for example), there is no Sent Items for the from user.</span></span>

- <span data-ttu-id="f22c3-134">アプリケーションが `/me` エンドポイント (または `user-id` の部分がサインインしているユーザーに相当する `/users/{user-id}`) を使用して送信する場合、既定では、メッセージは送信ユーザーの [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-134">If your application sends by using the `/me` endpoint (or `/users/{user-id}` where the `user-id` corresponds to the signed in user), by default, the message will be saved in the sending user's Sent Items folder.</span></span>
- <span data-ttu-id="f22c3-135">アプリケーションが、`user-id` の部分が差出人ユーザーに相当する `/users/{user-id}` を使用して送信する場合、規定では、メッセージは差出人ユーザーの [送信済みアイテム] フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-135">If your application sends by using the `/users/{user-id}` where the `user-id` corresponds to the from user, by default, the message will be saved in the from user's Sent Items folder.</span></span>
    > [!IMPORTANT]
    > <span data-ttu-id="f22c3-136">この方法で送信するためには、送信ユーザーは、**代理人として送信する**アクセス許可または**メールボックス所有者として送信する**アクセス許可に加え、**フル アクセス**のメールボックス アクセス許可を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f22c3-136">In order to send this way, the sending user must have the **Full Access** mailbox permission in addition to either the **Send on Behalf** or **Send As** permission.</span></span>

<span data-ttu-id="f22c3-137">既定の動作は、他の外部の要因によって変わります。</span><span class="sxs-lookup"><span data-stu-id="f22c3-137">The default behavior can be changed by other outside factors:</span></span>

- <span data-ttu-id="f22c3-138">管理者は、差出人ユーザーのメールボックスで、[代理人から送信されたメッセージのコピーを必ず　[送信済みアイテム] フォルダーに保存する](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox)ように更新できます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-138">Administrators can update the from user's mailbox to [always save a copy of messages sent from a delegate](/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox) to their Sent Items.</span></span>
- <span data-ttu-id="f22c3-139">[メールの送信](/graph/api/user-sendmail?view=graph-rest-1.0)要求で `saveToSentItems` プロパティを `false` に設定することで、アイテムが [送信済みアイテム] フォルダーに保存されないようにできます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-139">By setting the `saveToSentItems` property to `false` in a [send mail](/graph/api/user-sendmail?view=graph-rest-1.0) request, you can prevent the item from being saved to the Sent Items folder.</span></span> <span data-ttu-id="f22c3-140">ただし、管理者が "コピーを必ず保存する" 設定の構成を行っている場合、メッセージは引き続き差出人ユーザーの [送信済みアイテム] に保存されます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-140">However, if an administrator has configured the "always save a copy" setting, the message will still be saved to the from user's Sent Items.</span></span>

## <a name="examples"></a><span data-ttu-id="f22c3-141">例</span><span class="sxs-lookup"><span data-stu-id="f22c3-141">Examples</span></span>

### <a name="example-1-successful-send-through-me-endpoint"></a><span data-ttu-id="f22c3-142">例 1: /me エンドポイントを使用した送信の成功</span><span class="sxs-lookup"><span data-stu-id="f22c3-142">Example 1: Successful send through /me endpoint</span></span>

<span data-ttu-id="f22c3-143">この例では、Adele Vance に、Allan Deyoung のメールボックスへの**代理人として送信する**アクセス許可が付与されています。</span><span class="sxs-lookup"><span data-stu-id="f22c3-143">In this example, Adele Vance has been granted **Send on Behalf** permission to Allan Deyoung's mailbox.</span></span>

#### <a name="request"></a><span data-ttu-id="f22c3-144">要求</span><span class="sxs-lookup"><span data-stu-id="f22c3-144">Request</span></span>

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Expense reports",
    "body": {
      "contentType": "text",
      "content": "Have you submitted your expense reports yet?"
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": {
      "emailAddress": {
        "address": "AllanD@contoso.com"
      }
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="f22c3-145">応答</span><span class="sxs-lookup"><span data-stu-id="f22c3-145">Response</span></span>

```http
HTTP/1.1 202 Accepted
```

### <a name="example-2-unsuccessful-attempt-to-send-without-permissions"></a><span data-ttu-id="f22c3-146">例 2: アクセス許可がない状態での送信の失敗</span><span class="sxs-lookup"><span data-stu-id="f22c3-146">Example 2: Unsuccessful attempt to send without permissions</span></span>

<span data-ttu-id="f22c3-147">この例では、Adele Vance は Patti Fernandez を差出人としてメールを送信しようとしていますが、**代理人として送信する**アクセス許可も**メールボックス所有者として送信する**アクセス許可も付与されていません。</span><span class="sxs-lookup"><span data-stu-id="f22c3-147">In this example, Adele Vance attempts to send an email from Patti Fernandez, but has not been granted either the **Send on Behalf** or **Send As** permission.</span></span> <span data-ttu-id="f22c3-148">応答には `ErrorSendAsDenied` エラーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f22c3-148">The response contains a `ErrorSendAsDenied` error.</span></span>

<!-- markdownlint-disable MD024 -->

#### <a name="request"></a><span data-ttu-id="f22c3-149">要求</span><span class="sxs-lookup"><span data-stu-id="f22c3-149">Request</span></span>

```http
POST /me/sendmail
Content-Type: application/json

{
  "message": {
    "subject": "Support ticket",
    "body": {
      "contentType": "text",
      "content": "I noticed you opened a support ticket yesterday..."
    },
    "toRecipients": [
      {
        "emailAddress": {
          "address": "MeganB@contoso.com"
        }
      }
    ],
    "from": {
      "emailAddress": {
        "address": "PattiF@contoso.com"
      }
    }
  }
}
```

#### <a name="response"></a><span data-ttu-id="f22c3-150">応答</span><span class="sxs-lookup"><span data-stu-id="f22c3-150">Response</span></span>

```http
HTTP/1.1 403 Forbidden
Content-Type: application/json

{
  "error": {
    "code": "ErrorSendAsDenied",
    "message": "The user account which was used to submit this request does not have the right to send mail on behalf of the specified sending account., Cannot submit message.",
    "innerError": {
      "request-id": "24e7991e-01ae-4cc2-8e06-532a96fd8948",
      "date": "2019-01-16T18:53:25"
    }
  }
}
```

## <a name="next-steps"></a><span data-ttu-id="f22c3-151">次の手順</span><span class="sxs-lookup"><span data-stu-id="f22c3-151">Next steps</span></span>

<span data-ttu-id="f22c3-152">詳細情報:</span><span class="sxs-lookup"><span data-stu-id="f22c3-152">Find out more about:</span></span>

- [<span data-ttu-id="f22c3-153">Outlook メールと統合する理由</span><span class="sxs-lookup"><span data-stu-id="f22c3-153">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="f22c3-154">Microsoft Graph v1.0 の[メール API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) とメール PAPI の[用途](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases)。</span><span class="sxs-lookup"><span data-stu-id="f22c3-154">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and mail API [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      FileNotFound: '[/exchange/recipients-in-exchange-online/manage-user-mailboxes/automatically-save-sent-items-in-delegator-s-mailbox](always save a copy of messages sent from a delegate)'.",
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      InvalidUrlFormat '[/office365/admin/add-users/give-mailbox-permissions-to-another-user?view=o365-worldwide](Office 365 admin center)'.",
    "Error: /concepts/outlook-send-mail-from-other-user.md:\r\n      FileNotFound: '[/Exchange/recipients/mailbox-permissions](mailbox permissions)'. "
  ]
}
-->
