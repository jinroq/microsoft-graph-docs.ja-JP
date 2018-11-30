---
title: リソースの種類を説明します。
description: '相手の電子メール アドレスに基づいてユーザーに通知を表します。 この通知の種類とも呼ばれます '
ms.openlocfilehash: 7e70c6a84665b474ea4d8421f60e78687ebb49b6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067223"
---
# <a name="mention-resource-type"></a><span data-ttu-id="8322f-104">リソースの種類を説明します。</span><span class="sxs-lookup"><span data-stu-id="8322f-104">mention resource type</span></span>

> <span data-ttu-id="8322f-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8322f-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8322f-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8322f-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8322f-107">相手の電子メール アドレスに基づいてユーザーに通知を表します。</span><span class="sxs-lookup"><span data-stu-id="8322f-107">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="8322f-108">この通知の種類は、参照 @ とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="8322f-108">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="8322f-109">[メッセージ](../resources/message.md)リソースは、**説明**をサポートします。</span><span class="sxs-lookup"><span data-stu-id="8322f-109">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="8322f-110">サインイン中のユーザーがそのメッセージ インスタンスに記載されているかどうかを示す**mentionsPreview**プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8322f-110">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="8322f-111">**紹介**のナビゲーション プロパティを取得の詳細を記載されている、またはそのインスタンスの参照を削除するをサポートしているも含まれています。</span><span class="sxs-lookup"><span data-stu-id="8322f-111">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="8322f-112">メッセージを作成するには、アプリケーションを作成できます、記載されている同じ`POST`**に関する**プロパティで、説明を含めることによって要求されます。</span><span class="sxs-lookup"><span data-stu-id="8322f-112">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="8322f-113">使用して、`GET`の要求、`$filter`クエリ パラメーターでは、アプリ返すことができますすべてのメッセージで、サインインしているユーザーのメールボックスをユーザーに言及します。</span><span class="sxs-lookup"><span data-stu-id="8322f-113">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="8322f-114">A`GET`の要求、`$expand`クエリのパラメーターは、特定のメッセージ内のすべての記述を展開してアプリケーションをことができます。</span><span class="sxs-lookup"><span data-stu-id="8322f-114">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="8322f-115">アプリの中にアプリケーションを設定および参照投稿を行っているユーザーがメッセージの本文を作成する) などの既存のコンテキストで保持できる軽量の通知を有効に、メッセージで参照を取得することは、このメカニズムが基になる**紹介**プロパティを設定します。.</span><span class="sxs-lookup"><span data-stu-id="8322f-115">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="8322f-116">担当者が簡単に判りますし、によって記述されている`GET`が、要求、`$filter`または`$expand`パラメーターのクエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="8322f-116">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="8322f-117">Outlook メール クライアントが表示され、ユーザーが入力するときに、 `@` 、メッセージの作成中に Outlook により、ユーザーを選択するか、または @ 言及を完了するための名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="8322f-117">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="8322f-118">作成し、メッセージまたはイベントを送信する前に、outlook は、"**説明**"プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="8322f-118">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="8322f-119">Outlook を使用しても`GET`での操作`$filter`と`$expand`、サインイン中のユーザー、ユーザーのことを説明するメッセージを検索できるように、迅速な対応を可能にするアクション アイテムや、ディスカッションをユーザーに警告します。</span><span class="sxs-lookup"><span data-stu-id="8322f-119">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8322f-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8322f-120">JSON representation</span></span>

<span data-ttu-id="8322f-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8322f-121">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="8322f-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8322f-122">Properties</span></span>
| <span data-ttu-id="8322f-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8322f-123">Property</span></span>     | <span data-ttu-id="8322f-124">型</span><span class="sxs-lookup"><span data-stu-id="8322f-124">Type</span></span>   |<span data-ttu-id="8322f-125">説明</span><span class="sxs-lookup"><span data-stu-id="8322f-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8322f-126">application</span><span class="sxs-lookup"><span data-stu-id="8322f-126">application</span></span> | <span data-ttu-id="8322f-127">String</span><span class="sxs-lookup"><span data-stu-id="8322f-127">String</span></span> | <span data-ttu-id="8322f-128">参照投稿を作成するアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="8322f-128">The name of the application where the mention is created.</span></span> <span data-ttu-id="8322f-129">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8322f-129">Optional.</span></span> <span data-ttu-id="8322f-130">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="8322f-130">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="8322f-131">clientReference</span><span class="sxs-lookup"><span data-stu-id="8322f-131">clientReference</span></span> | <span data-ttu-id="8322f-132">String</span><span class="sxs-lookup"><span data-stu-id="8322f-132">String</span></span> | <span data-ttu-id="8322f-133">リソース インスタンスの親を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="8322f-133">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="8322f-134">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8322f-134">Optional.</span></span> <span data-ttu-id="8322f-135">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="8322f-135">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="8322f-136">createdBy</span><span class="sxs-lookup"><span data-stu-id="8322f-136">createdBy</span></span>  | [<span data-ttu-id="8322f-137">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8322f-137">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="8322f-138">参照投稿を行ったユーザーの電子メール情報。</span><span class="sxs-lookup"><span data-stu-id="8322f-138">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="8322f-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8322f-139">createdDateTime</span></span>  |<span data-ttu-id="8322f-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8322f-140">DateTimeOffset</span></span> |<span data-ttu-id="8322f-141">クライアントでメンションが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8322f-141">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="8322f-142">deepLink</span><span class="sxs-lookup"><span data-stu-id="8322f-142">deepLink</span></span> | <span data-ttu-id="8322f-143">String</span><span class="sxs-lookup"><span data-stu-id="8322f-143">String</span></span> | <span data-ttu-id="8322f-144">リソース インスタンスに記載されているのコンテキストへの高度な web リンク。</span><span class="sxs-lookup"><span data-stu-id="8322f-144">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="8322f-145">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8322f-145">Optional.</span></span> <span data-ttu-id="8322f-146">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="8322f-146">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="8322f-147">id</span><span class="sxs-lookup"><span data-stu-id="8322f-147">id</span></span> | <span data-ttu-id="8322f-148">String</span><span class="sxs-lookup"><span data-stu-id="8322f-148">String</span></span>| <span data-ttu-id="8322f-149">リソース インスタンス内のメンションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="8322f-149">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="8322f-150">記載されています。</span><span class="sxs-lookup"><span data-stu-id="8322f-150">mentioned</span></span> | [<span data-ttu-id="8322f-151">emailAddress</span><span class="sxs-lookup"><span data-stu-id="8322f-151">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="8322f-p111">メンションした人の電子メール情報。必須です。</span><span class="sxs-lookup"><span data-stu-id="8322f-p111">The email information of the mentioned person. Required.</span></span> |
|<span data-ttu-id="8322f-154">mentionText</span><span class="sxs-lookup"><span data-stu-id="8322f-154">mentionText</span></span> | <span data-ttu-id="8322f-155">String</span><span class="sxs-lookup"><span data-stu-id="8322f-155">String</span></span> | <span data-ttu-id="8322f-156">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8322f-156">Optional.</span></span> <span data-ttu-id="8322f-157">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="8322f-157">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="8322f-158">メッセージで、参照を取得するには、代わりに、メッセージの**bodyPreview**プロパティには、参照してください。</span><span class="sxs-lookup"><span data-stu-id="8322f-158">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="8322f-159">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="8322f-159">serverCreatedDateTime</span></span> | <span data-ttu-id="8322f-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8322f-160">DateTimeOffset</span></span> | <span data-ttu-id="8322f-161">日付と時刻、記載されているサーバー上で作成されます。</span><span class="sxs-lookup"><span data-stu-id="8322f-161">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="8322f-162">省略可能。</span><span class="sxs-lookup"><span data-stu-id="8322f-162">Optional.</span></span> <span data-ttu-id="8322f-163">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="8322f-163">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="8322f-164">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8322f-164">Relationships</span></span>
<span data-ttu-id="8322f-165">なし</span><span class="sxs-lookup"><span data-stu-id="8322f-165">None</span></span>


## <a name="methods"></a><span data-ttu-id="8322f-166">メソッド</span><span class="sxs-lookup"><span data-stu-id="8322f-166">Methods</span></span>

| <span data-ttu-id="8322f-167">メソッド</span><span class="sxs-lookup"><span data-stu-id="8322f-167">Method</span></span>           | <span data-ttu-id="8322f-168">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8322f-168">Return Type</span></span>    |<span data-ttu-id="8322f-169">説明</span><span class="sxs-lookup"><span data-stu-id="8322f-169">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8322f-170">[投稿](../api/user-sendmail.md#request-2)および送信</span><span class="sxs-lookup"><span data-stu-id="8322f-170">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="8322f-171">なし</span><span class="sxs-lookup"><span data-stu-id="8322f-171">None</span></span> | <span data-ttu-id="8322f-172">作成し、新しいメッセージの一部として参照投稿を送信します。</span><span class="sxs-lookup"><span data-stu-id="8322f-172">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="8322f-173">新しい下書きを[投稿](../api/user-post-messages.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="8322f-173">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="8322f-174">**説明**する 1 つまたは複数オブジェクトを含む[メッセージ](../resources/message.md)です。</span><span class="sxs-lookup"><span data-stu-id="8322f-174">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="8322f-175">新しいメッセージの下書きを作成し、**ことを説明**する 1 つまたは複数オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="8322f-175">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="8322f-176">[Get](../api/user-list-messages.md#request-2)メッセージを私に言及しています。</span><span class="sxs-lookup"><span data-stu-id="8322f-176">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="8322f-177">[message](../resources/message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8322f-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="8322f-178">**説明**のこのユーザーを含む、サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="8322f-178">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="8322f-179">メッセージの[取得](../api/message-get.md#request-2)とその評価</span><span class="sxs-lookup"><span data-stu-id="8322f-179">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="8322f-180">[message](../resources/message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8322f-180">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="8322f-181">メッセージを取得し、各**説明**メッセージの詳細を展開します。</span><span class="sxs-lookup"><span data-stu-id="8322f-181">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="8322f-182">参照[の削除](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="8322f-182">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="8322f-183">なし</span><span class="sxs-lookup"><span data-stu-id="8322f-183">None</span></span> |<span data-ttu-id="8322f-184">サインインしているユーザーのメールボックス内で指定したメッセージにおいて、指定したメンションを削除します。</span><span class="sxs-lookup"><span data-stu-id="8322f-184">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->