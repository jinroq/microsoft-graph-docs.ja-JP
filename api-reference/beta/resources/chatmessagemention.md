---
title: chatMessageMention リソースの種類
description: 'chatmessage エンティティ内のメンションを表します。 メンションは、ユーザー、チーム、ボット、またはチャネルにすることができます。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 7dc2948821bee244e3ccde6e134a7ac2a201ad63
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543687"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="a89cf-104">chatMessageMention リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a89cf-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a89cf-105">[chatmessage](chatmessage.md)エンティティ内のメンションを表します。</span><span class="sxs-lookup"><span data-stu-id="a89cf-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="a89cf-106">メンションは、[ユーザー](user.md)、[チーム](team.md)、ボット、または[チャネル](channel.md)にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a89cf-106">The mention can be to a [user](user.md), [team](team.md), bot, or [channel](channel.md).</span></span> 

<span data-ttu-id="a89cf-107">1つまたは複数のメンションを含む**chatmessage**オブジェクトでは、メッセージ本文の**コンテンツ**プロパティは、HTML でチャットメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="a89cf-107">In a **chatMessage** object that contains one or more mentions, the message body **content** property represents the chat message in HTML.</span></span> <span data-ttu-id="a89cf-108">各メンションの**mentionText**を HTML `at`要素で囲みます。属性は`id` 、メンションの**id**プロパティに対応しています。</span><span class="sxs-lookup"><span data-stu-id="a89cf-108">It encloses the **mentionText** of each mention in an HTML `at` element, with an `id` attribute that corresponds to the **id** property of the mention.</span></span>

<span data-ttu-id="a89cf-109">一例として、チャットメッセージには2つのメンションが含まれており、それぞれに "Megan" と "Alex" という説明文があります。</span><span class="sxs-lookup"><span data-stu-id="a89cf-109">As an example, a chat message contains two mentions, with the mention text "Megan" and "Alex" respectively.</span></span> <span data-ttu-id="a89cf-110">body**コンテンツ**プロパティは、 `at` 2 つのメンションの要素を次のように指定します。</span><span class="sxs-lookup"><span data-stu-id="a89cf-110">Its body **content** property specifies `at` elements for the two mentions as follows:</span></span>

``` json
"body": {
    "contentType": "html",
    "content": "<div><div>Ah, <at id=\"0\">Megan</at>, <at id=\"1\">Alex</at>, I saw them in a separate folder. Thanks!</div>\n</div>"
}
```

<span data-ttu-id="a89cf-111">**コンテンツ**プロパティの最初のメンションには、0 `id`の HTML 属性があります。</span><span class="sxs-lookup"><span data-stu-id="a89cf-111">In the **content** property, the first mention has an HTML `id` attribute of 0.</span></span> <span data-ttu-id="a89cf-112">これは、 **chatMessageMention**の最初のインスタンスの**id**プロパティに対応します。これは0でもあります。</span><span class="sxs-lookup"><span data-stu-id="a89cf-112">This corresponds to the **id** property of that first instance of **chatMessageMention**, which is also 0.</span></span>

<span data-ttu-id="a89cf-113">2番目のメン`id`ションの属性は1で、2番目のインスタンスの**id**プロパティと一致します。1は1です。</span><span class="sxs-lookup"><span data-stu-id="a89cf-113">The second mention has an `id` attribute of 1, matching the **id** property of the second instance, which is 1.</span></span>

<span data-ttu-id="a89cf-114">この例の詳細については、「 [List channel message リプライ](../api/channel-list-messagereplies.md#example)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a89cf-114">For a fuller context of the example, see [List channel message replies](../api/channel-list-messagereplies.md#example).</span></span>

## <a name="properties"></a><span data-ttu-id="a89cf-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a89cf-115">Properties</span></span>
| <span data-ttu-id="a89cf-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a89cf-116">Property</span></span>     | <span data-ttu-id="a89cf-117">型</span><span class="sxs-lookup"><span data-stu-id="a89cf-117">Type</span></span>   |<span data-ttu-id="a89cf-118">説明</span><span class="sxs-lookup"><span data-stu-id="a89cf-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a89cf-119">id</span><span class="sxs-lookup"><span data-stu-id="a89cf-119">id</span></span>|<span data-ttu-id="a89cf-120">Int32</span><span class="sxs-lookup"><span data-stu-id="a89cf-120">Int32</span></span>|<span data-ttu-id="a89cf-121">指定した**chatmessage**で言及されているエンティティのインデックスです。</span><span class="sxs-lookup"><span data-stu-id="a89cf-121">Index of an entity being mentioned in the specified **chatMessage**.</span></span> <span data-ttu-id="a89cf-122">メッセージ本文の対応する`<at id="{index}">`タグの {index} 値と一致します。</span><span class="sxs-lookup"><span data-stu-id="a89cf-122">Matches the {index} value in the corresponding `<at id="{index}">` tag in the message body.</span></span>|
|<span data-ttu-id="a89cf-123">mentionText</span><span class="sxs-lookup"><span data-stu-id="a89cf-123">mentionText</span></span>|<span data-ttu-id="a89cf-124">string</span><span class="sxs-lookup"><span data-stu-id="a89cf-124">string</span></span>|<span data-ttu-id="a89cf-125">メンションを表すために使用される文字列。</span><span class="sxs-lookup"><span data-stu-id="a89cf-125">String used to represent the mention.</span></span> <span data-ttu-id="a89cf-126">たとえば、ユーザーの表示名、チーム名。</span><span class="sxs-lookup"><span data-stu-id="a89cf-126">For example, a user's display name, a team name.</span></span>|
|<span data-ttu-id="a89cf-127">明記</span><span class="sxs-lookup"><span data-stu-id="a89cf-127">mentioned</span></span>|[<span data-ttu-id="a89cf-128">identitySet</span><span class="sxs-lookup"><span data-stu-id="a89cf-128">identitySet</span></span>](identityset.md)|<span data-ttu-id="a89cf-129">前述したエンティティ (ユーザー、アプリケーション、チーム、またはチャネル)。</span><span class="sxs-lookup"><span data-stu-id="a89cf-129">The entity (user, application, team, or channel) that was mentioned.</span></span>  <span data-ttu-id="a89cf-130">@mentioned されたチャネルまたはチームの場合は、チーム/チャネルの ID を提供する**会話**プロパティと、チームまたはチャネルのいずれかを表す**conversationIdentityType**プロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="a89cf-130">If it was a channel or team that was @mentioned, the identitySet contains a **conversation** property giving the ID of the team/channel, and a **conversationIdentityType** property that represents either the team or channel.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a89cf-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a89cf-131">JSON representation</span></span>

<span data-ttu-id="a89cf-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a89cf-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": 1024,
  "mentionText": "string",
  "mentioned": {"@odata.type": "microsoft.graph.identitySet"}
 }

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "chat mention resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/chatmessagemention.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
