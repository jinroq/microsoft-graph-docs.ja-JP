---
title: 言及リソースの種類
description: 個人の電子メールアドレスに基づいて、ユーザーへの通知を表します。
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 28a77b393f2d5574453d08b93df487ffc5203e2c
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342325"
---
# <a name="mention-resource-type"></a><span data-ttu-id="bb77f-103">言及リソースの種類</span><span class="sxs-lookup"><span data-stu-id="bb77f-103">mention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb77f-104">個人の電子メールアドレスに基づいて、ユーザーへの通知を表します。</span><span class="sxs-lookup"><span data-stu-id="bb77f-104">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="bb77f-105">この種類の通知は、@ メンションとも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="bb77f-105">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="bb77f-106">[メッセージ](../resources/message.md)リソースは、**メンション**をサポートしています。</span><span class="sxs-lookup"><span data-stu-id="bb77f-106">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="bb77f-107">このプロパティには、サインインしているユーザーがそのメッセージインスタンスで言及されているかどうかを示す**mentionsPreview**プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb77f-107">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="bb77f-108">また、メン**ション**ナビゲーションプロパティも含まれています。これは、メンションの詳細を取得するか、そのインスタンス内のメンションを削除することをサポートします。</span><span class="sxs-lookup"><span data-stu-id="bb77f-108">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="bb77f-109">アプリケーションでは、メッセージを作成するときに、メン**ション**プロパティ`POST`にメンションを含めることによって、同じ要求でメンションを作成できます。</span><span class="sxs-lookup"><span data-stu-id="bb77f-109">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="bb77f-110">クエリパラメーター `GET`を指定して要求を使用すると、アプリはサインインしているユーザーのメールボックス内のすべてのメッセージを返し、そのユーザーに言及できます。 `$filter`</span><span class="sxs-lookup"><span data-stu-id="bb77f-110">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="bb77f-111">クエリパラメーターを使用して要求する`GET`と、特定のメッセージ内のすべてのメンションを展開できます。 `$expand`</span><span class="sxs-lookup"><span data-stu-id="bb77f-111">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="bb77f-112">メッセージでメンションを指定してメンションを取得するためのこのメカニズムにより、説明を作成しているユーザーが既存のコンテキスト (メッセージ本文の作成など) を既存のコンテキスト\*\*\*\* 内に残すことができます。.</span><span class="sxs-lookup"><span data-stu-id="bb77f-112">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="bb77f-113">指定された人物は、 `GET` `$filter`または`$expand`クエリパラメーターを使用して、要求によってどこにあるか、どこにあるかを簡単に確認できます。</span><span class="sxs-lookup"><span data-stu-id="bb77f-113">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="bb77f-114">たとえば、outlook メールクライアントでは、ユーザーがメッセージの作成`@`中に入力すると、ユーザーは名前を選択または入力して、@ メンションを完了できます。</span><span class="sxs-lookup"><span data-stu-id="bb77f-114">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="bb77f-115">Outlook は、メッセージまたはイベントを作成して送信する前に、**メンション**プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="bb77f-115">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="bb77f-116">Outlook で`GET` `$filter`は、および`$expand`を使用して、サインインしているユーザーに、ユーザーに通知するメッセージを検索させ、処理アイテムまたはディスカッションについての警告を表示して、応答を高速化することもできます。</span><span class="sxs-lookup"><span data-stu-id="bb77f-116">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="bb77f-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bb77f-117">JSON representation</span></span>

<span data-ttu-id="bb77f-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="bb77f-118">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="bb77f-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb77f-119">Properties</span></span>
| <span data-ttu-id="bb77f-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bb77f-120">Property</span></span>     | <span data-ttu-id="bb77f-121">型</span><span class="sxs-lookup"><span data-stu-id="bb77f-121">Type</span></span>   |<span data-ttu-id="bb77f-122">説明</span><span class="sxs-lookup"><span data-stu-id="bb77f-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb77f-123">application</span><span class="sxs-lookup"><span data-stu-id="bb77f-123">application</span></span> | <span data-ttu-id="bb77f-124">String</span><span class="sxs-lookup"><span data-stu-id="bb77f-124">String</span></span> | <span data-ttu-id="bb77f-125">メンションが作成されたアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="bb77f-125">The name of the application where the mention is created.</span></span> <span data-ttu-id="bb77f-126">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bb77f-126">Optional.</span></span> <span data-ttu-id="bb77f-127">使用されず、**メッセージ**の既定値として null になります。</span><span class="sxs-lookup"><span data-stu-id="bb77f-127">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="bb77f-128">clientreference</span><span class="sxs-lookup"><span data-stu-id="bb77f-128">clientReference</span></span> | <span data-ttu-id="bb77f-129">String</span><span class="sxs-lookup"><span data-stu-id="bb77f-129">String</span></span> | <span data-ttu-id="bb77f-130">リソースインスタンスの親を表す一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="bb77f-130">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="bb77f-131">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bb77f-131">Optional.</span></span> <span data-ttu-id="bb77f-132">使用されず、**メッセージ**の既定値として null になります。</span><span class="sxs-lookup"><span data-stu-id="bb77f-132">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="bb77f-133">createdBy</span><span class="sxs-lookup"><span data-stu-id="bb77f-133">createdBy</span></span>  | [<span data-ttu-id="bb77f-134">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bb77f-134">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="bb77f-135">メンションを行ったユーザーの電子メール情報。</span><span class="sxs-lookup"><span data-stu-id="bb77f-135">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="bb77f-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="bb77f-136">createdDateTime</span></span>  |<span data-ttu-id="bb77f-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb77f-137">DateTimeOffset</span></span> |<span data-ttu-id="bb77f-138">クライアントでメンションが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="bb77f-138">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="bb77f-139">リンク</span><span class="sxs-lookup"><span data-stu-id="bb77f-139">deepLink</span></span> | <span data-ttu-id="bb77f-140">String</span><span class="sxs-lookup"><span data-stu-id="bb77f-140">String</span></span> | <span data-ttu-id="bb77f-141">リソースインスタンス内のメンションのコンテキストへのディープ web リンク。</span><span class="sxs-lookup"><span data-stu-id="bb77f-141">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="bb77f-142">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bb77f-142">Optional.</span></span> <span data-ttu-id="bb77f-143">使用されず、**メッセージ**の既定値として null になります。</span><span class="sxs-lookup"><span data-stu-id="bb77f-143">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="bb77f-144">id</span><span class="sxs-lookup"><span data-stu-id="bb77f-144">id</span></span> | <span data-ttu-id="bb77f-145">String</span><span class="sxs-lookup"><span data-stu-id="bb77f-145">String</span></span>| <span data-ttu-id="bb77f-146">リソース インスタンス内のメンションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="bb77f-146">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="bb77f-147">明記</span><span class="sxs-lookup"><span data-stu-id="bb77f-147">mentioned</span></span> | [<span data-ttu-id="bb77f-148">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bb77f-148">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="bb77f-149">記載されているユーザーの電子メール情報。</span><span class="sxs-lookup"><span data-stu-id="bb77f-149">The email information of the mentioned person.</span></span> <span data-ttu-id="bb77f-150">必須です。</span><span class="sxs-lookup"><span data-stu-id="bb77f-150">Required.</span></span> |
|<span data-ttu-id="bb77f-151">mentionText</span><span class="sxs-lookup"><span data-stu-id="bb77f-151">mentionText</span></span> | <span data-ttu-id="bb77f-152">String</span><span class="sxs-lookup"><span data-stu-id="bb77f-152">String</span></span> | <span data-ttu-id="bb77f-153">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bb77f-153">Optional.</span></span> <span data-ttu-id="bb77f-154">使用されず、**メッセージ**の既定値として null になります。</span><span class="sxs-lookup"><span data-stu-id="bb77f-154">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="bb77f-155">メッセージ内のメンションを取得するには、代わりにメッセージの**bodyPreview**プロパティを参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb77f-155">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="bb77f-156">serverん datetime</span><span class="sxs-lookup"><span data-stu-id="bb77f-156">serverCreatedDateTime</span></span> | <span data-ttu-id="bb77f-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb77f-157">DateTimeOffset</span></span> | <span data-ttu-id="bb77f-158">メンションがサーバー上に作成された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="bb77f-158">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="bb77f-159">省略可能。</span><span class="sxs-lookup"><span data-stu-id="bb77f-159">Optional.</span></span> <span data-ttu-id="bb77f-160">使用されず、**メッセージ**の既定値として null になります。</span><span class="sxs-lookup"><span data-stu-id="bb77f-160">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="bb77f-161">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="bb77f-161">Relationships</span></span>
<span data-ttu-id="bb77f-162">なし</span><span class="sxs-lookup"><span data-stu-id="bb77f-162">None</span></span>


## <a name="methods"></a><span data-ttu-id="bb77f-163">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb77f-163">Methods</span></span>

| <span data-ttu-id="bb77f-164">メソッド</span><span class="sxs-lookup"><span data-stu-id="bb77f-164">Method</span></span>           | <span data-ttu-id="bb77f-165">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="bb77f-165">Return Type</span></span>    |<span data-ttu-id="bb77f-166">説明</span><span class="sxs-lookup"><span data-stu-id="bb77f-166">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bb77f-167">[投稿](../api/user-sendmail.md#request-2)と送信</span><span class="sxs-lookup"><span data-stu-id="bb77f-167">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="bb77f-168">なし</span><span class="sxs-lookup"><span data-stu-id="bb77f-168">None</span></span> | <span data-ttu-id="bb77f-169">新しいメッセージの一部としてメンションを作成して送信します。</span><span class="sxs-lookup"><span data-stu-id="bb77f-169">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="bb77f-170">新しい下書きに[投稿](../api/user-post-messages.md#request-2)する</span><span class="sxs-lookup"><span data-stu-id="bb77f-170">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="bb77f-171">1つまたは複数の**メンション**オブジェクトを含む[メッセージ](../resources/message.md)。</span><span class="sxs-lookup"><span data-stu-id="bb77f-171">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="bb77f-172">新しいメッセージの下書きを作成し、1つまたは複数の**メンション**オブジェクトを含めます。</span><span class="sxs-lookup"><span data-stu-id="bb77f-172">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="bb77f-173">自分宛てのメッセージを[取得](../api/user-list-messages.md#request-2)する</span><span class="sxs-lookup"><span data-stu-id="bb77f-173">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="bb77f-174">[message](../resources/message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bb77f-174">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="bb77f-175">このユーザーの**メンション**を含む、サインインしているユーザーのメールボックス内のすべてのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="bb77f-175">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="bb77f-176">メッセージとそのメンションを[取得](../api/message-get.md#request-2)する</span><span class="sxs-lookup"><span data-stu-id="bb77f-176">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="bb77f-177">[message](../resources/message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="bb77f-177">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="bb77f-178">メッセージを取得して、メッセージ内の各**メンション**の詳細を展開します。</span><span class="sxs-lookup"><span data-stu-id="bb77f-178">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="bb77f-179">メンションを[削除](../api/message-delete.md#request-2)する</span><span class="sxs-lookup"><span data-stu-id="bb77f-179">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="bb77f-180">なし</span><span class="sxs-lookup"><span data-stu-id="bb77f-180">None</span></span> |<span data-ttu-id="bb77f-181">サインインしているユーザーのメールボックス内で指定したメッセージにおいて、指定したメンションを削除します。</span><span class="sxs-lookup"><span data-stu-id="bb77f-181">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
