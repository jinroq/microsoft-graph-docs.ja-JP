---
title: リソースの種類を説明します。
description: 相手の電子メール アドレスに基づいてユーザーに通知を表します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: f8e04722edf878b4f3851de837908dc5c0a02de7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523198"
---
# <a name="mention-resource-type"></a><span data-ttu-id="b5762-103">リソースの種類を説明します。</span><span class="sxs-lookup"><span data-stu-id="b5762-103">mention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5762-104">相手の電子メール アドレスに基づいてユーザーに通知を表します。</span><span class="sxs-lookup"><span data-stu-id="b5762-104">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="b5762-105">この通知の種類は、参照 @ とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="b5762-105">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="b5762-106">[メッセージ](../resources/message.md)リソースは、**説明**をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b5762-106">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="b5762-107">サインイン中のユーザーがそのメッセージ インスタンスに記載されているかどうかを示す**mentionsPreview**プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b5762-107">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="b5762-108">**紹介**のナビゲーション プロパティを取得の詳細を記載されている、またはそのインスタンスの参照を削除するをサポートしているも含まれています。</span><span class="sxs-lookup"><span data-stu-id="b5762-108">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="b5762-p103">メッセージを作成すると、アプリは、**Mentions** プロパティにメンションを含むことで、同じ `POST` 要求にメンションを作成できます。`$filter` クエリ パラメーターを含む `GET` 要求を使用して、アプリは、サインインしているユーザーのメールボックス内にある、ユーザーをメンションするすべてのメッセージを返すことができます。`$expand` クエリ パラメーターを含む `GET` 要求によって、アプリは特定のメッセージのすべてのメンションを展開できるようになります。</span><span class="sxs-lookup"><span data-stu-id="b5762-p103">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property. Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user. A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="b5762-p104">アプリがメッセージ内のメンションを設定して取得できるようにするこのメカニズムによって、簡易的な通知が可能になり、アプリが基になる **Mentions** プロパティを設定すると同時に、メンションを行うユーザーは既存のコンテキスト内に留まることができます (メッセージ本文の作成など)。メンションされたユーザーは、`$filter` または `$expand` クエリ パラメーターを含む `GET` 要求を介して、ユーザーがメンションされたかどうかとメンションされた場所を簡単に検索することができます。</span><span class="sxs-lookup"><span data-stu-id="b5762-p104">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property. Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="b5762-114">Outlook メール クライアントが表示され、ユーザーが入力するときに、 `@` 、メッセージの作成中に Outlook により、ユーザーを選択するか、または @ 言及を完了するための名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="b5762-114">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="b5762-115">作成し、メッセージまたはイベントを送信する前に、outlook は、"**説明**"プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="b5762-115">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="b5762-116">Outlook を使用しても`GET`での操作`$filter`と`$expand`、サインイン中のユーザー、ユーザーのことを説明するメッセージを検索できるように、迅速な対応を可能にするアクション アイテムや、ディスカッションをユーザーに警告します。</span><span class="sxs-lookup"><span data-stu-id="b5762-116">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b5762-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b5762-117">JSON representation</span></span>

<span data-ttu-id="b5762-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b5762-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mention"
}-->

```json
{
  "application": "string",
  "clientReference": "string",
  "createdBy": {"@odata.type": "microsoft.graph.emailAddress"},
  "createdDateTime": "DateTimeOffset",
  "deepLink": "string",
  "id": "string (identifier)",
  "mentioned": {"@odata.type": "microsoft.graph.emailAddress"},
  "mentionText": "string",
  "serverCreatedDateTime": "DateTimeOffset"
}

```
## <a name="properties"></a><span data-ttu-id="b5762-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5762-119">Properties</span></span>
| <span data-ttu-id="b5762-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b5762-120">Property</span></span>     | <span data-ttu-id="b5762-121">型</span><span class="sxs-lookup"><span data-stu-id="b5762-121">Type</span></span>   |<span data-ttu-id="b5762-122">説明</span><span class="sxs-lookup"><span data-stu-id="b5762-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5762-123">application</span><span class="sxs-lookup"><span data-stu-id="b5762-123">application</span></span> | <span data-ttu-id="b5762-124">String</span><span class="sxs-lookup"><span data-stu-id="b5762-124">String</span></span> | <span data-ttu-id="b5762-p106">メンションが作成されるアプリケーションの名前。省略可能。**Message** の場合は使用されず、null として既定値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b5762-p106">The name of the application where the mention is created. Optional. Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="b5762-128">ClientReference</span><span class="sxs-lookup"><span data-stu-id="b5762-128">clientReference</span></span> | <span data-ttu-id="b5762-129">String</span><span class="sxs-lookup"><span data-stu-id="b5762-129">String</span></span> | <span data-ttu-id="b5762-p107">リソース インスタンスの親を表す一意の識別子。省略可能。**Message** の場合は使用されず、null として既定値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b5762-p107">A unique identifier that represents a parent of the resource instance. Optional. Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="b5762-133">createdBy</span><span class="sxs-lookup"><span data-stu-id="b5762-133">createdBy</span></span>  | [<span data-ttu-id="b5762-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b5762-134">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="b5762-135">参照投稿を行ったユーザーの電子メール情報。</span><span class="sxs-lookup"><span data-stu-id="b5762-135">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="b5762-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b5762-136">createdDateTime</span></span>  |<span data-ttu-id="b5762-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5762-137">DateTimeOffset</span></span> |<span data-ttu-id="b5762-138">クライアントでメンションが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b5762-138">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="b5762-139">DeepLink</span><span class="sxs-lookup"><span data-stu-id="b5762-139">deepLink</span></span> | <span data-ttu-id="b5762-140">String</span><span class="sxs-lookup"><span data-stu-id="b5762-140">String</span></span> | <span data-ttu-id="b5762-p108">リソース インスタンス内のメンションのコンテキストへの深い Web リンク。省略可能。**Message** の場合は使用されず、null として既定値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b5762-p108">A deep web link to the context of the mention in the resource instance. Optional. Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="b5762-144">id</span><span class="sxs-lookup"><span data-stu-id="b5762-144">id</span></span> | <span data-ttu-id="b5762-145">String</span><span class="sxs-lookup"><span data-stu-id="b5762-145">String</span></span>| <span data-ttu-id="b5762-146">リソース インスタンス内のメンションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="b5762-146">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="b5762-147">Mentioned</span><span class="sxs-lookup"><span data-stu-id="b5762-147">mentioned</span></span> | [<span data-ttu-id="b5762-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="b5762-148">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="b5762-p109">メンションした人の電子メール情報。必須です。</span><span class="sxs-lookup"><span data-stu-id="b5762-p109">The email information of the mentioned person. Required.</span></span> |
|<span data-ttu-id="b5762-151">MentionText</span><span class="sxs-lookup"><span data-stu-id="b5762-151">mentionText</span></span> | <span data-ttu-id="b5762-152">String</span><span class="sxs-lookup"><span data-stu-id="b5762-152">String</span></span> | <span data-ttu-id="b5762-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="b5762-153">Optional.</span></span> <span data-ttu-id="b5762-154">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="b5762-154">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="b5762-155">メッセージで、参照を取得するには、代わりに、メッセージの**bodyPreview**プロパティには、参照してください。</span><span class="sxs-lookup"><span data-stu-id="b5762-155">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="b5762-156">ServerCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b5762-156">serverCreatedDateTime</span></span> | <span data-ttu-id="b5762-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b5762-157">DateTimeOffset</span></span> | <span data-ttu-id="b5762-p111">サーバーでメンションが作成された日時。省略可能。**Message** の場合は使用されず、null として既定値に設定されます。</span><span class="sxs-lookup"><span data-stu-id="b5762-p111">The date and time that the mention is created on the server. Optional. Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b5762-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b5762-161">Relationships</span></span>
<span data-ttu-id="b5762-162">なし</span><span class="sxs-lookup"><span data-stu-id="b5762-162">None</span></span>


## <a name="methods"></a><span data-ttu-id="b5762-163">メソッド</span><span class="sxs-lookup"><span data-stu-id="b5762-163">Methods</span></span>

| <span data-ttu-id="b5762-164">メソッド</span><span class="sxs-lookup"><span data-stu-id="b5762-164">Method</span></span>           | <span data-ttu-id="b5762-165">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b5762-165">Return Type</span></span>    |<span data-ttu-id="b5762-166">説明</span><span class="sxs-lookup"><span data-stu-id="b5762-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5762-167">[投稿](../api/user-sendmail.md#request-2)および送信</span><span class="sxs-lookup"><span data-stu-id="b5762-167">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="b5762-168">なし</span><span class="sxs-lookup"><span data-stu-id="b5762-168">None</span></span> | <span data-ttu-id="b5762-169">新しいメッセージの一部としてメンションを作成および送信する</span><span class="sxs-lookup"><span data-stu-id="b5762-169">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="b5762-170">新しい下書きを[投稿](../api/user-post-messages.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="b5762-170">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="b5762-171">**説明**する 1 つまたは複数オブジェクトを含む[メッセージ](../resources/message.md)です。</span><span class="sxs-lookup"><span data-stu-id="b5762-171">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="b5762-172">新しいメッセージの下書きを作成し、**ことを説明**する 1 つまたは複数オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="b5762-172">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="b5762-173">[Get](../api/user-list-messages.md#request-2)メッセージを私に言及しています。</span><span class="sxs-lookup"><span data-stu-id="b5762-173">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="b5762-174">[message](../resources/message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5762-174">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="b5762-175">**説明**のこのユーザーを含む、サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="b5762-175">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="b5762-176">メッセージの[取得](../api/message-get.md#request-2)とその評価</span><span class="sxs-lookup"><span data-stu-id="b5762-176">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="b5762-177">[message](../resources/message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b5762-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="b5762-178">メッセージを取得し、各**説明**メッセージの詳細を展開します。</span><span class="sxs-lookup"><span data-stu-id="b5762-178">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="b5762-179">メンションの削除</span><span class="sxs-lookup"><span data-stu-id="b5762-179">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="b5762-180">なし</span><span class="sxs-lookup"><span data-stu-id="b5762-180">None</span></span> |<span data-ttu-id="b5762-181">サインインしているユーザーのメールボックス内で指定したメッセージにおいて、指定したメンションを削除します。</span><span class="sxs-lookup"><span data-stu-id="b5762-181">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
