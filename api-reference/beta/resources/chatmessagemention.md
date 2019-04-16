---
title: chatMessageMention リソースの種類
description: 'chatmessage エンティティ内のメンションを表します。 メンションは、ユーザー、チーム、ボット、またはチャネルにすることができます。 '
localization_priority: Normal
author: nkramer
ms.openlocfilehash: 5d7304325e48c87bfd75b57bf49585f66a77b262
ms.sourcegitcommit: a39db1154a07aa0dd7e96fb6f9d7e891a812207e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/16/2019
ms.locfileid: "31889997"
---
# <a name="chatmessagemention-resource-type"></a><span data-ttu-id="e9ea5-104">chatMessageMention リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9ea5-104">chatMessageMention resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e9ea5-105">[chatmessage](chatmessage.md)エンティティ内のメンションを表します。</span><span class="sxs-lookup"><span data-stu-id="e9ea5-105">Represents a mention in a [chatMessage](chatmessage.md) entity.</span></span> <span data-ttu-id="e9ea5-106">メンションは、ユーザー、チーム、ボット、またはチャネルにすることができます。</span><span class="sxs-lookup"><span data-stu-id="e9ea5-106">The mention can be to a user, team, bot, or channel.</span></span> 

## <a name="properties"></a><span data-ttu-id="e9ea5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9ea5-107">Properties</span></span>
| <span data-ttu-id="e9ea5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9ea5-108">Property</span></span>     | <span data-ttu-id="e9ea5-109">型</span><span class="sxs-lookup"><span data-stu-id="e9ea5-109">Type</span></span>   |<span data-ttu-id="e9ea5-110">説明</span><span class="sxs-lookup"><span data-stu-id="e9ea5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e9ea5-111">id</span><span class="sxs-lookup"><span data-stu-id="e9ea5-111">id</span></span>|<span data-ttu-id="e9ea5-112">int</span><span class="sxs-lookup"><span data-stu-id="e9ea5-112">int</span></span>|<span data-ttu-id="e9ea5-113">記載されているエンティティのインデックス。</span><span class="sxs-lookup"><span data-stu-id="e9ea5-113">Index of the entity being mentioned.</span></span> <span data-ttu-id="e9ea5-114">メッセージ本文の<at id="index">タグと一致します。</span><span class="sxs-lookup"><span data-stu-id="e9ea5-114">Matches with the <at id="index"> tag of the message body.</span></span>|
|<span data-ttu-id="e9ea5-115">mentionText</span><span class="sxs-lookup"><span data-stu-id="e9ea5-115">mentionText</span></span>|<span data-ttu-id="e9ea5-116">string</span><span class="sxs-lookup"><span data-stu-id="e9ea5-116">string</span></span>|<span data-ttu-id="e9ea5-117">メンションを表すために使用される文字列。</span><span class="sxs-lookup"><span data-stu-id="e9ea5-117">String used to represent the mention.</span></span> <span data-ttu-id="e9ea5-118">たとえば、ユーザーの表示名、チーム名などです。</span><span class="sxs-lookup"><span data-stu-id="e9ea5-118">For example, User display name, Team name.</span></span>|
|<span data-ttu-id="e9ea5-119">明記</span><span class="sxs-lookup"><span data-stu-id="e9ea5-119">mentioned</span></span>|[<span data-ttu-id="e9ea5-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="e9ea5-120">identitySet</span></span>](identityset.md)|<span data-ttu-id="e9ea5-121">前述したエンティティ (ユーザー、アプリケーション、チーム、またはチャネル)。</span><span class="sxs-lookup"><span data-stu-id="e9ea5-121">The entity (user, application, team, or channel) that was mentioned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e9ea5-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9ea5-122">JSON representation</span></span>

<span data-ttu-id="e9ea5-123">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e9ea5-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.chatMessageMention"
}-->

```json
{
  "id": "number",
  "mentionText": "string",
  "mentioned": "microsoft.graph.identitySet"
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
