---
title: リソースの種類を説明します。
description: 相手の電子メール アドレスに基づいてユーザーに通知を表します。
author: simonhult
ms.openlocfilehash: a9c00daed067ecd41f0f687687ac9bf7f86d6f2c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334231"
---
# <a name="mention-resource-type"></a><span data-ttu-id="fea03-103">リソースの種類を説明します。</span><span class="sxs-lookup"><span data-stu-id="fea03-103">mention resource type</span></span>

> <span data-ttu-id="fea03-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fea03-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fea03-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fea03-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fea03-106">相手の電子メール アドレスに基づいてユーザーに通知を表します。</span><span class="sxs-lookup"><span data-stu-id="fea03-106">Represents a notification to a person based on the person's email address.</span></span> <span data-ttu-id="fea03-107">この通知の種類は、参照 @ とも呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="fea03-107">This type of notification is also known as @-mentions.</span></span>

<span data-ttu-id="fea03-108">[メッセージ](../resources/message.md)リソースは、**説明**をサポートします。</span><span class="sxs-lookup"><span data-stu-id="fea03-108">The [message](../resources/message.md) resource supports **mention**.</span></span> <span data-ttu-id="fea03-109">サインイン中のユーザーがそのメッセージ インスタンスに記載されているかどうかを示す**mentionsPreview**プロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fea03-109">It includes a **mentionsPreview** property that indicates whether the signed-in user is mentioned in that message instance.</span></span> <span data-ttu-id="fea03-110">**紹介**のナビゲーション プロパティを取得の詳細を記載されている、またはそのインスタンスの参照を削除するをサポートしているも含まれています。</span><span class="sxs-lookup"><span data-stu-id="fea03-110">It also includes the **mentions** navigation property, which supports getting details of a mention, or deleting a mention in that instance.</span></span>

<span data-ttu-id="fea03-111">メッセージを作成するには、アプリケーションを作成できます、記載されている同じ`POST`**に関する**プロパティで、説明を含めることによって要求されます。</span><span class="sxs-lookup"><span data-stu-id="fea03-111">When creating a message, an app can create a mention in the same `POST` request by including the mention in the **mentions** property.</span></span> <span data-ttu-id="fea03-112">使用して、`GET`の要求、`$filter`クエリ パラメーターでは、アプリ返すことができますすべてのメッセージで、サインインしているユーザーのメールボックスをユーザーに言及します。</span><span class="sxs-lookup"><span data-stu-id="fea03-112">Using a `GET` request with the `$filter` query parameter, an app can return all the messages in the signed-in user's mailbox that mention the user.</span></span> <span data-ttu-id="fea03-113">A`GET`の要求、`$expand`クエリのパラメーターは、特定のメッセージ内のすべての記述を展開してアプリケーションをことができます。</span><span class="sxs-lookup"><span data-stu-id="fea03-113">A `GET` request with the `$expand` query parameter lets the app expand all mentions in a specific message.</span></span>

<span data-ttu-id="fea03-114">アプリの中にアプリケーションを設定および参照投稿を行っているユーザーがメッセージの本文を作成する) などの既存のコンテキストで保持できる軽量の通知を有効に、メッセージで参照を取得することは、このメカニズムが基になる**紹介**プロパティを設定します。.</span><span class="sxs-lookup"><span data-stu-id="fea03-114">This mechanism of letting an app set and get mentions in messages enables lightweight notifications, where the user making the mention can remain in the existing context (such as composing a message body) while the app sets the underlying **mentions** property.</span></span> <span data-ttu-id="fea03-115">担当者が簡単に判りますし、によって記述されている`GET`が、要求、`$filter`または`$expand`パラメーターのクエリを実行します。</span><span class="sxs-lookup"><span data-stu-id="fea03-115">Mentioned persons can easily find out if and where they are mentioned through `GET` requests with the `$filter` or `$expand` query parameter.</span></span>  

<span data-ttu-id="fea03-116">Outlook メール クライアントが表示され、ユーザーが入力するときに、 `@` 、メッセージの作成中に Outlook により、ユーザーを選択するか、または @ 言及を完了するための名前を入力します。</span><span class="sxs-lookup"><span data-stu-id="fea03-116">For example, in the Outlook mail client, when a user types `@` while writing a message, Outlook lets the user select or enter a name to complete the @-mention.</span></span> <span data-ttu-id="fea03-117">作成し、メッセージまたはイベントを送信する前に、outlook は、"**説明**"プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="fea03-117">Outlook sets the **mentions** property before it creates and sends the message or event.</span></span> <span data-ttu-id="fea03-118">Outlook を使用しても`GET`での操作`$filter`と`$expand`、サインイン中のユーザー、ユーザーのことを説明するメッセージを検索できるように、迅速な対応を可能にするアクション アイテムや、ディスカッションをユーザーに警告します。</span><span class="sxs-lookup"><span data-stu-id="fea03-118">Outlook also uses `GET` operations with `$filter` and `$expand` to let the signed-in user look up messages that mention the user, alerting the user to action items or discussions, which allows for a faster response.</span></span>


## <a name="json-representation"></a><span data-ttu-id="fea03-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fea03-119">JSON representation</span></span>

<span data-ttu-id="fea03-120">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fea03-120">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="fea03-121">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fea03-121">Properties</span></span>
| <span data-ttu-id="fea03-122">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fea03-122">Property</span></span>     | <span data-ttu-id="fea03-123">種類</span><span class="sxs-lookup"><span data-stu-id="fea03-123">Type</span></span>   |<span data-ttu-id="fea03-124">説明</span><span class="sxs-lookup"><span data-stu-id="fea03-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fea03-125">application</span><span class="sxs-lookup"><span data-stu-id="fea03-125">application</span></span> | <span data-ttu-id="fea03-126">String</span><span class="sxs-lookup"><span data-stu-id="fea03-126">String</span></span> | <span data-ttu-id="fea03-127">参照投稿を作成するアプリケーションの名前。</span><span class="sxs-lookup"><span data-stu-id="fea03-127">The name of the application where the mention is created.</span></span> <span data-ttu-id="fea03-128">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fea03-128">Optional.</span></span> <span data-ttu-id="fea03-129">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="fea03-129">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="fea03-130">clientReference</span><span class="sxs-lookup"><span data-stu-id="fea03-130">clientReference</span></span> | <span data-ttu-id="fea03-131">String</span><span class="sxs-lookup"><span data-stu-id="fea03-131">String</span></span> | <span data-ttu-id="fea03-132">リソース インスタンスの親を表す一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="fea03-132">A unique identifier that represents a parent of the resource instance.</span></span> <span data-ttu-id="fea03-133">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fea03-133">Optional.</span></span> <span data-ttu-id="fea03-134">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="fea03-134">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="fea03-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="fea03-135">createdBy</span></span>  | [<span data-ttu-id="fea03-136">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fea03-136">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="fea03-137">参照投稿を行ったユーザーの電子メール情報。</span><span class="sxs-lookup"><span data-stu-id="fea03-137">The email information of the user who made the mention.</span></span> |
|<span data-ttu-id="fea03-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fea03-138">createdDateTime</span></span>  |<span data-ttu-id="fea03-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea03-139">DateTimeOffset</span></span> |<span data-ttu-id="fea03-140">クライアントでメンションが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="fea03-140">The date and time that the mention is created on the client.</span></span> |
|<span data-ttu-id="fea03-141">deepLink</span><span class="sxs-lookup"><span data-stu-id="fea03-141">deepLink</span></span> | <span data-ttu-id="fea03-142">String</span><span class="sxs-lookup"><span data-stu-id="fea03-142">String</span></span> | <span data-ttu-id="fea03-143">リソース インスタンスに記載されているのコンテキストへの高度な web リンク。</span><span class="sxs-lookup"><span data-stu-id="fea03-143">A deep web link to the context of the mention in the resource instance.</span></span> <span data-ttu-id="fea03-144">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fea03-144">Optional.</span></span> <span data-ttu-id="fea03-145">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="fea03-145">Not used and defaulted as null for **message**.</span></span> |
|<span data-ttu-id="fea03-146">id</span><span class="sxs-lookup"><span data-stu-id="fea03-146">id</span></span> | <span data-ttu-id="fea03-147">String</span><span class="sxs-lookup"><span data-stu-id="fea03-147">String</span></span>| <span data-ttu-id="fea03-148">リソース インスタンス内のメンションの一意の識別子。</span><span class="sxs-lookup"><span data-stu-id="fea03-148">The unique identifier of a mention in a resource instance.</span></span>|
|<span data-ttu-id="fea03-149">記載されています。</span><span class="sxs-lookup"><span data-stu-id="fea03-149">mentioned</span></span> | [<span data-ttu-id="fea03-150">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fea03-150">emailAddress</span></span>](../resources/emailaddress.md) | <span data-ttu-id="fea03-p110">メンションした人の電子メール情報。必須です。</span><span class="sxs-lookup"><span data-stu-id="fea03-p110">The email information of the mentioned person. Required.</span></span> |
|<span data-ttu-id="fea03-153">mentionText</span><span class="sxs-lookup"><span data-stu-id="fea03-153">mentionText</span></span> | <span data-ttu-id="fea03-154">String</span><span class="sxs-lookup"><span data-stu-id="fea03-154">String</span></span> | <span data-ttu-id="fea03-155">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fea03-155">Optional.</span></span> <span data-ttu-id="fea03-156">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="fea03-156">Not used and defaulted as null for **message**.</span></span> <span data-ttu-id="fea03-157">メッセージで、参照を取得するには、代わりに、メッセージの**bodyPreview**プロパティには、参照してください。</span><span class="sxs-lookup"><span data-stu-id="fea03-157">To get the mentions in a message, see the **bodyPreview** property of the message instead.</span></span> |
|<span data-ttu-id="fea03-158">serverCreatedDateTime</span><span class="sxs-lookup"><span data-stu-id="fea03-158">serverCreatedDateTime</span></span> | <span data-ttu-id="fea03-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fea03-159">DateTimeOffset</span></span> | <span data-ttu-id="fea03-160">日付と時刻、記載されているサーバー上で作成されます。</span><span class="sxs-lookup"><span data-stu-id="fea03-160">The date and time that the mention is created on the server.</span></span> <span data-ttu-id="fea03-161">省略可能。</span><span class="sxs-lookup"><span data-stu-id="fea03-161">Optional.</span></span> <span data-ttu-id="fea03-162">使用され、**メッセージ**の場合は null ではありません。</span><span class="sxs-lookup"><span data-stu-id="fea03-162">Not used and defaulted as null for **message**.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fea03-163">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fea03-163">Relationships</span></span>
<span data-ttu-id="fea03-164">なし</span><span class="sxs-lookup"><span data-stu-id="fea03-164">None</span></span>


## <a name="methods"></a><span data-ttu-id="fea03-165">メソッド</span><span class="sxs-lookup"><span data-stu-id="fea03-165">Methods</span></span>

| <span data-ttu-id="fea03-166">メソッド</span><span class="sxs-lookup"><span data-stu-id="fea03-166">Method</span></span>           | <span data-ttu-id="fea03-167">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fea03-167">Return Type</span></span>    |<span data-ttu-id="fea03-168">説明</span><span class="sxs-lookup"><span data-stu-id="fea03-168">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fea03-169">[投稿](../api/user-sendmail.md#request-2)および送信</span><span class="sxs-lookup"><span data-stu-id="fea03-169">[Post](../api/user-sendmail.md#request-2) and send</span></span> | <span data-ttu-id="fea03-170">なし</span><span class="sxs-lookup"><span data-stu-id="fea03-170">None</span></span> | <span data-ttu-id="fea03-171">作成し、新しいメッセージの一部として参照投稿を送信します。</span><span class="sxs-lookup"><span data-stu-id="fea03-171">Create and send mentions as part of a new message.</span></span>|
|<span data-ttu-id="fea03-172">新しい下書きを[投稿](../api/user-post-messages.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="fea03-172">[Post](../api/user-post-messages.md#request-2) to a new draft</span></span> | <span data-ttu-id="fea03-173">**説明**する 1 つまたは複数オブジェクトを含む[メッセージ](../resources/message.md)です。</span><span class="sxs-lookup"><span data-stu-id="fea03-173">[message](../resources/message.md) that contains one or more **mention** objects.</span></span> | <span data-ttu-id="fea03-174">新しいメッセージの下書きを作成し、**ことを説明**する 1 つまたは複数オブジェクトが含まれます。</span><span class="sxs-lookup"><span data-stu-id="fea03-174">Create a draft of a new message and include one or more **mention** objects.</span></span>|
|<span data-ttu-id="fea03-175">[Get](../api/user-list-messages.md#request-2)メッセージを私に言及しています。</span><span class="sxs-lookup"><span data-stu-id="fea03-175">[Get](../api/user-list-messages.md#request-2) messages mentioning me</span></span> | <span data-ttu-id="fea03-176">[message](../resources/message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fea03-176">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="fea03-177">**説明**のこのユーザーを含む、サインイン中のユーザーのメールボックス内のすべてのメッセージを取得します。</span><span class="sxs-lookup"><span data-stu-id="fea03-177">Get all the messages in the signed-in user's mailbox that contain a **mention** of this user.</span></span>|
|<span data-ttu-id="fea03-178">メッセージの[取得](../api/message-get.md#request-2)とその評価</span><span class="sxs-lookup"><span data-stu-id="fea03-178">[Get](../api/message-get.md#request-2) a message and its mentions</span></span> | <span data-ttu-id="fea03-179">[message](../resources/message.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="fea03-179">[message](../resources/message.md) collection</span></span> | <span data-ttu-id="fea03-180">メッセージを取得し、各**説明**メッセージの詳細を展開します。</span><span class="sxs-lookup"><span data-stu-id="fea03-180">Get a message and expand the details of each **mention** in the message.</span></span>|
|<span data-ttu-id="fea03-181">参照[の削除](../api/message-delete.md#request-2)</span><span class="sxs-lookup"><span data-stu-id="fea03-181">[Delete](../api/message-delete.md#request-2) a mention</span></span> | <span data-ttu-id="fea03-182">なし</span><span class="sxs-lookup"><span data-stu-id="fea03-182">None</span></span> |<span data-ttu-id="fea03-183">サインインしているユーザーのメールボックス内で指定したメッセージにおいて、指定したメンションを削除します。</span><span class="sxs-lookup"><span data-stu-id="fea03-183">Deletes the specified mention in the specified message in the signed-in user's mailbox.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->